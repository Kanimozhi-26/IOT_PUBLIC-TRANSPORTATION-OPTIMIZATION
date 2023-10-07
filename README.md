Abstract: 
Public transport can play an important role in reducing usage of privatevehicles by individuals which can, in turn, reduce traffic congestion, pollution, andusage of fossil fuel. But, for that public transport needs to be reliable. People shouldnot have to wait for the bus for a long time without having any idea when the buswill come. Further, people should get a seat in the bus. To ensure this, 
efficientlyandaccuratelyschedulingandprovisioningofbusesisofparamountimportan ce.Infact, nowadays buses are scheduled as per the need. But these scheduling is beingdonemanuallyinIndiase1Oursurveyshowsthattherearemanyalgorithmsproposedi n the literature for scheduling and provisioning of buses. There is a need to tailorthese algorithms for Indian scenario. We present a brief overview of these algo-rithmsinthispaper.Wealsoidentifyopenissueswhichneedtobeaddressed. 
KeywordsScheduling•Provisioning•Publictransport•IoT 
 
1 Introduction 
 
Withanincreaseinpopulation,thedemandforpublictransportservicealsoincreases. This situation pushes the public transport infrastructure to its limits inpeakhours.Thishasleadtothelatearrivalsofpublictransportattheirscheduled 
 
 
D.Patel(&)Z.Narmawala  S.Tanwar• 	• 	 
DepartmentofCE,InstituteofTechnology,NirmaUniversity,Ahmedabad,Gujarat,Indiaemail:15mcen18@nirmauni.ac.in 
Z.Narmawala e-mail: zunnun80@gmail.com 
S.Tanwar e-mail:sudeep149@rediffmail.com 
P.K.Singh 
DepartmentofCSE,JaypeeUniversityofInformationTechnology, 
Waknaghat, Himachal Pradesh, Indiaemail:pradeep_84cs@yahoo.com 
©SpringerNatureSingaporePteLtd.2019 	39 
B.K.Panigrahietal.(eds.),SmartInnovationsinCommunicationandComputational Sciences,AdvancesinIntelligentSystemsandComputing670,https://doi.org/10.10
07/978-981-10-8971-8_4 stops, inefficient use of resources, and a decrease in operating cost. And again thissituation leads to switching of other modes of transportation by people which isundesirable.ThetraditionalschedulingoperationinIndiaisnotefficientforlarge-scale running routes [1]; i.e., public transport still lags behind in India. Theintelligentpublictransportationschedulingbecomesthemainresearcharea.Hence, by using the emerging technologies, public transportation can be scheduled in anoptimized way to meet the public demand. Hence, to provide the better transportationservices,theschedulingalgorithmshavebeenproposedwhichfocusesonthe many factors such as a number of passengers, the capacity of buses, waitingtimeofpassengers, arrivaltime,anddeparturetime.Thebestschedulingalgorithmis one which leads to the decrease in waiting time of passengers while maintainingthe capacity of the passengers in public transport. Hence, IoT is the most emergingtechnologywhichhasbeenusedbypublictransportservices. 
As per the survey of researchers, it has been concluded that all the presentsystems which are based on transportation system provide the service of eitherreservation or displays bus status. In transportation system, it is also important tomaintain the schedule of buses. But due to traffic and many more parameters,schedules get disturbed. Usually, passengers have to wait for the buses because ofbad scheduling, overcrowding, traffic congestion, and breakdowns. Overcrowdingoccurs because of not determining the correct frequency for demand and improperscheduling. Frequency relates to the number of trips which are needed to cope upwith the passenger demand during a peak or fixed period. Hence, it is important tohave exact traffic information to notify the exact arrival and departure timings ofbuses. This information can be available by using GPS [2]. Along with these, it isalso important to schedule buses according to the requirements of the public. Thesolution is to develop efficient scheduling algorithm which can schedule the busesautomaticallybyanalyzingthehistoricaldata. 
There are many scheduling algorithms available such as priority, round robin,firstcomefirstserve,lastcomefirstserve,andmuchmore.Butthesealgorithmsared eveloped for operating systems. Algorithms like genetic algorithm [3], greedyrandomizedadaptivesearchprocedure(GRASP)[4],tripfrequencyscheduling,a ndvehicle routing problem are such scheduling algorithms which either schedule thevehicles or finds proper routes for buses. These algorithms have the drawback interms of a number of jobs or vehicles. There is a need of scheduling 
algorithmwhich can schedule buses as per the requirement of passengers on proper time andproper routes. Some algorithms use heuristics to calculate the parameters 
andschedule it accordingly. But these heuristics require same number of jobs with thesame number of resources. Hence, if we use these algorithms for scheduling 
ofbuses, it will require the same number of buses with the same number of routes. 
Itbecomescompulsorytohavethesamenumberofparameters.Hence,itisnecessaryto develop such algorithm which can even schedule one bus. We can use assign-ment 
problem to assign buses for required route with heuristics to schedule thebuses as per the requirement and reschedule the buses which are not required forthaFigure 1 shows the present scenario of the public transportation system whichuses RFID tags to track the public transport to have live data about the stopscovered by the buses. It also uses GSM/GPRS to notify the passengers about thecurrent status of buses. Servers are used from which data are fetched to notify thepassengers. In more general, this system shows the school bus which is trackedusing RFID tags and GSM/GPRS, and its status is notified to the parents so thattheirwaitingtimeatthestopsdecreaseswaitingunnecessarilyatstops. 
AccordingtothePlanningCommission(2013)[5]survey,ithasbeenconcludedthat there is an increase in traffic of public transport as people refer it much fortraveling. According to the survey, people prefer railways and roadways increas-ingly and it is expected to grow up to 11 percent and 7 percent per year, respec-tively. By this, it is expected that traffic could increase up to 16 factors by next 20years. Since it was about 7 to 8 factors in last 10 years, it is growing very fast.Hence,thisprovestheneedforpublictransportwhichshouldbescheduledaccording to the need. Figure 2 shows an increase in traffic in roadways and railwaysinbillionpassengerkilometer(bpkm). –	Acompletetaxonomyofpublictransport,whichcanbefurtherclassifiedintogenerala ndselectiveapproach,isprovidedusingIoTasatool. 
–	Approachesusedforschedulingpublictransportareanalyzedwithrespecttoparamet ers,suchaspositioning,time. 
–	Finally,asystematiccomparisonofthevariouspublictransportsystemwithprosandc onsofeachisprovidedinthetext. 
 
 
 
