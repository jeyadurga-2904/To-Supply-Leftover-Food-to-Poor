# 🥘 To Supply Leftover Food to Poor

A **Salesforce-based cloud application** designed to collect and distribute surplus food from restaurants, households, and events to the poor and needy.  
This project aims to **reduce food wastage** and **combat hunger** through an automated, transparent, and efficient food distribution system.

---

## 👥 Team Details

**Project Title:** To Supply Leftover Food to Poor  
**Team Leader:** Jeya Durga R (913022104007)  
**Team Members:**  
- Naveetharan T (913022104301)  
- Nithishkumar R (913022104023)  
- Jaya Akash R (913022104037)  

**Institution:** University College of Engineering, Ramanathapuram  
*(A Constituent College of Anna University, Chennai – 600025)*  
**Course:** Bachelor of Engineering – Computer Science and Engineering  
**Semester:** 7th (Final Year)  
**Project Duration:** Naan Mudhalvan Project (Nov–Dec 2025)

---

## 📘 Abstract

The **Leftover Food Distribution System** automates the entire process — from donor registration to food pickup, volunteer assignment, and delivery confirmation — using Salesforce tools like **Flows**, **Apex Triggers**, **Reports**, and **Dashboards**.

The project’s main objective is to minimize food waste while promoting social welfare by connecting **food donors** with **volunteers/NGOs** who deliver food to those in need.

---

## 🚀 Features

- 👩‍🍳 **Donor Registration:** Restaurants, event organizers, and households can log surplus food details.  
- 🚴 **Volunteer Assignment:** Volunteers receive real-time notifications to pick up food.  
- 🕒 **Real-Time Tracking:** Track food pickup and delivery status dynamically.  
- 📊 **Reports & Dashboards:** View metrics on donations, volunteers, and beneficiaries.  
- 💬 **Feedback System:** Collect feedback from donors and recipients to improve transparency.

---

## 🧩 Tools & Technologies

- **Platform:** Salesforce CRM  
- **Automation:** Flows & Apex Triggers  
- **Notifications:** Email Alerts  
- **Analytics:** Reports & Dashboards  

---

## 🧠 System Workflow

1. Donor registers leftover food details.  
2. Volunteer/NGO accepts the pickup request.  
3. Food is collected and delivered to the needy.  
4. Delivery status and feedback are recorded.  
5. Reports and dashboards track overall impact.  

---

## ⚙️ Implementation Details

### Custom Objects
- **Donor**  
- **Food Listing**  
- **Pickup Request**  
- **Delivery**  
- **Feedback**

### Key Fields
- *Food Type*, *Quantity*, *Expiry Time* (Food Listing)  
- *Status*, *Assigned Volunteer* (Pickup Request)  
- *Delivery Time*, *Location* (Delivery)  
- *Rating*, *Comments* (Feedback)

### Sample Apex Trigger
```apex
trigger DropOffTrigger on Drop_Off_point__c (before insert) {
    for (Drop_Off_point__c drop : Trigger.new) {
        drop.Distance__c = drop.distance_calculation__c;
    }
}
```

### Flows
- **Flow 1:** Auto-updates status to “Delivered” after confirmation.  
- **Flow 2:** Sends alerts to volunteers when new food is listed.

---

## 📈 Reports & Dashboards

- **Report:** Food Donation Report — grouped by Food Type & Delivery Status  
- **Dashboard:** Donation Impact Dashboard — visualizes number of donations, volunteers, and beneficiaries served.

---

## 🧾 Challenges & Solutions

| Challenge | Solution |
|------------|-----------|
| “Submit” button not visible in Flow | Adjusted screen size and saved |
| Error while updating delivery status | Fixed picklist values and field references |
| Missing custom fields in object | Verified API names and re-added fields |

---

## 🎥 Demonstration

- When a donor adds food details, a volunteer is automatically notified via email.  
- Upon successful delivery, the system updates status and records feedback.

🔗 **Demo Links:**  
- [GitHub Repository](https://github.com/jeyadurga-2904/To-Supply-Leftover-Food-to-Poor)  
- [SmartInternz Workspace](https://nme.smartinternz.com/Student/guided_project_workspace/3739)

---

## ✅ Conclusion

The project effectively reduces food wastage by connecting donors and volunteers through Salesforce automation.  
It ensures **transparency**, **efficiency**, and **real-time coordination**, promoting a sustainable and hunger-free community.

---

## 🔮 Future Enhancements

- Develop dedicated **login portals** for donors and volunteers.  
- Integrate with **local NGOs and food banks**.  
- Launch **mobile app** for faster updates and tracking.

---

## 📚 References

1. [Salesforce Trailhead Documentation](https://trailhead.salesforce.com)  
2. [SmartInternz Naan Mudhalvan Portal](https://nme.smartinternz.com)  
3. [Salesforce Developer Guide](https://developer.salesforce.com)  
4. [GitHub Repository](https://github.com/jeyadurga-2904/To-Supply-Leftover-Food-to-Poor)
