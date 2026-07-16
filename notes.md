# Project 12. Session Hijacking

# Part 1 – Session Hijacking Fundamentals

## Objective

The main goal of this part is to understand how Session Hijacking works. This includes learning about session management, session identifiers, cookies and security best practices. These are the basics that we need to know before we can do the demonstrations that are covered later in this project.

---

# Session

When you use a website it needs to remember who you are. This is where a session comes in. A session is like a way that websites keep track of what you are doing on their site. The websites server keeps all the information about your session. This happens after you log in successfully. Every time you visit a page on the site your browser sends a special code to the server. This code is called the Session ID.

### Key Points

- The server is in charge of the session.

- A session starts after you log in.

- The Session ID is like a name tag that says who you are.

- The session ends when you log out or when it times out.

---

# Session ID (Session Token)

The Session ID is a code that the server gives you when you log in. This code is like a password that only the server and your browser know. When you visit a page your browser sends this code to the server so it knows who you are. You do not have to log in

### Characteristics

- The Session ID is randomly generated.

- Every time you log in you get a Session ID.

- The Session ID is used to say who you are.

- It is hard to guess what the Session ID is.

---

# Methods Used to Exchange Session IDs

Websites use ways to send Session IDs back and forth.

### Common Methods

- Hidden fields on forms

- Cookies which're the most common way

Cookies are used the most because your browser automatically sends them to the website every time you visit.

---

# Cookies

Cookies are pieces of information that the website stores on your browser. They help the website remember who you are and what you like. The website sends cookies to your browser. Then your browser sends them back to the website. This helps the website give you an experience.

### Purpose

- Cookies help the website remember who you are.

- They store your preferences.

- They help make the website more personal.

![Alt text](screenshots/session-management-concepts.png)

**Session Management Concepts**

```text

session-management-concepts.png

```

Take a look at Page 3 of the CEHv13 Session Hijacking module. It shows:

- What a session is

- What a Session ID is

- What a Session Token is

- What cookies are

- Different attack methods

- Session Sniffing

---

# Session Hijacking

Session Hijacking is when someone steals your Session ID and uses it to pretend to be you. If someone gets your Session ID they can get into your account without knowing your password.

### Objectives of an Attacker

- Steal Session IDs.

- Get around the login process.

- Get information.

- Pretend to be an user.

![Alt text](screenshots/session-hijacking-diagram.png)

**Session Hijacking**

```text

session-hijacking-diagram.png

```

Take a look at Page 4 of the CEHv13 Session Hijacking module. It shows:

- What Session Hijacking is

- How to stop it

---

# Attack Methods

There are ways to do Session Hijacking. Some ways involve the server. Some involve the client.

### Server-Side Attacks

- Guessing Session IDs

- Session Fixation

- Session Sniffing

### Client-Side Attacks

- Cross-Site Scripting, which is also called XSS

---

# Session Sniffing

Session Sniffing is when someone listens in on your internet traffic to get your Session ID or cookies. If they get this information they can pretend to be you and get into your accounts.

This can lead to:

- Identity Theft

- Information Theft

- Fraud

- Getting into your accounts without permission

---

# Countermeasures

## General User Best Practices

- Do not click on links in emails.

- Always log out when you are done.

- Keep your browser up, to date.

- Clear your browsing data, including your cache and cookies.

## Web Developer Best Practices

- Make Session IDs that are hard to guess.

- Give a Session ID when someone logs in.

- Keep session data secret.

- End sessions when someone logs out.

- Use firewalls to block malicious traffic.

---

# Key Concepts Learned

- What a session is

- What a Session ID is

- What a Session Token is

- What cookies are

- What Session Hijacking is

- What Session Sniffing is

- What Session Fixation is

- What Cross-Site Scripting is (XXS)

- How to keep sessions secure

- How to stop Session Hijacking

---

# conclusion

In this part I learned how websites use Session IDs and cookies to remember who you are. 
I also learned how attackers can steal Session IDs and how to stop them. This will help me understand how to keep my accounts safe.
