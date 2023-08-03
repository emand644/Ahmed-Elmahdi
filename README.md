# Ahmed-Elmahdi
Deviation Calculator
 
def calculate(digits):
# the private function or the unchangable data
    if len(digits)!=9:
    #the digits should not be more thean 9
        raise Error("list should contain 9 digits")
        matrix=np.array(digits).reshape(3,3)
        returned_dictionary={
            
            'mean': [list(matrix.mean(axis=1)), list(matrix.mean(axis=0)), matrix.mean().tolist()],
         'variance': [list(matrix.var(axis=1)), list(matrix.var(axis=0)), matrix.var().tolist()],
         'standard deviation': [list(matrix.std(axis=1)), list(matrix.std(axis=0)), matrix.std().tolist()],
         'max': [list(matrix.max(axis=1)), list(matrix.max(axis=0)), matrix.max().tolist()],
         'min': [list(matrix.min(axis=1)), list(matrix.min(axis=0)), matrix.min().tolist()],
         'sum': [list(matrix.sum(axis=1)), list(matrix.sum(axis=0)), matrix.sum().tolist()]
        } 
        return returned_dictionary
returned_dictionary = calculate([0, 1, 2, 3, 4, 5, 6, 7, 8])
print(result)
        
