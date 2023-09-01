---
permalink: /contact/
layout: page
title: Contact Information
subtitle: 
---

<div id="summerOfficeHours">
    <!-- Summer office hours go here -->
    <h2>Summer Office Hours</h2>
    <p><strong>Mon:</strong> By appointment<br />
    <strong>Tues:</strong> 9:00am - 2:00pm<br />
    <strong>Wed:</strong> 9:00am - 2:00pm<br />
    <strong>Thur:</strong> 9:00am - 2:00pm<br />
    <strong>Fri:</strong> By appointment</p>
</div>

<div id="regularOfficeHours">
    <!-- Regular office hours go here -->
    <h2>Office Hours</h2>
    <p><strong>Mon:</strong> 8:00am - 3:30pm<br />
    <strong>Tues:</strong> 8:00am - 3:30pm<br />
    <strong>Wed:</strong> 8:00am - 3:30pm<br />
    <strong>Thur:</strong> 8:00am - 3:30pm<br />
    <strong>Fri:</strong> 8:00am - 3:30pm</p>
</div>

<!-- Contact Numbers -->
<h2>Contact Numbers</h2>
<p><strong>Phone:</strong> <a href="tel:+17724611225">1-772-461-1225</a><br />
Office: Ext. 1<br />
Administrator: Ext. 2<br />
<!---Parsonage: Ext. 3<br />--->
<strong>Fax:</strong> 772-461-1226</p>

<!-- Email -->
<h2>Email</h2>
<p>General Inquiries: <a href="mailto:office@oabcministries.org">office@oabcministries.org</a><br />
Records Request: <a href="mailto:records@oabcministries.org">records@oabcministries.org</a></p>

<script>
    // Function to display office hours based on the current month
    function displayOfficeHours() {
        var today = new Date();
        var currentMonth = today.getMonth() + 1; // Months are zero-based, so add 1
        var summerMonths = [5, 6, 7]; // May, June, and July are summer months

        var summerOfficeHoursDiv = document.getElementById('summerOfficeHours');
        var regularOfficeHoursDiv = document.getElementById('regularOfficeHours');

        if (summerMonths.includes(currentMonth)) {
            summerOfficeHoursDiv.style.display = 'block'; // Show summer office hours
            regularOfficeHoursDiv.style.display = 'none'; // Hide regular office hours
        } else {
            summerOfficeHoursDiv.style.display = 'none'; // Hide summer office hours
            regularOfficeHoursDiv.style.display = 'block'; // Show regular office hours
        }
    }

    // Call the function to initially display the correct office hours
    displayOfficeHours();
</script>
