# Q3
Birden fazla stack'i bir array'e yerleştirmenin yolu;
1. Array'i içine yerleştirilmek istenen stack sayısına göre parçalara ayırarak başlamaktır. 
  örneğin: 3 stack için  
  1. Bölge = arr[0] to arr[(n/k)-1] , 2. Bölge = arr[n/k] to arr[(2n/k)-1] , 3. Bölge = arr[2n/k] to arr[n-1]
2. Sonrasında her bir stack'ten alınan öğeler o stack için ayrılmış bölgeye sırasıyla yerleştirilir.

 Bu işlemler sırasında karşılaşılabilecek en önemli problem arrayde yetersiz alanla karşılaşılmasıdır. Array içerisine eklenme sırasında stack kendi alanını aşabilir.
 Ayrıca arrayin en sonundaki kısmı kullanan stack array boyutunu aşıcak sayıda elemana sahip olabilir. Bu durumda sistem out of index hatası vericektir.
