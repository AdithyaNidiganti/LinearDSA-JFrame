# LinearDSA-JFrame

import java.awt.EventQueue;
import javax.swing.JFrame;
import javax.swing.JPanel;
import javax.swing.border.EmptyBorder;
import javax.swing.JLabel;
import javax.swing.JButton;
import javax.swing.JToggleButton;
import javax.swing.JTextField;
import javax.swing.SwingConstants;
import java.awt.event.ActionListener;
import java.awt.event.WindowEvent;
import java.awt.event.ActionEvent;
import java.awt.Font;
import java.awt.Toolkit;
import java.beans.PropertyChangeListener;
import java.beans.PropertyChangeEvent;
public class LinearDSA extends JFrame {
private static final long serialVersionUID = 1L;
public static void main(String[] args) {
EventQueue.invokeLater(new Runnable() {
public void run() {
try {
LinearDSA frame = new LinearDSA();
frame.setVisible(true);
} catch (Exception e) {
e.printStackTrace();
}
}
});
}
public void close() {
WindowEvent closeWindow = new WindowEvent(this, WindowEvent.WINDOW_CLOSING);
Toolkit.getDefaultToolkit().getSystemEventQueue().postEvent(closeWindow);
}
public LinearDSA() {
setDefaultCloseOperation(JFrame.DISPOSE_ON_CLOSE);
setBounds(100, 100, 450, 300);
JPanel contentPane = new JPanel();
contentPane.addPropertyChangeListener(new PropertyChangeListener() {
public void propertyChange(PropertyChangeEvent evt) {
}
});
contentPane.setBorder(new EmptyBorder(5, 5, 5, 5));

setContentPane(contentPane);
contentPane.setLayout(null);
JButton btnNewButton = new JButton("Queue");
btnNewButton.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("Queue");
array.setVisible(true);
}
});
btnNewButton.setBounds(48, 177, 89, 23);
contentPane.add(btnNewButton);
JButton btnNewButton_1 = new JButton("Circular Queue");
btnNewButton_1.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("CircularQueue");
array.setVisible(true);
}
});
btnNewButton_1.setBounds(267, 75, 103, 23);
contentPane.add(btnNewButton_1);

JButton btnNewButton_2 = new JButton("Stack");
btnNewButton_2.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("Stack");
array.setVisible(true);
}
});
btnNewButton_2.setBounds(48, 127, 89, 23);
contentPane.add(btnNewButton_2);
JButton btnNewButton_3 = new JButton("DoubleLinkedList");
btnNewButton_3.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("DoublyLinkedList");
array.setVisible(true);
}
});
btnNewButton_3.setBounds(267, 177, 103, 23);
contentPane.add(btnNewButton_3);
JButton btnNewButton_4 = new JButton("Array");
btnNewButton_4.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("Array");
array.setVisible(true);	
}
});
btnNewButton_4.setBounds(48, 75, 89, 23);
contentPane.add(btnNewButton_4);

JButton btnNewButton_5 = new JButton("SingleLinkedList");
btnNewButton_5.addActionListener(new ActionListener() {
public void actionPerformed(ActionEvent e) {
close();
DSA array = new DSA("SingleLinkedList");
array.setVisible(true);
}
});
btnNewButton_5.setBounds(267, 127, 103, 23);
contentPane.add(btnNewButton_5);
JLabel lblNewLabel = new JLabel("Data Structures");
lblNewLabel.setFont(new Font("Tahoma", Font.BOLD, 20));
lblNewLabel.setBounds(135, 11, 166, 23);
contentPane.add(lblNewLabel);
}
 }
