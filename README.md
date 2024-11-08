"# Email_Slicer" 
 
def email_slicer(email):
    # Check if email contains "@" and "." to ensure it's valid
    if "@" in email and "." in email:
        # Split the email into username and domain parts
        username, domain = email.split("@")
        return username, domain
    else:
        return "Invalid email format"
 
# Get email input from the user
email_input = input("Enter an email address: ")
 
# Call the function to slice the email
result = email_slicer(email_input)
 
# Output the result
if isinstance(result, tuple):
    print(f"Username: {result[0]}")
    print(f"Domain: {result[1]}")
else:
    print(result)
has context menu
