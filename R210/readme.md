                Rev210.  Revised the following parts to enable Erasing of UserIDs when completing Write operation.
                The Erase operation does not erase the UserIDs this is the same as previous versions of the software.
                Credit to Bill Roth on his ground to create the ASM.

                PIC18F26K80
                PIC18F25K80
                PIC18F45K80
                PIC18F65K80
                PIC18F46K80
                PIC18F66K80
                PIC18LF26K80
                PIC18LF45K80
                PIC18LF65K80
                PIC18LF66K80
                PIC18LF25K80
                PIC18LF46K80
                PIC18F65K90
                PIC18F87K22
                PIC18F66K22
                PIC18F65K22
                PIC18F85K22
                PIC18F86K22
                PIC18F67K22
                PIC18F67K90
                PIC18F85K90
                PIC18F86K90
                PIC18F87K90
                PIC18F66K90

                When used in association with the PICKitPlus GUI software there two new ini file entries as follows:

                  4.61.0.50
                        Added new ini entries to support UserID management
                        SUIV: N
                        DUIE: N

                        Added new ini to support family 19 UserID management
                        DUIE: N

                        DisableUserIdErase.  This parameter can be Y or N.  When Y this will enable erasure of UserIDs ONLY during Write operations.
                        When N this will not erase the UserIds.  This is therefore will force the same operation as prior versions of the applications.

                        Added new ini support UserID management
                        SUIV: N

                        StopUserIdVerification.  This parameter can be Y or N.  When Y the UserIDs will not be verified.

              PICKitPlus GUIs when used with the 2.63.210 parts database or greater will now erase UserIDs on Write Operations.
              To completely erase a part complete the following.
                1. Ensure Programmer/Clear Memory Buffer on Erase is selected.
                2. Select `Erase` to erase the part. This will also clear the application buffers.  The UserIDs will be shown as the default values.
                3. Seletct `Write` to write to the part. This will write the default values.
                The part is now Erased
