package com.randomgenerator.Sumit1334;


import com.google.appinventor.components.annotations.*;
import com.google.appinventor.components.runtime.*;
import com.google.appinventor.components.common.ComponentCategory;
import com.google.appinventor.components.runtime.errors.YailRuntimeError;

import java.util.Locale;
import java.util.Random;


@DesignerComponent(version = 1,  description = "This extension is created bt Sumit kumar for generating string with your desired length.<br>" +
                   "Kodular Profile<br><a href='https://community.kodular.io/u/sumit1334' target='_blank'>https://community.kodular.io/u/sumit1334</a><br>",
        category = ComponentCategory.EXTENSION,
        nonVisible = true,   iconName = "https://community.kodular.io/user_avatar/community.kodular.io/sumit1334/120/82654_2.png")
@SimpleObject(external = true)
public class RandomGenerator extends AndroidNonvisibleComponent {
    private ComponentContainer container;
    public RandomGenerator(ComponentContainer container) {
        super(container.$form());
        this.container = container;
    }
    private String[] s = "a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,v,w,x,y,z".split(",");
    private String[] intst = "a,b,c,d,e,f,g,h,i,j,k,l,m,n,o,p,q,r,s,t,u,v,w,x,y,z,A,B,C,D,E,F,G,H,I,J,K,L,M,N,O,P,Q,R,S,T,U,V,W,X,Y,Z,1,2,3,4,5,6,7,8,9,0".split(",");

    @SimpleFunction(description = "Generate random string for given length")
    public String LowerCase(int length){
        if (length<1)
            throw new YailRuntimeError("length cant be 0","length error");
        else {
            String retur = "";
            for (int i=0;i<length;i++){
                Random r = new Random();
                retur=retur+s[r.nextInt(26)];
            }
            return retur;
        }

    }
    @SimpleFunction(description = "Generate random string Uppercase")
    public String UpperCase(int length){
        if (length<1)
            throw new YailRuntimeError("length cant be 0","length error");
        else {
            String retur = "";
            for (int i =0;i<length;i++){
                Random r = new Random();
                retur=retur+s[r.nextInt(26)];

            }
            return retur.toUpperCase(Locale.ROOT);
        }

    }
    @SimpleFunction(description = "Generate random Integer for given length")
    public String Integer(int length){
        if (length<1)
            throw new YailRuntimeError("length cant be 0","length error");
        else {
            String retur = "";

            for (int i=0;i<length;i++){
                Random r = new Random();
                retur=retur+r.nextInt(9);
            }
            return retur;
        }

    }
    @SimpleFunction(description = "Generate random string with integer include for given length")
    public String String(int length){
        if (length<1)
            throw new YailRuntimeError("length cant be 0","length error");
        else {
            String retur = "";

            for (int i=0;i<length;i++){
                Random r = new Random();
                retur=retur+intst[r.nextInt(intst.length)];
            }
            return retur;
        }

    }

 }
