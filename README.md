# FindOrgs
EmployStat = as.character(readline(prompt = "Enter EmployStat (salaried, hourly, or other): "));


CalcAnnBonus = function(inEmployStat)
{
  if(inEmployStat == "salaried")
  { 
    AnnBonusOut = 5000.00;
  } else if(inEmployStat == "hourly")
  { 
    AnnBonusOut = 2500.00;
  } else
  { 
    AnnBonusOut = 1250.00;
  }
  return(AnnBonusOut);
}

AnnBonus = CalcAnnBonus(EmployStat) # function call
print(sprintf("The EmployStat is %-6s", EmployStat));
print(sprintf("The AnnBonus is %-6.2f", AnnBonus));
