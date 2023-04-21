Select p.Name as ProductName, 
	   c.Name as CategoryName
from Product p
join ProductCategory pc on pc.ProductId = p.Id
join Category c on pc.CategoryId = c.Idw
order by p.Name, c.Name