# README
Resume Builder
def generate_resume():
    name = input("Enter your full name: ")
    email = input("Enter your email address: ")
    education = input("Enter your education background: ")
    experience = input("Enter your work experience: ")
    skills = input("Enter your skills: ")

    resume_content = f"""
    # {name}'s Resume
    
    ## Contact Information
    Email: {email}
    
    ## Education
    {education}
    
    ## Work Experience
    {experience}
    
    ## Skills
    {skills}
    """

    with open("resume.md", "w") as file:
        file.write(resume_content)

if __name__ == "__main__":
    generate_resume()
