//  # Income-Calc
//  A calculator that will average out your annual income based off your weekly or bi-weekly checks 


System.out.println(" do you make weekly or bi-weekly checks? enter 'weekly' or 'biweekly' ");
        Scanner inputFromSystem = new Scanner(System.in);
        String biWeeklyOrWeeklyCheck = inputFromSystem.nextLine();



        if (biWeeklyOrWeeklyCheck.equals ("biweekly")  ){

             System.out.println(" enter your average check for every two weeks (within 1 month): ");
             Scanner inputFromSystem2 = new Scanner(System.in);
             int biWeeklyCheck = inputFromSystem2.nextInt();

             int biTotalForOneMonth = biWeeklyCheck * 2;
             int biAnnualIncome = biTotalForOneMonth * 12;

             System.out.println(" This is your monthly income: $"+biTotalForOneMonth);
             System.out.println(" This is your annual income (monthly income * 12 months): $"+biAnnualIncome);
        }



        else if (biWeeklyOrWeeklyCheck.equals ("weekly") ){

             System.out.println(" enter your average weekly check ");
             Scanner inputFromSystem3 = new Scanner(System.in);
             int weeklyCheck = inputFromSystem3.nextInt();

             int TotalForOneMonth = weeklyCheck * 4;
             int AnnualIncome = TotalForOneMonth * 12;

             System.out.println(" This is your monthly income: $"+TotalForOneMonth);
             System.out.println(" This is your annual income (monthly income * 12 months): $"+AnnualIncome);
        }



        else {

             System.out.println(" invalid input try again ");
        }
