For the pickle files containing the instances we use pandas to open the files:
Here is a simple function implementation for opening the files.


    def ReadInstanceCFP(InstanciaFile):
        
        Data = pd.read_pickle(InstanciaFile)
    
        I = Data['I'].iloc[0]
    
        J = Data['J'].iloc[0]
    
        Ij = Data['Ij'].iloc[0]
    
        w = Data['w'].iloc[0]
    
        distanciaspc = Data['distanciaspc'].iloc[0]
    
        distanciasp = Data['distanciasp'].iloc[0]
    
        c = Data['c'].iloc[0]
    
        p = Data['p'].iloc[0]
    
        return I, J, Ij, w, distanciaspc, distanciasp, c, p

