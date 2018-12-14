Variational Auto-encoders
====

Input:

    2D map of pixels (CNN)
    
    
Combine with high level information
    
    
First test:

    python test.py
    
    
dE/dx application
====

Train on MIP, train to "autoencode"

    python dedx.py  
    
        
Prepare flat tree
====

    ln -s /media/amassiro/SAMSUNG/CernData/dedx/calibration/ Data
    
    
    g++ -o prepareTree.exe prepareTree.cpp `root-config --cflags --glibs`
     
    ./prepareTree.exe     Data/tree_filtered_mc.root    flat_tree_Z.root
    ./prepareTree.exe     Data/tree_filtered_data_calibrated_new_many_eta_regions_30iov.root    flat_tree_data.root
    
    
    
    