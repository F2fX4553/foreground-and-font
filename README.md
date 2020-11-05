# foreground-and-font

def fgall(pos,fg):
    pos.update()
    clt = pos.winfo_children()
    my = ttk.Style()
    my.configure('TButton', foreground=fg)
    my.configure('TRadiobutton', foreground=fg)
    my.configure('TTCheckbutton', foreground=fg)
    for c in clt:
        try:
            c['foreground']= fg
        except:
            pass



def fontall(pos,font):
    pos.update()
    clt = pos.winfo_children()
    my = ttk.Style()
    my.configure('TButton', font=font)
    my.configure('TRadiobutton', font=font)
    my.configure('TCheckbutton', font=font)
    for c in clt:
        try:
            c['font']= font
        except:
            pass