1.2 Organization 
 
Rest of the paper is organized as follows. Section 2 presents the similar work doneby various researchers in this domain with tabular comparison of each approach.Section 3 provides the challenges and open research problems in this domain, andfinally,Sect.4concludesthearticlewithfuturescope. 
 
 
2 LiteratureSurvey 
 
This section provides the detailed description of the work done under this domainby 	various 	researchers.Wehavedividedthisdescription intotwocategories:generalized and selective. Next subsection explains each category in detail withprosandconsofeach. 
2.0 GeneralizedApproach 
 
Since last few years, research has been carried out to develop the optimizationmodelswhichwillincreasetheconvenienceofpassengers,andonthebusma nagement side, bus operations are reduced. Depending on the approach fordetermining optimal solutions, the bus scheduling models studied so far can beclassified into a number of types. These models use heuristics to calculate totaltrafficcost. 
Fu et al. [6] proposed a new operating strategy in which service vehicles isfollowed by the lead vehicle with all stop service and also by providing the facilityto skip some stops as an express service. Chen [7] measures bus service reliability,vehicle load capacity, by considering the headway adherence and average waitingtime. Yan proposed a network flow problem using a mathematical model whichuses Lagrangian relaxation. Kim et al. [8] constructed a schedule based on thestarting point and stops by using travel time response model for critical schedulingareas. 
 
 
2.1 SelectiveApproach 
 
