# Simulated Ticket Log

All 6 tickets are **simulated** for practice. Every response follows the same structure:

**Acknowledge → Diagnose → Resolve → Confirm → Close**


---

## TICKET #001: Printer won't print

**User:** I have been trying to print the month-end report for 30 minutes and nothing comes out. The printer says it's online. This is so frustrating, I need this before 2pm!
**Category:** Hardware / Printer
**Priority:** Medium

---

## Response

**Acknowledge:** Hello Temilade, thank you for reporting this. I understand 
this is blocking your work and I'll help you resolve it right away.

**Diagnose:** Could you confirm whether the printer shows as “Offline” 
on your computer? In the meantime, please check that the printer is 
powered on and connected to the same network as your laptop.

**Resolve:** Based on similar cases, this is often caused by a stalled 
print spooler. Please try: (1) Restart the Print Spooler service, 
(2) Remove and re-add the printer. Step-by-step instructions are here: [link].

**Confirm:** Once you've tried this, please let me know if the printer 
appears online and whether a test page prints successfully.

**Close:** If the issue persists, I will escalate this to the network 
team for a deeper check. Thank you for your patience.

**Resolution notes (internal):** Stuck job cleared from print queue, print spooler service restarted. Root cause: large PDF job failed mid-spool. Resolved in 15 minutes.


---

## TICKET #002: Laptop running very slowly

**User:** My laptop has been getting slower and slower for weeks. It takes 5 minutes to start and Excel freezes. Please help.
**Category:** Hardware
**Priority:** Low

---

## Response

**Acknowledge:** Hello Mike, slowdowns are quite common and fixable, I am sorry that this is affecting your work.

**Diagnose:** We need to find out what is making use of your Pc's resources. Please press *Ctrl + Shift + Esc* to open Task Manager and tell me which items are highest under CPU, Memory and Disk. Also, how many programs open when you start the laptop, and roughly how full is your C: drive?

**Resolve:** Common fixes: (1) disable unnecessary startup apps in the Task Manager *Startup* tab; (2) free disk space (Settings → System → Storage, then use Storage Sense); (3) install pending Windows updates; (4) run a full antivirus scan. Please restart afterwards.

**Confirm:** Once you've tried this, Let me know whether startup time and Excel are better. If not, I'd like to check the hard drive health, and if a RAM or SSD upgrade may be needed.

**Close:** I'll close this once performance is acceptable.

**Resolution notes (internal):** 11 startup items disabled, 18 GB freed, updates installed. Boot time reduced from about 5 min to under 1 min. Recommended an SSD upgrade at next hardware refresh.


---

## TICKET #003: Cannot open shared drive

**User:** I can't open the shared "Operations" folder since this morning. It says "Windows cannot access \\fileserver\November-report". My whole team needs the files.
**Category:** Network
**Priority:** High

---

## Response

**Acknowledge:** Hello Ngozi, Thanks for the clear details. Because your whole team depends on this folder, I'm treating it as high priority.

**Diagnose:** First I need to know whether this affects only you or the whole team. Can your colleagues open the folder? Are you connected to the office network (or VPN if remote)?

**Resolve:** If it's only you: please restart your computer and try again. If it still fails, I'll check that your account still has permission to the folder and that your computer can reach the file server. If your colleagues also can't open it, I will escalate to the server/network team right away and keep you updated.

**Confirm:** Please let me know what your colleagues are seeing. I'll update you within 30 minutes either way.

**Close:** Once access is restored and verified by you, I'll close the ticket.

**Resolution notes (internal):** Only Ngozi was affected. Drive mapping was lost after an update; re-mapped the network drive and confirmed group membership. No server issue.


---

## TICKET #004: Suspicious email, user clicked a link

**User:** I got an email saying my bank account will be suspended and I clicked the link and entered my email password. Now I'm worried. What do I do?
**Category:** Security / Phishing
**Priority:** Critical

---

## Response

**Acknowledge:** Hello Maxwell, Thank you for reporting this straight away. That was exactly the right thing to do, and you are not in trouble. 

**Diagnose:** This looks like a phishing attack. Because you entered your email password, we must assume it's compromised. Please disconnect your laptop from Wi-Fi/network now, but keep it on. Do not delete the email.

**Resolve:** I'm taking these steps now: (1) resetting your email password and signing out all active sessions; (2) enabling multi-factor authentication; (3) checking your mailbox for unusual sign-ins; (4) running a full malware scan on your laptop; (5) notifying the security Team. Please also change your password on any other site where you used the same one, and contact your bank directly if you entered any banking details.

**Confirm:** Please call me so I can talk you through the reset. I'll update you after the scan.

**Close:** The ticket stays open until the scan is clean, MFA is on and the security Team signs off. A short follow-up note on spotting phishing will be sent to you.

**Resolution notes (internal):** Escalated to security lead as an incident. Password reset, sessions revoked, MFA enabled, no malicious inbox rules found, scan clean. Sender domain blocked. Suggested a phishing awareness reminder for the team.


---

## TICKET #005: Forgot password / account locked

**User:** I came back from leave and forgot my password. I tried several times and now it says my account is locked. I can't work at all!
**Category:** Accounts / Account Lockout
**Priority:** High

---

## Response

**Acknowledge:** Welcome back Nwachukwu, and sorry for the poor start. A lockout is a security feature, and it's easy to fix.

**Diagnose:** Too many failed attempts triggers an automatic lock. Before I make any changes, I need to verify your identity. Please confirm your employee ID and your department manager's name. For security, please do **not** send your password in this ticket.

**Resolve:** Once verified, I'll unlock your account and issue a temporary password through a secure channel. You'll be prompted to create a new password at first login. It should be at least 12 characters, combining words, numbers and symbols.

**Confirm:** Please log in and tell me whether it worked. If you'd like, I can show you how to set up the self-service password reset to avoid this in the future.

**Close:** I'll close the ticket after you confirm a successful login.

**Resolution notes (internal):** Identity verified via employee ID and manager name. Account unlocked, temporary password given via phone, forced change at next login. Recommended password manager.


---

## TICKET #006: Can't connect to office Wi-Fi

**User:** My laptop can see the office Wi-Fi but it says "Can't connect to this network". Everyone else is online. I have a client call in an hour and can't even open my email.
**Category:** Network / Wi-Fi
**Priority:** High

---

## Response

**Acknowledge:** Hi Omotola, Thank you for letting us know. With a client call coming up, I'm treating this as a priority.

**Diagnose:** Since other people are connected, the problem is likely with your laptop's saved connection rather than the office network. Let's start by confirming Wi-Fi is on and Airplane mode is off.

**Resolve:** Please try this: *Settings → Network & internet → Wi-Fi → Manage known networks → select the office network → Forget*. Then reconnect and re-enter the Wi-Fi password. If that fails, restart your laptop and try again.

**Confirm:** Let me know if you're online. If it still fails, please send me the exact wording of the error message and I'll check whether your device is blocked or has a wrong IP address on the router.

**Close:** Once you're connected and can open your email, I'll close the ticket.

**Resolution notes (internal):** Stale saved profile after Wi-Fi password change. Forgetting the network and reconnecting fixed it. Advised user to expect the same on their phone.