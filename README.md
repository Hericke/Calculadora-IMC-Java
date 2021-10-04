# Calculadora-IMC-Java
Calculadora de IMC exercício de Java
import javax.swing.JOptionPane;
import java.text.DecimalFormat;

public class CalculadoraImc {public static void main(String args[]){
    double altura ,peso, imc;
    altura=Double.parseDouble(JOptionPane.showInputDialog("Digite sua altura"));
    peso= Double.parseDouble(JOptionPane.showInputDialog("Digite seu Peso"));
     imc = peso / (altura * altura);
     DecimalFormat decimal = new DecimalFormat("0.00");
     String valorFormato =decimal.format(imc);
     if (imc >=18.5 && imc <= 24.9){
         JOptionPane.showMessageDialog(null,"IMC ="+valorFormato+"Peso Normal");

     } else if (imc >=25 && imc <= 29.9){
         JOptionPane.showMessageDialog(null,"IMC ="+valorFormato+"Sobre peso");

     } else if (imc >=30 && imc <= 34.9){
         JOptionPane.showMessageDialog(null,"IMC ="+valorFormato+"Obeso");


     } else if (imc >=35 && imc <= 39.9) {
         JOptionPane.showMessageDialog(null, "IMC =" + valorFormato + "obesidade Tipo II");

     } else if (imc >=40 )
         JOptionPane.showMessageDialog(null, "IMC =" + valorFormato + "obesidade Tipo II");

    {

}
}}
