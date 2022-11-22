<h1>1: Create a bucket</h1>

Navigation menu > Cloud Storage > Browser > Create Bucket<br>
Name your bucket > "Name as per given in lab" > Continue<br>
Choose where to store your data > Region: us-east1 > Continue<br>
Use default for the remaining<br>
Create<br>

<h1>2: Create a Pub/Sub topic</h1>

Navigation menu > Pub/Sub > Topics<br>
Create Topic > Name:  "Name as per given in lab" > Create Topic<br>


<h1>3: Create the thumbnail Cloud Function</h1>

Navigation menu > Cloud Functions > Create Function<br>
Use the following config:<br>
Name: "Name as per given in lab" <br> Region: us-east1 <br> Trigger: Cloud Storage <br> Event type: Finalize/Create <br> Bucket: BROWSE > Select the qwiklabs bucket<br>
Remaining default > Next<br>
Runtime: Node.js 10 Entry point: thumbnail<br>
Add the code appropiately<br>
Download the image from URL<br>
Navigation menu > Cloud Storage > Browser > Select your bucket > Upload files<br>
Refresh bucket<br>


<h1>4: Remove the previous cloud engineer</h1>

Navigation menu > IAM & Admin > IAM<br>
Search for the "Username 2" > Edit > Delete Role<br>
