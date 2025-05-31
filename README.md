public class HospitalReport {

    public static void main(String[] args) {
        // Array of patient visit types
        String[] patientVisits = {"Emergency", "Outpatient", "Inpatient", "Outpatient", "Emergency"};

        for (int i = 0; i < patientVisits.length; i++) {
            String visitType = patientVisits[i];

            switch (visitType) {
                case "Emergency":
                    System.out.println("Visit " + (i + 1) + ": Immediate care required.");
                    break;
                case "Outpatient":
                    System.out.println("Visit " + (i + 1) + ": Routine check-up scheduled.");
                    break;
                case "Inpatient":
                    System.out.println("Visit " + (i + 1) + ": Patient admitted to ward.");
                    break;
                default:
                    System.out.println("Visit " + (i + 1) + ": Unknown visit type.");
                    break;
            }
        }
    }
}
