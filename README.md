# cs3353-lab-quiz-solved
**TO GET THIS SOLUTION VISIT:** [CS3353 Lab Quiz Solved](https://www.ankitcodinghub.com/product/cs335-ai-ml-theory-cs337-3/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;124293&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS3353 Lab Quiz Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
Instructions

1. It is an OPEN BOOK and OPEN INTERNET examination.

4. Be sure to follow the upload instructions.

5. Total time for the examination is 2 hours 30 minutes.

6. This is an open-ended assignment. You are free to use any API from the following libraries to solve the problems: pytorch, numpy, scipy, matplotlib, time.

1. Multi-Task Learning For this problem, we are given with a dataset of

N = 469 samples where each training feature x ∈Rd with d = 28 features. Notice that unlike the problems explored in lab so far, this problem involves two target variables y1 ∈{0,1} and y2 ∈R. The first task corresponding to y1 is a simple binary classification task and the second task corresponding to y2 involves a univariate regression. You are expected to build a multi-task learning (MTL) model that aims to solve both the tasks by exploiting the similarity between them. Towards this end, you will build a machine learning model that has an embedding network ϕ : Rd →Rk where k is the embedding dimension. ϕ is shared across both the tasks. From ϕ, there are two task-specific network heads η1 : Rk → {0,1} and η2 : Rk → R that emits the output. You will design a loss function of the form L1 + λL2 where λ ∈ R is a hyperparameter that trades-off between the losses corresponding to both these tasks.

Note: You will not receive any credit if you solve these tasks using two independent models.

You can train a model of your choice.You need to complete the function predict labels(model, X) that takes in 2 arguments. model is the trained machine learning model and X ∈Rn×d are the test features for which we make predictions. This function returns two vectors y1, y2 of shape Rn where y1 is the class predictions and y2 is the regression predictions.

The following will be checked for evaluation:

1.b The dumped model pickle will be checked to ensure that the task has been solved using a single model.

1.c We will use the predict labels function, along with the trained model pickle and the test dataset, to ensure consistency with the dumped predictions y1 pred and y2 pred.

c /6+6

2. This is a simple problem where you are expected to complete the code for computing the test metrics that are usually used to evaluate classification and regression tasks. Each of these functions receive two arguments namely preds, targets where preds∈Rn is a vector consisting of predictions and targets ∈Rn is a vector consisting of the ground-truth. These functions should return a single scalar as output.

• accuracy

• precision

• recall

• f1 score

• mean squared error

• mean absolute error

c /6

c /2

3. It is a common practice to split the training dataset into train and validation splits and use the validation dataset to tune hyper-parameters. So in this question, you have to write a function that splits the training dataset into train and validation dataset. You need to complete the function train val split(x, y1, y2, train pc) that takes the arguments as training features, classification target, regression target, train pc where train pc ∈ [0,1] represents the percentage of samples to be present in the training dataset. This function should return x trn, y1 trn, y2 trn, x val, y1 val, y2 val.

1 Submission instructions

Complete the functions in assignment.py. Do not modify the function signatures. Keep the file in a folder named &lt;ROLL_NUMBER&gt;_quiz and compress it to a tar file named

&lt;ROLL_NUMBER&gt;_quiz.tar.gz using the command

tar -zcvf &lt;ROLL_NUMBER&gt;_quiz.tar.gz &lt;ROLL_NUMBER&gt;_quiz

Submit the tar file on Moodle. The directory structure should be –

&lt;ROLL_NUMBER&gt;_quiz

| – – – – assignment.py

| – – – – output.pkl

| – – – – model.pkl

Replace ROLL_NUMBER with your own roll number. If your Roll number has alphabets, they should be in “small” letters.

Total: 20
