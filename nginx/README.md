
                                                                                                           /-- nginx pod 1
                                                                                nginx-svc-1:   nginx-dep-1/
                                                                                                          \
       ingress controller                                                                                  \__ nginx pod 2   
       external(10.71.50.224)                          /rule1 /svc-1/(/?)(.*).  backend : nginx-svc-1
       (IP of one of the node)    -----------  Ingress/ 
                                                      \
                                                       \rule2 /svc-2/(/?)(.*).  backend : nginx-svc-2
                        
                                                                                                          /-- nginx pod 3
                                                                               nginx-svc-2:   nginx-dep-2/
                                                                                                         \
                                                                                                          \__ nginx pod 4
                                                                                                          
                                                                                                                 
      
