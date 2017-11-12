# deng
package denglu;

import java.awt.*;
import javax.swing.*;

public class LoginFrame extends JFrame{
	private JPanel contentpane;
	private JTextField textField;
	private JLabel lblNewLabel_1;
	private JTextField textField_1;
	private JButton btnNewButton;
	private JButton btnNewButton_1;
	
	public LoginFrame(){
		setTitle("登录");
		setDefaultCloseOperation(JFrame.EXIT_ON_CLOSE);
		setBounds(100,100,377,264);
		this.setSize(400,300);
		this.setLocation(450,240);
		JPanel panel=new JPanel();
		panel.setBorder(UIManager.getBorder("ScrollPane.border"));
		GridBagLayout gbl_panel=new GridBagLayout();
		panel.setLayout(gbl_panel);
		
		
		JLabel lblNewLabel=new JLabel("用户：");
		lblNewLabel.setFont(new Font("华文仿宋",Font.BOLD,14));
		lblNewLabel.setVerticalAlignment(SwingConstants.TOP);
		GridBagConstraints gbc_lblNewLabel=new GridBagConstraints();
		gbc_lblNewLabel.fill=GridBagConstraints.HORIZONTAL;
		gbc_lblNewLabel.insets=new Insets(0,0,5,5);
		gbc_lblNewLabel.anchor=GridBagConstraints.EAST;
		gbc_lblNewLabel.gridx=3;
		gbc_lblNewLabel.gridy=2;
		panel.add(lblNewLabel,gbc_lblNewLabel);
		
		textField=new JTextField();
		textField.setFont(new Font("华文仿宋",Font.BOLD,14));
		GridBagConstraints gbc_textField=new GridBagConstraints();
		gbc_textField.fill=GridBagConstraints.HORIZONTAL;
		gbc_textField.insets=new Insets(0,0,5,5);
		gbc_textField.anchor=GridBagConstraints.NORTHWEST;
		gbc_textField.gridx=4;
		gbc_textField.gridy=2;
		gbc_textField.gridwidth=4;
		panel.add(textField,gbc_textField);
		textField.setColumns(10);
		
		lblNewLabel_1=new JLabel("密码：");
		lblNewLabel_1.setFont(new Font("华文仿宋",Font.BOLD,14));
		GridBagConstraints gbc_lblNewLabel_1=new GridBagConstraints();
		gbc_lblNewLabel_1.fill=GridBagConstraints.HORIZONTAL;
		gbc_lblNewLabel_1.anchor=GridBagConstraints.EAST;
		gbc_lblNewLabel_1.insets=new Insets(0,0,5,5);
		gbc_lblNewLabel_1.gridx=3;
		gbc_lblNewLabel_1.gridy=3;
		panel.add(lblNewLabel_1,gbc_lblNewLabel_1);
		
		textField_1=new JTextField();
		textField_1.setFont(new Font("华文仿宋",Font.BOLD,14));
		GridBagConstraints gbc_textField_1=new GridBagConstraints();
		gbc_textField_1.insets=new Insets(0,0,5,5);
		gbc_textField_1.fill=GridBagConstraints.HORIZONTAL;
		gbc_textField_1.gridx=4;
		gbc_textField_1.gridy=3;
		gbc_textField_1.gridwidth=4;
		panel.add(textField_1,gbc_textField_1);
		textField.setColumns(10);
		
		btnNewButton=new JButton("登录");
		btnNewButton.setFont(new Font("华文仿宋",Font.BOLD,14));
		GridBagConstraints gbc_btnNewButton=new GridBagConstraints();
		gbc_btnNewButton.insets=new Insets(10,2,0,5);
		gbc_btnNewButton.gridx=4;
		gbc_btnNewButton.gridy=5;
		gbc_btnNewButton.gridheight=2;
		gbc_btnNewButton.anchor=GridBagConstraints.SOUTH;
		panel.add(btnNewButton,gbc_btnNewButton);
		
		btnNewButton_1=new JButton("取消");
		btnNewButton_1.setFont(new Font("华文仿宋",Font.BOLD,14));
		GridBagConstraints gbc_btnNewButton_1=new GridBagConstraints();
		gbc_btnNewButton_1.insets=new Insets(10,2,0,5);
		gbc_btnNewButton_1.gridx=5;
		gbc_btnNewButton_1.gridy=5;
		gbc_btnNewButton_1.gridheight=2;
		gbc_btnNewButton_1.anchor=GridBagConstraints.SOUTH;
		panel.add(btnNewButton_1,gbc_btnNewButton_1);
		this.add(panel,BorderLayout.CENTER);
		this.setVisible(true);
	}
}
