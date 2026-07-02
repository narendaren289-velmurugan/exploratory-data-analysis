import java.util.Arrays;

public class EDAProject {
    public static void main(String[] args) {

        int[] marks = {65, 78, 82, 90, 55, 70, 88, 95, 60, 75};

        int sum = 0;
        int max = marks[0];
        int min = marks[0];

        for (int mark : marks) {
            sum += mark;

            if (mark > max)
                max = mark;

            if (mark < min)
                min = mark;
        }

        double average = (double) sum / marks.length;

        Arrays.sort(marks);

        double median;
        if (marks.length % 2 == 0) {
            median = (marks[marks.length / 2 - 1] + marks[marks.length / 2]) / 2.0;
        } else {
            median = marks[marks.length / 2];
        }

        System.out.println("Exploratory Data Analysis (EDA)");
        System.out.println("-------------------------------");
        System.out.println("Marks: " + Arrays.toString(marks));
        System.out.println("Total = " + sum);
        System.out.println("Average = " + average);
        System.out.println("Maximum = " + max);
        System.out.println("Minimum = " + min);
        System.out.println("Median = " + median);
    }
}# exploratory-data-analysis
here is the model for exploratory 
