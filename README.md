# Create-Acontact-which-are-equal-to-the-NUmber-Of-CONTATt-Size-Field-
Create Acontact which are equal to the NUmber Of CONTATt Size Field 
public class AccounTContactHAndler1
{
  Public Static Void MyInsertConAc(List<Account> AddNewAcc)
  {
      map<id,decimal>Mycount=new map<id,decimal>();
      list<Contact>Fin=new list<Contact>();
        for(Account Acc:AddNewAcc)
        {
            Mycount.put(Acc.id,Acc.My_Contact_SIze__c);
        }
      
      if(Mycount.size()>0 && MyCount != null)
      {
          
          for(id Km:Mycount.keyset())
          {
              for(integer i=1;i<Mycount.get(Km);i++)
              {
                  contact con=new contact();
                      con.AccountId=Km;
                      con.FirstName='MyKm';
                       con.LastName='kms';
                     con.Active__c=true;
                     Fin.add(con);  
              }
              
          }
      }
      if(Fin.size()>0 && Fin!=null)
     insert Fin; 
  }
