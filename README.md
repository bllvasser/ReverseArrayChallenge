# ReverseArrayChallenge
package com.company;

import java.lang.reflect.Array;
import java.util.Arrays;
import java.util.Collections;

public class Main {

    public static void main(String[] args) {

        int[] anotherArray = new int[]{1,2,3,4,5};

        reverse(anotherArray);
        otherForward(anotherArray);

    }

    private static void otherForward(int[] array){

        int[] copiedArray = new int[]{};
        Arrays.sort(copiedArray);

        for(int i = 0; i < array.length; i++) {
            System.out.println("Copied Array " + array[i]);
        }
    }


    private static Integer [] reverse(int[] test){
        Integer array[] = {2,1,4,5,3};
        Arrays.sort(array, Collections.reverseOrder());
        for(int i = 0; i < array.length; i++) {
            System.out.println(array[i]);

        }
        return array;
    }
}
/Library/Java/JavaVirtualMachines/amazon-corretto-11.jdk/Contents/Home/bin/java "-javaagent:/Applications/IntelliJ IDEA CE.app/Contents/lib/idea_rt.jar=63280:/Applications/IntelliJ IDEA CE.app/Contents/bin" -Dfile.encoding=UTF-8 -classpath /Users/Bilaal/IdeaProjects/ReverseArrayChallenge/out/production/ReverseArrayChallenge com.company.Main
5
4
3
2
1
Copied Array 1
Copied Array 2
Copied Array 3
Copied Array 4
Copied Array 5

Process finished with exit code 0
