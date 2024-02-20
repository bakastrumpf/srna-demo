# srna-demo: "A Serbian Dictionary of recent Anglicisms"
<br>
A full-stack Java project.
<br><br>

<p>This is a demo project to display the development of a dictionary in the form of a Java web app after its print version has already been released. Dictionary entries that I rely on in my DB can be found in the “Serbian dictionary of recent Anglicisms” (Serbian original: <i><a href=”https://digitalna.ff.uns.ac.rs/sadrzaj/2021/978-86-6065-636-2”>Srpski rečnik novijih anglicizama</a></i>, short: <i>SRNA</i>).</p>
<br>

<p>
For the frontend part,  I rely on the MVC architecture with the combo of HTML, CSS, and Bootstrap. 
</p>
<br>

<p>
Secondly, for the database, I use mariaDB dialect of MySQL.
</p>
<p>
A dictionary entry has 8 fields visible to the guest (orthography, pronunciation, unacceptable forms, original English form with its adaptation to Serbian, meaning, usage examples, fixed expressions or collocations, cross references) and 4 fields visible to authors and associates (id, author, source, date [automatically recorded when the entry is added]). The presentation of a dictionary entry is constant and does not change.
</p>
<br>

<p>Finally, for the backend part, the app is written in Java, relying on Spring and Spring Boot. Later, once all this is functional, I may write the logic in PHP as well, relying on the same DB and frontend.
</p>
<br>

<p>The dict web app works with two types of entities: 
<ol>
<li>users: admin, author, associate, guest, and</li>
<li>dictionary entries</li>
</ol>
<br>

<p>
All users but guests have an id, name, last name, email, password, and a role; and can edit their profile data, but cannot delete their profile. The guest user is the only user who cannot register himself. Only admin can add a new user or delete a user. Only authors can delete dictionary entries. Associates can add and edit dictionary entries. A guest can only browse and preview dictionary entries.
</p>
<br>

<p>
A user can login and logout. Upon successful login, a user is allowed access to the functionalities defined for the user role.
</p>
<br>

<p>
<u>Problems</u>
<ul>
<li>
Exception handling: when a guest performs a search with no results (null value), display a message?
</li>
<li>
How to display dictionary entries that have multiple meanings? Are they separate entries, or should they be displayed within a single, umbrella entry?
</li>
<li>
In the beginning, before enabling work with DB, maybe use dictionary entries in JSON files stored within the project code.
</li>
</ul>
<br>

<br><br>
Description to be updated in the future.
<hr>