Vehicle Routing Problem In vehicle routing problem with time window, a numberofvehiclesareallocatedtorouteandeachwithgivencapacitywhichislocatedatas ingledepotwhichisservingpassengersdispersedgeographically.Inthisproblem,eachp assengerhasbeengiventhedemandandtheymustbeservedinspecifictimewindow. The main objective of this problem is to minimize the total cost of trav-eling while serving the customers with minimum cost. Figure 3 shows the vehiclerouting problem (VRP), and how a route is set up from base depot to each stopreducing the traveling cost. It reduces the path cost by setting the optimized routebetween stops from one station to other from depot. The main objective of VRP isasfollows: 
1.	Itminimizestheglobaltransportationcostbasedonglobaldistance. 
2.	Minimizesthenumberofresourcesneededtoserveallcustomers. 
3.	Variationintraveltimeandvehicleloadisleast. reduced. Depending on the approach fordetermining optimal solutions, the bus scheduling models studied so far can beclassified into a number of types. These models use heuristics to calculate totaltrafficcost. 
Fu et al. [6] proposed a new operating strategy in which service vehicles isfollowed by the lead vehicle with all stop service and also by providing the facilityto skip some stops as an express service. Chen [7] measures bus service reliability,vehicle load capacity, by considering the headway adherence and average waitingtime. Yan proposed a network flow problem using a mathematical model whichuses Lagrangian relaxation. Kim et al. [8] constructed a schedule based on thestarting point and stops by using travel time response model for critical schedulingareas. 
 
 
2.1 SelectiveApproach 
 
Vehicle Routing Problem In vehicle routing problem with time window, a numberofvehiclesareallocatedtorouteandeachwithgivencapacitywhichislocatedatas ingledepotwhichisservingpassengersdispersedgeographically.Inthisproblem,eachp assengerhasbeengiventhedemandandtheymustbeservedinspecifictimewindow. The main objective of this problem is to minimize the total cost of trav-eling while serving the customers with minimum cost. Figure 3 shows the vehiclerouting problem (VRP), and how a route is set up from base depot to each stopreducing the traveling cost. It reduces the path cost by setting the optimized routebetween stops from one station to other from depot. The main objective of VRP isasfollows: 
1.	Itminimizestheglobaltransportationcostbasedonglobaldistance. 
2.	Minimizesthenumberofresourcesneededtoserveallcustomers. 
3.	Variationintraveltimeandvehicleloadisleast. 
OnlineDial-A-
RideProblemwithTimeWindow(DARPTW)Routingandscheduling of buses can be referred as a On-line-Dial-A-Ride problem [7]. It takescare of the available set of resources and constraints. All the services related to thetransportation is Webbased and handled by mobile phones. Here, request is gen-erated one day prior to the beginning of service. Due to a high number of 
variablesinvolvedinit,thesolutionsavailablearebasedonheuristics.IntheOnlineDial-
A-RideProblemwithtimewindows(ODARPTW)[9]requestsareexhibited after some time, requiring the server to convey the articles from sources to destination, while the server is en-route for serving the different request. On the offchance that a demand is to be served, the server must achieve the time between thedemand’s landing and its due date. The objective here is to plan techniques for theserver to fill in whatever number of approaching requests as could reasonably beexpected by their due dates in an on-line way. The system for ODARPTW neitherhas data about the discharge time of the last demand nor has the aggregate numberofrequest.Itmustdecidetheconductoftheserverataspecificminuteoftimeasanel ement of the considerable number of request discharged up to time t (and thepresenttimet).Interestingly,adisconnectedtechniquehasdataaboutallrequestsinthe entiresuccessionasofnowattime0. 
Assignment algorithmis operation research method to optimize the cost. Itdealswiththetransportationproblemandtheassignmentofjobstotheworkersorassign mentofresourcestotheworkers.Theultimateobjectiveishowtoassign the jobs efficiently to the workers, and which worker should be assignedwhich type of job. In this problem, at least 3  3 matrix is required and also thesame number of × parameters. Assignment problem uses heuristics, in which theoperatingcostof the system can be maximized or minimized. If we are addingany constant in each and every element of columns and rows of the matrix, then 
itwillgenerateamatrix,whichcanminimizethetotaleffectiveness.Asituationalso exists, where we need to add a dummy column or a row when there are noexact number of resources, and jobs. The main disadvantage of this algorithm is anumber of jobs must be equal to the number of workers or else allocation of jobswillnotbeefficient. 
The data flow diagram of assignment algorithm is discussed below in Fig. 
4.This diagram shows how assignment algorithm works with its two conditions. Inassignment problem, basically there are two situations: First, when the number ofcutting lines is equal to the number of rows and columns, and second, when thenumberofcuttinglinesisnotequaltothenumberofrowsandcolumns. 
Table 1 represents the summary of the whole survey. In the table, there are fourcolumns. The first column is the name of author, second is the algorithm/methodthey have used for implementation, third is what are the pros of paper, and thefourthoneiswhatcanbeadded/improvedorconsinpaper. ChallengesandOpenResearchProblemsinSchedulingPublicTransport 
 
