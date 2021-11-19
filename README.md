# Sprint1
import java.util.Scanner;

/**
 *
 * @author Roo
 */
public /abstract/ class User {

    String userName;
    String password;
    String mobileNumber;
    String email;

    public User(String userName, String password, String mobileNumber, String email) {
        this.userName = userName;
        this.password = password;
        this.mobileNumber = mobileNumber;
        this.email = email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    public void setUserName(String userName) {
        this.userName = userName;
    }

    public void setPassword(String password) {
        this.password = password;
    }

    public void setMobileNumber(String mobileNumber) {
        this.mobileNumber = mobileNumber;
    }

    public String getUserName() {
        return userName;
    }

    public String getPassword() {
        return password;
    }

    public String getMobileNumber() {
        return mobileNumber;
    }

    public String getEmail() {
        return email;
    }
  
    public static void main(String args[]) throws Exception {
        Scanner sc = new Scanner(System.in);
        System.out.print("enter your username");
        String user = sc.nextLine();
        System.out.print("enter your password");
        String pass = sc.nextLine();
         System.out.print("enter your mobile number");
        String number = sc.nextLine();
        System.out.print("enter your email");
        String email = sc.nextLine();
        User login =new User(user,pass,number,email) ;
        
        
}}
