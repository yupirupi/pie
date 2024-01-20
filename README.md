def func(list1):
    t = len(list1)
    k = t - 1
    sum1 = 0 
    while k > -1:
        sum1= list1[k] + sum1
        k = k - 1
    return 'всего огоньков - ',sum1
list1 = [8,9,5,4,3,2]
result = func(list1)
print(result ) 
server_addres = ('', 80) 

httpd = HTTPServer(server_addres, CGIHTTPRequestHandler)

print('start')
httpd.serve_forever()
print('stop')