In existing public transportation systems, passengers need to register compulsoryfortraveling.Schedulingoftransportationserviceislimitedforthelimitedre sources.Schedulingofpublictransportisnotmuchefficientasitrequiresaccuratedata on traffic. Due to this, the waiting time of passengers increases. Passengersusedtotravelinpublictransportmostlyinpeakhours.Therefore,inpeakhours duetononexistenceschedulingmechanism,passengersincreasebeyondthecapacityofp ublic transport. As capacity of public transport increases, the counting of passengers in the existing system is not efficient. Waiting time of passengers increasesat stops in peak hours that is in morning and evening which increases traffic inbuses. Hence, there is a need to develop an efficient and accurate system forschedulingandprovisioningofbusesdynamicallybasedoncurrentdemand. 
Publictransportshouldprovidesafetraveling,cheapfare,andlesstraveltime.Inordert oachievetheseattributes,govtmustfocusonroadnetwork,optimalrouting,and minimum delay. Public transport efficiency depends upon all other relatedfactors, i.e. optimization of route, transfer optimization, and coordination amongfeederbusservice. 
 
 
3 ConclusionandFutureScope 
 
In India, traffic congestion problem is increasing day by day in urban centers. It isbecause of increase in population in urban areas with very high rate, and people preferprivatevehiclesoverpublictransport,astheyneedtowaitforalongamountoftimeto get a bus and often buses are crowded too. Hence, it is important to develop anefficient scheduling and provisioning of public transports so that waiting time oftravelers reduces and everyone gets seat in the bus. Many algorithms have beenproposed by various researchers as discussed in Sect. 2. These proposals do havetheir drawbacks as highlighted in Table 1. We need to improve these algorithms intermsofschedulingandprovisioningofpublictransportforIndianscenario. 
Infuture,wecandevelopasystemwhichcanallowseatreservationinrealtime.Sensors can be used to track seat occupancy and allow reservation for unoccupiedseats. 
 
 
References 
 
1.	K.Shankar, “Applications of advanced technologies to transportation systems in indiancontext,” International Journal of Earth Sciences and Engineering, vol. 4(6), pp. 394– 397,2011. 
2.	T.Halonen, J. Romero, and J. Melero, “Gsm, gprs and edge performance: evolution towards3g/umts,”2004. 
3.	F.A. Kidwai, B. R. Marwah, K. Deb, and M. R. Karim, “A genetic algorithm based busschedulingmodelfortransitnetwork,”vol.5,pp.477–489,2005. researchers as discussed in Sect. 2. These proposals do havetheir drawbacks as highlighted in Table 1. We need to improve these algorithms intermsofschedulingandprovisioningofpublictransportforIndianscenario. 
Infuture,wecandevelopasystemwhichcanallowseatreservationinrealtime.Sensors can be used to track seat occupancy and allow reservation for unoccupiedseats. 
 





 

 


