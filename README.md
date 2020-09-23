# PatchRNNExtra

    '''
        PatchRNNExtra: RNN-based Security Patch Identification with Oversampling Samples.
        Developer: Shu Wang
        Date: 2020-09-23
        Version: S2020.09.23-V4-Extra
        Description: patch identification using both commit messages and normalized diff code
                     with extra oversampling samples.
        File Structure:
        PatchRNNExtra
            |-- data                                    # data storage.
                    |-- negatives                           # negative samples.
                    |-- positives                           # positive samples.
                    |-- security_patch                      # positive samples. (official)
            |-- synthesis                               # synthetic data storage.
                    |-- negatives                           # negative samples. (synthetic)
                    |-- positives                           # positive samples. (synthetic)
                    |-- security_patch                      # positive samples. (synthetic)
            |-- temp                                    # temporary stored variables.
                    |-- data.npy                            # raw data. (important)
                    |-- props.npy                           # properties of diff code. (important)
                    |-- msgs.npy                            # commit messages. (important)
                    |-- ...                                 # other temporary files. (trivial)
            |-- PatchRNNExtra.py                        # main entrance. (Local)
        Usage:
            python PatchRNNExtra.py
        Dependencies:
            clang >= 6.0.0.2
            torch >= 1.2.0+cu92
            nltk  >= 3.3
    '''
