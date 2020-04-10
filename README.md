dat_teey=[]
mj=dat_teey
for q in range(0,9):
    mj.append(n[z[q]])
    dat_state = []
    dat_death= []
    dat_rate = [] 
    dat_statea=[]
    dat_deatha=[]
    dat_ratea=[]
    a=dat_state
    b=dat_death
    c=dat_rate
    for i in range(dat.shape[0]):
        if dat.iloc[i,1] == n[q]:
            a.append(dat.iloc[i, 3])
            b.append(dat.iloc[i,4])
            c.append(dat.iloc[i,4]/dat.iloc[i,3])
    plt.plot(a)
    plt.ylabel('Test Postive Cases ')
plt.legend(mj)
plt.show()
