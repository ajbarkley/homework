# homework
def main():
    #get rainfall from user
    rainfall = get_rainfall()

    #get the total of rainfall
    total = get_total(rainfall)

    #get the lowest amount of rainfall
    lowest = min(rainfall)
#       **OUTPUT WILL NEED TO READ MONTH W/ LOWEST TOTAL**

    #get the highest amount of rainfall
    highest = max(rainfall)
#       **OUTPUT WILL NEED TO READ MONTH W/ HIGHEST TOTAL**

    #get the average amount of rainfall
    average = total / len(rainfall)

    #print results
    print('The total rainfall in inches was: ' , total)
    print('The lowest rainfall in inches was: ' , lowest)
    print('The highest rainfall in inches was: ' , highest)
    print('The average rainfall in inches was: ' , average)

#get rainfall amounts from user per month
def get_rainfall():
    #get rainfall input from user and apply to list of months
    #create month list
    month = ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun', 'Jul',
            'Aug', 'Sep', 'Oct', 'Nov', 'Dec',]

    #"for" or "while" input loop **THIS IS WHERE IM CURRENTLY STUCK**
    index = 0
    while index < len(month):
        input('What was the rainfall anount in ', month + '?:')

    #return data
    return get_rainfall

def get_total(rainfall):

    #create accumulator
    total = 0
    #calcuate amounts
    for num in rainfall:
        total += num

    #return total
    return total

#call main
main()
