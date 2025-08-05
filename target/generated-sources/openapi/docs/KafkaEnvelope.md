

# KafkaEnvelope

## oneOf schemas
* [ApplicationAudit](ApplicationAudit.md)
* [CamundaAudit](CamundaAudit.md)
* [InstanceDlq](InstanceDlq.md)
* [IpeAudit](IpeAudit.md)
* [TaskDlq](TaskDlq.md)

## Example
```java
// Import classes:
import com.example.kafka.model.KafkaEnvelope;
import com.example.kafka.model.ApplicationAudit;
import com.example.kafka.model.CamundaAudit;
import com.example.kafka.model.InstanceDlq;
import com.example.kafka.model.IpeAudit;
import com.example.kafka.model.TaskDlq;

public class Example {
    public static void main(String[] args) {
        KafkaEnvelope exampleKafkaEnvelope = new KafkaEnvelope();

        // create a new ApplicationAudit
        ApplicationAudit exampleApplicationAudit = new ApplicationAudit();
        // set KafkaEnvelope to ApplicationAudit
        exampleKafkaEnvelope.setActualInstance(exampleApplicationAudit);
        // to get back the ApplicationAudit set earlier
        ApplicationAudit testApplicationAudit = (ApplicationAudit) exampleKafkaEnvelope.getActualInstance();

        // create a new CamundaAudit
        CamundaAudit exampleCamundaAudit = new CamundaAudit();
        // set KafkaEnvelope to CamundaAudit
        exampleKafkaEnvelope.setActualInstance(exampleCamundaAudit);
        // to get back the CamundaAudit set earlier
        CamundaAudit testCamundaAudit = (CamundaAudit) exampleKafkaEnvelope.getActualInstance();

        // create a new InstanceDlq
        InstanceDlq exampleInstanceDlq = new InstanceDlq();
        // set KafkaEnvelope to InstanceDlq
        exampleKafkaEnvelope.setActualInstance(exampleInstanceDlq);
        // to get back the InstanceDlq set earlier
        InstanceDlq testInstanceDlq = (InstanceDlq) exampleKafkaEnvelope.getActualInstance();

        // create a new IpeAudit
        IpeAudit exampleIpeAudit = new IpeAudit();
        // set KafkaEnvelope to IpeAudit
        exampleKafkaEnvelope.setActualInstance(exampleIpeAudit);
        // to get back the IpeAudit set earlier
        IpeAudit testIpeAudit = (IpeAudit) exampleKafkaEnvelope.getActualInstance();

        // create a new TaskDlq
        TaskDlq exampleTaskDlq = new TaskDlq();
        // set KafkaEnvelope to TaskDlq
        exampleKafkaEnvelope.setActualInstance(exampleTaskDlq);
        // to get back the TaskDlq set earlier
        TaskDlq testTaskDlq = (TaskDlq) exampleKafkaEnvelope.getActualInstance();
    }
}
```


