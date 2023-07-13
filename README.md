function insertionSort(arr) {
    for (let i = 1; i < arr.length; i++) {
        const current = arr[i];
        let j = i - 1;
        while (j >= 0 && arr[j] > current) {
            arr[j + 1] = arr[j];
            j--;
        }
        arr[j + 1] = current;
    }
    return arr;
}

const arr = [5, 2, 4, 6, 1, 3];
console.log(`Unsorted array: ${arr}`);
console.log(`Sorted array: ${insertionSort(arr)}`);


The code above defines a function called insertionSort that takes an array as input and returns the sorted array using the insertion sort algorithm. The function iterates over each element in the array starting from the second element. For each element, it compares it with the previous elements in the array and inserts it into the correct position in the sorted sequence. Finally, it returns the sorted array.