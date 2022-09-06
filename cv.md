***Sergey Kurmel***
**********************************
Mobile: +375297604056

Mail: kurmels@gmail.com

LinkedIn: sergey-kurmel-ba396659

Skype: kurmel_s 

Discord: Sergey Kurmel
==================================

***Summary***
**********************************
I am currently studying Javascript diligently. 
My goal is to gain knowledge and skills that will be enough for employment in the company. 
I want to learn everything new and interesting.
==================================

***SKILLS***
**********************************
Java Core 

HTML, CSS, JavaScript

Git, GitHub

SQL, MySQL

XML 

Strong knowledge of Object-Oriented principles Good understanding of design patterns and Agile methodologies  

Knowledge of Clean Code Experience with software development methodologies
==================================

***Code examples***
**********************************
'''

Function GetUserDocInternetAddress (username As String) As String

	Dim books As Variant
	
	Dim viewNames As NotesView
	
	Dim done As Variant
	
	done = False
	
	books = session.AddressBooks
	
	GetUserDocInternetAddress=""
	
	ForAll dbNames In books
	
		If ( dbNames.IsPublicAddressBook ) And ( Not done )  Then
		
			done = True
			
			Call dbNames.Open( "", "" )
			
			'Print "Èñïîëüçóåì  names.nsf íà ñåðâåðå "+dbNames.Server
			
			Set viewNames = dbNames.GetView("($VIMPeople)")	
			
			Set GetUserDoc = viewNames.GetDocumentByKey(username)
			
			If Not GetUserDoc Is Nothing Then
			
				GetUserDocInternetAddress=GetUserDoc.InternetAddress(0)
				
			End If
			
		End If
		
	End ForAll	
	
End Function

'''
==================================

***Experience***
**********************************
Designing, developing, implementing, integrating and supporting custom developed on the Lotus platform.
==================================

***EDUCATION***
**********************************
BELARUSIAN STATE UNIVERSITY OF INFORMATICS 
AND  RADIOELECTRONICS 

Electronic and optical hardware engineering 2003–2008

Faculty of Computer-Aided Design
==================================

***English***
**********************************
Knowledge of English at the Intermediate level.
==================================

