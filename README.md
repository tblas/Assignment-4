Titanium.UI.setBackgroundColor('#000');

var win1 = Titanium.UI.createWindow({  //Windows
    text: 'Katie Gregory',
    backgroundColor:'#008080'
});
var DetailedWindow = Ti.UI.createWindow({
	text:'More Info.',
	backgroundColor:'#fff'
});
var titleView = Ti.UI.createView({		//Titles
	height: '20%',
	width: '100%',
	top:'0%',
	backgroundImage: '/Images/UIEF Flat Creek.jpg'
});
var titleLabel = Ti.UI.createLabel({
	text:'Katie Gregory',
	left: '45%',
	height: Ti.UI.FILL,
	font:{
			fontSize:'75sp',
			fontWeight:'bold',
			fontColor:'#000000'
	}									
});
var MoreinfoTitleView = Ti.UI.createView({
	top: 0,
	backgroundColor: 'black',
	height:'20%',
	width: '100%',
});
var MoreinfoTitleLabel = Ti.UI.createLabel({
	text:'More Information',
	textAlign: 'center',
	color: '#008080',
	height:Ti.UI.FILL,
	font:{
		fontSize:'75sp',
		fontWeight:'bold',
	}
});
var ContactList = Ti.UI.createView({				//HOME SCREEN
	height:'13%',
	width:'45%',
	left:'35%',
	top: '40%',				
});
var contactInfo = Ti.UI.createLabel({
	text: 'Katie Gregory \nUniversity of Idaho /nCollege of Businesss and Economics \n HR and Operations Mgt.\nPhone: (208) 841-8979 \nEmail:greg5562@uidaho.edu',
	textAlign:'center',
	height:Ti.UI.FILL,
	font:{
		fontSize:'25sp'
	}
});
var HomeScrnPic = Ti.UI.createView({
	height:'35%',
	width:'80%',
	left:'20%',
	bottom: 0,
	borderRadius: 20,
	backgroundImage:'/Images/V_F167.jpg'
});
var returnView = Ti.UI.createView({		//ButtonViews
	bottom: '0',
	left: 0,
	height:'10%',
	width:'100%',
	backgroundColor:'black'
});
var MoreinfoView = Ti.UI.createView({		
	height: '20%',
	width: '20%',
	left: 0,
	top: '20%'
});
var blurbView = Ti.UI.createView({
	top: '22%',
	left: '20%',
	height: '15%',
	width: '80%',
});	
var MoreinfoWindView = Ti.UI.createView({
	height: '70%',
	width: '100%',
	top: '20%',
	bottom: '5%',
	backgroundImage: '/Images/Bus 353- Final Resume Image.JPG',
});		

var blurbLabel = Ti.UI.createLabel({		
	textAlign: 'center',
	top: '5%',
	text: 'My name is Katie Gregory. I am currently a senior at the University of Idaho. I enjoy the outdoors and traveling. Under the ‘More info.’ Tab you will find my resume with a more detailed portfolio of who I am.  ',
	font:{
		fontSize:'25sp',
		fontWeight:'bold',
	}	
});

var MoreinfoButton = Ti.UI.createButton({			//Buttons
	title: 'More Info.',
		color:'#008080',
		height:Ti.UI.FILL,
		width:'100%',
		height: '100%',
		borderColor: '#008080',							
		textAlign:'Center',
		font:{
			fontSize:'35sp',
			fontWeight:'bold'
		},
		backgroundColor:'black'
});
var BackButton = Ti.UI.createButton({
	title:'Back',
	color:'black',
	borderRadius: 10,
	height:Ti.UI.FILL,
	width:'15%',
	height:'100%',
	left: 0,
	bordercolor:'black',
	backgroundColor: '#008080',
	textAlign:'center',
	font:{
		fontSize:'35sp',
		fontWeight:'bold',
	},
	backgroundcolor:'#808080'
});
MoreinfoButton.addEventListener('click', function(e){
	win1.close();
	MoreinfoWindow.close();
	MoreinfoWindow.open();
});
BackButton.addEventListener('click', function(e){
	win1.open();
});

win1.open();
win1.add(titleView);
titleView.add(titleLabel);
win1.add(MoreinfoView);
win1.add(blurbView);
win1.add(HomeScrnPic);
win1.add(ContactList);
DetailedWindow.add(BackView);
MoreinfoWindow.add(MoreinfoTitleView);
MoreinfoWindow.add(MoreinfoWindView);


blurbView.add(blurbLabel);
MoreinfoView.add(MoreinfoButton);
returnView.add(BackButton);
MoreinfoTitleView.add(MoreinfoTitleLabel);
ContactList.add(contactInfo);

Bus 353- Final Resume Image.JPG
UIEF Flat Creek.jpg
V__F167.jpg
