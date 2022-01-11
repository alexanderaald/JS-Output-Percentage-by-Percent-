# JS-Output-Percentage-by-Percent-


 var arrayShuffle = function(array) {
        for ( var i = 0, length = array.length, swap = 0, temp = ''; i < length; i++ ) {
            swap        = Math.floor(Math.random() * (i + 1));
            temp        = array[swap];
            array[swap] = array[i];
            array[i]    = temp;
        }
        return array;
        };

        var percentageChance = function(values, chances) {
        for ( var i = 0, pool = []; i < chances.length; i++ ) {
            for ( var i2 = 0; i2 < chances[i]; i2++ ) {
                pool.push(i);
            }
        }
        return values[arrayShuffle(pool)['0']];
        };

        for ( var i = 0; i < 1; i++ ) {
        console.log(percentageChance(['hi', 'test', 'bye'], [90, 5, 5]));
        }
