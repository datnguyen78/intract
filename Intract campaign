function clickTasksAndVerify() {
    // Select all elements with a specific class name (task elements)
    const tasks = document.querySelectorAll('._one_time_task_container_baselink_1ejbz_1');

    // If no task elements are found, log a message and exit
    if (tasks.length === 0) {
        console.log('No task elements found.');
        return;
    }

    // Iterate through each task element
    tasks.forEach((task, index) => {
        // Add event listeners to handle click and prevent default behavior
        task.addEventListener('click', (event) => {
            event.stopPropagation();
            event.preventDefault();
        }, true);

        // Click the task element
        task.click();
        console.log('Clicked on task element ' + (index + 1));
    });

    // Log the number of tasks clicked
    console.log('Clicked on ' + tasks.length + ' task element(s) in total.');

    // Set a timeout to perform the next action after a short delay
    setTimeout(() => {
        // Select all verify buttons with a specific data attribute
        const verifyButtons = document.querySelectorAll('button[data-verify-button-status="idle"]._container_byz4l_1');

        // If no verify buttons are found, log a message and exit
        if (verifyButtons.length === 0) {
            console.log('No verify buttons found.');
            return;
        }

        // Iterate through each verify button
        verifyButtons.forEach((button, index) => {
            // Click the verify button
            button.click();
            console.log('Clicked on verify button ' + (index + 1));
        });

        // Log the number of verify buttons clicked
        console.log('Clicked on ' + verifyButtons.length + ' verify button(s) in total.');
    }, 8000); // 8000 milliseconds delay (8 seconds)
}

// Call the function
clickTasksAndVerify();
