import javax.swing.*;
import java.awt.*;
import java.awt.event.ActionEvent;
import java.awt.event.ActionListener;

class A extends JFrame{
	JPanel p,p1,p2;
	JLabel l,l1,l2,l3,l4;
	JTextField t,t1,t2;
	JButton b,b1;
	
	class B implements ActionListener{
		@Override
		public void actionPerformed(ActionEvent e) {
			try {
				double p=Double.parseDouble(t.getText());
				double r=Double.parseDouble(t1.getText());
				double u=Double.parseDouble(t2.getText());
				l4.setText(p*r*u/100+"");
			}catch( Exception ex) {
				JOptionPane.showMessageDialog(null, "Invalid input");
			}
		}
	}
	
	class C implements ActionListener{
		@Override
		public void actionPerformed(ActionEvent e) {
			l4.setText(null);
			t.setText(null);
			t1.setText(null);
			t2.setText(null);
		}
	}
	
	A(){
		setSize(416,400);
		setTitle("SIP Calculator");
		setLocationRelativeTo(null);
		getContentPane().setBackground(Color.lightGray);;
		setDefaultCloseOperation(JFrame.DISPOSE_ON_CLOSE);
		setLayout(null);
		
		p = new JPanel();
		p.setBounds(10, 10, 380, 200);
		p.setBackground(Color.DARK_GRAY);
		add(p);
		p.setLayout(null);
		
		
		l = new JLabel("Enter prenciple amount (rs) =");
		l.setBounds(20, 10, 200, 20);
		l.setForeground(Color.white);
		p.add(l);
		
		l1 = new JLabel("Enter rate of interest (%) = ");
		l1.setBounds(20, 60, 200, 20);
		l1.setForeground(Color.white);
		p.add(l1);
		
		l2 = new JLabel("Enter time period (years)  = ");
		l2.setBounds(20, 110, 200, 20);
		l2.setForeground(Color.white);
		p.add(l2);
		
		t=new JTextField();
		t.setBounds(200,10,150,20);
		p.add(t);
		
		t1=new JTextField();
		t1.setBounds(200,60,150,20);
		p.add(t1);
		
		t2=new JTextField();
		t2.setBounds(200,110,150,20);
		p.add(t2);
		
		b = new JButton("Calculate");
		b.addActionListener(new B());
		b.setBounds(220,150,100,20);
		p.add(b);
		
		p1=new JPanel();
		p1.setBounds(10, 230, 380, 120);
		p1.setBackground(Color.DARK_GRAY);
		add(p1);
		p1.setLayout(null);
		
		l3 = new JLabel("Simple interest (%)   = ");
		l3.setBounds(40, 30, 150,20);
		l3.setForeground(Color.white);
		p1.add(l3);
		
		p2 = new JPanel();
		p2.setBounds(180,30,150,20);
		p1.add(p2);
		
		l4 =new JLabel();
		l4.setBounds(160,30,150,20);
		p2.add(l4);
		
		b1 = new JButton("Clear");
		b1.addActionListener(new C());
		b1.setBounds(200,70,100,20);
		p1.add(b1);
		
	}
}

public class SIP {
	public static void main(String[] args) {
		A a = new A();
		a.setVisible(true);
	}
}
