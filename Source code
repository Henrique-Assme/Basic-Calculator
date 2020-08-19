package com.example.calculadora;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.text.TextUtils;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {
    EditText num1, num2;
    Button somar, subtrair, multiplicar, dividir, limpar;
    Float n1, n2, result;
    String message;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        num1 = (EditText) findViewById(R.id.editTextNum1);
        num2 = (EditText) findViewById(R.id.editTextNum2);
        somar = (Button) findViewById(R.id.btnSoma);
        subtrair = (Button) findViewById(R.id.btnSubtracao);
        multiplicar = (Button) findViewById(R.id.btnMultiplicacao);
        dividir = (Button) findViewById(R.id.btnDivisao);
        limpar = (Button) findViewById(R.id.btnLimpar);
        somar.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                if(TextUtils.isEmpty(num1.getText().toString()) || TextUtils.isEmpty(num2.getText().toString())){
                    num1.setError("Digite o número");
                    num2.setError("Digite o número");
                }
                else{
                    n1 = Float.parseFloat(num1.getText().toString());
                    n2 = Float.parseFloat(num2.getText().toString());
                    result = n1+n2;
                    message = result.toString();
                    Toast.makeText(MainActivity.this, message, Toast.LENGTH_LONG).show();
                }
            }
        });
        subtrair.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                if(TextUtils.isEmpty(num1.getText().toString()) || TextUtils.isEmpty(num2.getText().toString())){
                    num1.setError("Digite o número");
                    num2.setError("Digite o número");
                }
                else{
                    n1 = Float.parseFloat(num1.getText().toString());
                    n2 = Float.parseFloat(num2.getText().toString());
                    result = n1-n2;
                    message = result.toString();
                    Toast.makeText(MainActivity.this, message, Toast.LENGTH_LONG).show();
                }
            }
        });
        multiplicar.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                if(TextUtils.isEmpty(num1.getText().toString()) || TextUtils.isEmpty(num2.getText().toString())){
                    num1.setError("Digite o número");
                    num2.setError("Digite o número");
                }
                else{
                    n1 = Float.parseFloat(num1.getText().toString());
                    n2 = Float.parseFloat(num2.getText().toString());
                    result = n1*n2;
                    message = result.toString();
                    Toast.makeText(MainActivity.this, message, Toast.LENGTH_LONG).show();
                }
            }
        });
        dividir.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                if(TextUtils.isEmpty(num1.getText().toString()) || TextUtils.isEmpty(num2.getText().toString())){
                    num1.setError("Digite o número");
                    num2.setError("Digite o número");
                }
                else{
                    n1 = Float.parseFloat(num1.getText().toString());
                    n2 = Float.parseFloat(num2.getText().toString());
                    if(n2==0){
                        Toast.makeText(MainActivity.this, "Divisão por zero é indeterminada!", Toast.LENGTH_LONG).show();
                    }
                    else{
                        result = n1/n2;
                        message = result.toString();
                        Toast.makeText(MainActivity.this, message, Toast.LENGTH_LONG).show();
                    }
                }
            }
        });
        limpar.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                num1.setText("");
                num2.setText("");
            }
        });
    }
}
