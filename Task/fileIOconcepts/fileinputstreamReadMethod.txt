package org.jsp.app10;

import java.io.FileInputStream;
import java.io.FileNotFoundException;

public class FileInputStreamMethodsMainClass {

	public static void main(String[] args) {
		// TODO Auto-generated method stub

		try {
			FileInputStream input=new FileInputStream("input.txt");
			input.read();
			input.read();
			
			System.out.println("Data is :"+input.available());
			input.read();
			input.mark(2);
			input.read();
			input.read();
			input.reset();
			System.out.println("Dta is :"+ input.available());
			
		}
		catch (Exception e) {
			// TODO Auto-generated catch block
			e.printStackTrace();
		}
		
	}

}
output:-
Data is :36
Dta is :33
