Lab 5 - Reinforcement Learning
=======================================

.. contents:: :depth: 2

Lecture 5.1: Intro to RL and Its Applications in Robotics
---------------------------------
Intro to RL and Its Applications in Robotics Lecture by Tingnan Zhang, May 3, 2023. 

.. raw:: html


    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://zoom.us/rec/play/fRXFHoFrjlpjt9gVOVWnNRHo8R_rU-iOtRmXF3u8XZ2KgrK8DENzo5SLFn48L2RiJcmcUXKFhwb7Q729.sdVpKRsw8rBYbteF?canPlayFromShare=true&from=share_recording_detail&continueMode=true&iet=wmdFLQ8F3rRme3xcMnqQkcS4WVgXJLlma3JnnwIMf9s.AG.zojk4nPlEHorB-cOnef5NeSTIy_isT_weOI8mg6ZsJFRIYdvDuj8VR7KZNB77MY905pGOC3gGFh8Zu_Ws2BMXjwx5dgF_N3awLjQr9aAbK_IKaTbX9hzJ44lydc.3uEehfVWzpW155ugpy4JJQ.s3GZJ3oN2zvD4zuv&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2F2Rgy4kgC2RPpqFGcQbghGeMx1iotEH1K_TFiCiuSZwgywJSamoBCZl7q4zAQjwQl.WJPRPSJBnX4rzr4B%3Fiet%3DwmdFLQ8F3rRme3xcMnqQkcS4WVgXJLlma3JnnwIMf9s.AG.zojk4nPlEHorB-cOnef5NeSTIy_isT_weOI8mg6ZsJFRIYdvDuj8VR7KZNB77MY905pGOC3gGFh8Zu_Ws2BMXjwx5dgF_N3awLjQr9aAbK_IKaTbX9hzJ44lydc.3uEehfVWzpW155ugpy4JJQ.s3GZJ3oN2zvD4zuv" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

|

Lecture 5.2: Reinforcement Learning on Legged Robots
---------------------------------
Reinforcement learning on legged robots lecture by Jie Tan, May 10, 2023. 

.. raw:: html


    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://zoom.us/rec/play/0vMKffsjh5Bi4exwZ6CIAhuAQP3WuDW2zIJj5z0FDS8uAUXxsElks7eXIP9mEYAEzFH8wxu551NcRNuv.pOZ47OLJt09Z9TjB?canPlayFromShare=true&from=share_recording_detail&continueMode=true&iet=pZx1gb2D_2ZMpQ4cOj19S3S88rmBjWA3oPhFoO-flSk.AG.D_nTZ0dyKvgJLLKvlTdSB0X9u8E8wzExKAa6NvelKeblzJ6_TMEvdtL9FXV9lR-kqp_XDlW4k5XnZkyHg0uiV_Lm2AridUiBefMeAQq8KwzJz7ykxbhXfr99lRY.Mk_5ok_9KyI4g85Frp-56Q.rdEK4pPXqGABoqlQ&componentName=rec-play&originRequestUrl=https%3A%2F%2Fzoom.us%2Frec%2Fshare%2FxD3jWNSXqgGLc-bHv_wbilELP5ZVCCreLV7Hyg10wk6u5TVa7X_2qjLadxPIwdFR.Rwn4C-0Fu1KEVLf9%3Fiet%3DpZx1gb2D_2ZMpQ4cOj19S3S88rmBjWA3oPhFoO-flSk.AG.D_nTZ0dyKvgJLLKvlTdSB0X9u8E8wzExKAa6NvelKeblzJ6_TMEvdtL9FXV9lR-kqp_XDlW4k5XnZkyHg0uiV_Lm2AridUiBefMeAQq8KwzJz7ykxbhXfr99lRY.Mk_5ok_9KyI4g85Frp-56Q.rdEK4pPXqGABoqlQ" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

|

Lecture 5.3: Embodied Intelligence
---------------------------------
Embodied Intelligence lecture by Adrien Gaidon, May 15, 2023.

Zoom password (if prompted): ^dgGqIB5

.. raw:: html


    <div style="position: relative; padding-bottom: 56.25%; height: 0; overflow: hidden; max-width: 100%; height: auto;">
        <iframe src="https://tri-global.zoom.us/rec/play/4ql7Dq8KY_H3fJXGoMNdh43vf7CtC-IDNVQIQUtAZ0rMgVImu9iuoncfLOnEYqwWNEacxgDVnD2nEppS.6E_fFY1yKz-djrzq?canPlayFromShare=true&from=share_recording_detail&continueMode=true&componentName=rec-play&originRequestUrl=https%3A%2F%2Ftri-global.zoom.us%2Frec%2Fshare%2FqrW7_T9WGtCS6Jm5L1Hkj8j4bmWmhExtsMbXf_gleMvp7XxjfChKZcS4tlzkfC8u.Zem3cLxjybJG2B6h" frameborder="0" allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe>
    </div>

|

Lab instructions
-------------------

These instructions assume you are running Mac or Linux. If you have Windows 10 or lower, I recommend dual-booting linux. If you have Windows 11, try using the Windows Linux Subsystem. Otherwise proceed at your own risk!

Step 1. Set up simulation environment
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Clone the simulator repository ``git clone https://github.com/jietan/puppersim.git``
#. Follow the instructions in the `System setup <https://github.com/jietan/puppersim#system-setup/>`_ and `Getting the code ready <https://github.com/jietan/puppersim#getting-the-code-ready/>`_ sections of the Puppersim README.md.

Step 2. Train the policy using RL (ARS)
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Follow instructions at https://github.com/Nate711/puppersim/blob/main/puppersim/reacher/README.md to run the commands to train the policy.
#. Wait about 50 iterations until going to step 3 but leave it training

Step 3. Run your policy in simulator
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Follow instructions at https://github.com/Nate711/puppersim/blob/main/puppersim/reacher/README.md to run the policy.

Step 4. Deploy policy to robot
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
#. Follow instructions at https://github.com/Nate711/puppersim/blob/main/puppersim/reacher/README.md to deploy to your robot.

Step 5. One day project of your choice
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Do your own mini project!

Some ideas:

* Teach the robot to trace out a specific shape in the air. (medium)
* Teach the robot to turn itself off by pressing its power button. (medium)
* Add a cube in the pybullet simulation and teach the robot to kick it. (hard)
* Turn off torque on the elbow or shoulder motor and make the robot learn to balance the arm vertically. (hard)

|

(Old) RL Lecture
---------------------------------

https://share.icloud.com/photos/0836FiHhLJuCXCs9TyqSW8Ilw

.. raw:: html

    <iframe src="https://docs.google.com/presentation/d/e/2PACX-1vSOdXk8Tz55ZzrXGzIeHZUEigYQPUS2bPOIQPeFiRIXSRrVX7hqwXnC1yJnaZoH-uvJZ0OnK4JAW14o/embed?start=false&loop=false&delayms=60000" frameborder="0" width="600" height="400" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>
