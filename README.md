# contabancaria
package com.mycompany.contabancaria1;
/**
 *
 * @author Paulo
 */
public class Conta {
    private int numeroConta;
    private String donoConta;
    private double saldo;
    private double limite;
    
    public double getSaldo(){
        return this.saldo;
    }
    public double setSaldo(double saldo){
        return this.saldo = saldo;
    }
    
    public double setLimite(double limite){
        return this.limite = limite;
    }
    
    void sacarDinheiro(double quantia){
        this.saldo -= quantia;
    }
    
    void depositarDinheiro(double quantia){
        this.saldo += quantia;
    }