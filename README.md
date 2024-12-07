Online Voting Portal

This project is an Online Voting Portal built using Python and the Django framework. It allows users to register, vote for candidates, and view results securely. The system integrates two-factor authentication (2FA) using OTP and facial recognition using the LBPH algorithm in OpenCV.

Features:

User Registration & Authentication: Secure user registration and login with OTP-based two-factor authentication.
Voting: Users can vote for candidates in an election, with the system ensuring that each user can vote only once.
Candidate Management: Admins can add, remove, or update candidate details.
Facial Recognition: Utilizes OpenCV's LBPH algorithm for facial recognition to enhance security and verify user identity.
Results Display: Real-time election results are displayed, showing the total votes per candidate.
Technologies Used

Frontend: HTML, CSS, JavaScript (for basic interactivity)
Backend: Django (Python)
Database: PostgreSQL
Authentication: OTP-based 2FA, Facial Recognition (OpenCV)


Installation

Clone the repository:
git clone https://github.com/your-username/online-voting-portal.git
cd online-voting-portal

Setup Virtual Environment (optional but recommended):
python3 -m venv venv
source venv/bin/activate  # On Windows, use `venv\Scripts\activate`

Install Dependencies:
pip install -r requirements.txt

Setup Database:
Make sure PostgreSQL is installed and configured. Then, run the following command to apply migrations:
python manage.py migrate

Run the Development Server:
python manage.py runserver
Visit http://127.0.0.1:8000/ in your browser to access the portal.

Usage:

User Registration:
New users can register with their email and phone number.
OTP will be sent to their phone for verification.

Voting:
After logging in, users can vote for a candidate.
Voting is only allowed once per user.

Admin Panel:
Admins can manage candidates and view election results.

Facial Recognition:
During registration, users will need to upload a photo for facial recognition, which will be used during the login process for verification.
