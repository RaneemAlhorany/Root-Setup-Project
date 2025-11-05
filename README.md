# Root-Setup-Project
It's stage 0 in your PHP language learning journey

project (1) : Root Setup Project

    ? goal (Learn how to):
        1) Install and run PHP locally
        2) Create your first PHP file
        3) See PHP and HTML working together

1) install local server
   
         Steps: How to install a local server
   
            In this stage: we will install the XAMPP server
            Note: Official website link:
[click here Official website ](https://www.apachefriends.org/)            
  
   Steps to install XAMPP
            
              1) Go to the official XAMPP website:
                         https://www.apachefriends.org/
                
             2) Download the XAMPP installer suitable for your operating system 
                    (Windows, macOS, or Linux)
        
             3) Run the installer as Administrator
        
             4) Follow the installation wizard:
                # Choose the components you want to install 
                      (Apache, MySQL, PHP, phpMyAdmin, etc.)
                # Select the installation folder 
                    (default: C:\xampp)
                  ! Note: It's important to remember this path because your projects will be stored inside it
                # Continue until installation begins
        
             5) Once installation is complete launch the XAMPP Control Panel
        
             6) Start the Apache and MySQL modules by clicking the "Start" buttons
        
             7) To verify the installation:
                 Open your browser and go to: http://localhost/
                 If you see the XAMPP dashboard, installation was successful.
        
             8) To access phpMyAdmin:
                 Go to: http://localhost/phpmyadmin/
    
  Tip:
  
         If Apache doesn't start, check if another program (like Skype or IIS)
         is using port 80 or 443.
         You can change the port in:
         XAMPP Control Panel -> Config -> Apache (httpd.conf)
    
   Note:
   
         All your projects should be placed inside the "htdocs" folder.
         Example path: C:\xampp\htdocs\
    
   How to run your project:
    
         1) Open your browser
         2) Type in the URL bar: 
           http://localhost/projectFolder/fileName.php
    
   Example:

         If your folder is named "myapp" and file is "index.php"
         Then type: http://localhost/myapp/index.php
         
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

   
2)  PHP Introduction
 
          # PHP is a server-side scripting language used to create dynamic web pages.
          # It can be embedded inside HTML.
        
         The file extension should always be: .php
                  nameFile.php
        
   Note:
   
            If you want to use PHP code inside HTML, the file must have a .php extension
        
  Difference between HTML and PHP files:
  
             .html → supports only client-side code (HTML, CSS, JS)
             .php  → supports both client-side and server-side code (HTML + PHP)
        
  Example:Embedding PHP inside HTML
        
        <!DOCTYPE html>
        <html>
            <body>
                <h1>
                    <?php
                        echo "This is my first PHP line inside HTML!";
                    ?>
                </h1>
            </body>
        </html>
        
////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

3) Basic PHP Structure

   The PHP code should be written as follows:
   
        <?php
            // Write your PHP code between these tags
        ?>
        
    Syntax of the print statement in PHP:
   
             echo "text";
            
   Example 1: Printing a simple text
   
        <?php
            echo "Hi!";
        ?>
        
   Note:
   
            1) Every PHP statement must end with a semicolon (;)
            2) echo is used to display text or variable values on the web page
            3) Strings can be written using single (' ') or double (" ") quotes

//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////////

4) method

 Function: date()
         
  Purpose:
  
             To get and format the current date and time in PHP
         
   Information:
   
             The date() function in PHP is used to format and display the current date and time
            
  Prototype:
  
            string date(string $format);
            
  Description:
  
            # Returns the current date and time formatted according to the specified pattern
            # Common format characters:
                    Y → Year (4 digits)
                    m → Month (2 digits)
                    d → Day (2 digits)
                    H → Hour (24-hour format)
                    i → Minutes
                    s → Seconds
                    
  ^ Examples:
        
            echo date("Y-m-d H:i:s");
            Output: 2025-11-05 12:30:45 (example)
            
            echo date("d-m-Y");
            Output: 05-11-2025 (example)
            
            echo date("H:i");
            Output: 14:22 (example - time only)
    
  Notes:
  
            # The function uses the server’s local time by default.
            # You can change the timezone using:
                date_default_timezone_set("Asia/Amman");
example :

    date_default_timezone_set("Asia/Amman"); // Set timezone
    echo "Current Jordan time: " . date("Y-m-d H:i:s");
  
