# QA-DSA---12--Duplicate_numberof_same_array_count

function DuplicateNumberinSameArray(Arr) {
    let xPointer = 0
    for (let i = 0; i < Arr.length; i++) {
        if (Arr[i] > Arr[xPointer]) {
            xPointer += 1
            Arr[xPointer] = Arr[i]
        }
    }
    return (xPointer + 1)
}

console.log(DuplicateNumberinSameArray([0, 0, 1, 1, 1, 2, 2, 3, 3, 4]))
