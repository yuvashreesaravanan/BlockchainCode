# BlockchainCode
pragma solidity 0.4.18 <= 0.6.12;

contract HealthCare{

 string Name;
 string addrs;
 string DocName;
 string ReasonForVisit;
 string    DateOfVisit;
 string PatientId;
 int    AmoountPaid;

 function HealthCare(string nName, string nAddrs, string nDocName, string nVisit, string nDate, string nPatientId, int nAmnt) public{
 
   Name = nName;
   addrs = nAddrs;
   DocName = nDocName;
  ReasonForVisit = nVisit;
  DateOfVisit = nDate;
  PatientId = nPatientId;
  AmoountPaid=nAmnt;

 }

   function getHealthCares() public view returns(string,string,string,string,string,string,int) {
 
     return(Name, addrs, DocName, ReasonForVisit, DateOfVisit, PatientId, AmoountPaid);

   }
    

}
