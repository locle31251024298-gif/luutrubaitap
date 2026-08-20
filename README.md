using System;

public class Student
{
    private string name;
    private double score;
    private static int totalStudents = 0;

    public Student(string name, double score)
    {
        this.name = name;
        this.score = score;
        totalStudents++;
    }

    // TODO: write instance methods here

    public string GetName()
    {
        return name;
    } 

    public double GetScore ()
    {
        return score;
    }
    public bool  IsPassed()
    {
        return score >= 5.0; 
    }
    // score >= 6.5 → "Good"
    // score >= 5.0 → "Average"

    public string GetClassification()
    {
        if (score >= 8.0) return "Excellent";
        if (score >= 6.5) return "Good";
        if (score >= 5.0) return "Average";
        return "Weak";

    }


    // TODO: write static methods here






