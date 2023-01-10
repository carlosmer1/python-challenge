# python-challenge



open(file_to_load) as financial data:
    reader = csv.reader (financial_data)
    
    header = next(reader)
    
    first_row = next(reader)
    total_months = total_months + 1
    total_net = total_net + int(first_row[1])
    prev-net = int(first_row[1])
    
    for row in reader:
       
    #track total
        total_months = total-months + 1
        total_net = total_net + int(row[1])
        
        #track net change
        net_change = int(row[1]) - prev_net
        prev_net = int(row[1])
        net_change_list = net_change_list + [net_change]
        month_of_change = month_of_change + [row[0]]
        
        #greatest increase
        if net_change > greatest_increase[1]:
            greatest_increase[0] = row[0]
            greatest_increase[1] = net_change
            
            #greatest decrease
            if net_change < greatest_decrease[1]:
                greatest_decrease[0] = row[0]
                greatest_decrease[1] = net_change
                
                run
