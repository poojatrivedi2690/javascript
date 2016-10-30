function insertionSort(array)
{
    for(var i = 1; i < array.length; ++i)
    {
        var currentItem = array[i];

        for(var j = i - 1; j >= 0; --j)
        {
            if(array[j] <= currentItem) break;
            array[j + 1] = array[j];
        }

        array[j + 1] = currentItem;
    }

    return array;
}
insertionSort([7,5,2,4,3,9]); 