# des_block.py implements the DES cryptographic algorithm
# allowing to compute any intermediate value.
# Copyright (C) 2008 Florent Flament (florent.flament@telecom-paristech.fr)
#
# This program is free software: you can redistribute it and/or modify
# it under the terms of the GNU General Public License as published by
# the Free Software Foundation, version 3 of the License.
#
# This program is distributed in the hope that it will be useful,
# but WITHOUT ANY WARRANTY; without even the implied warranty of
# MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
# GNU General Public License for more details.
#
# You should have received a copy of the GNU General Public License
# along with this program.  If not, see <http://www.gnu.org/licenses/>.

# Some DES specific constants
__MSG_SIZE__ = 64  # DES messages are 64 bits long

__IP_PERM__ = (
    57, 49, 41, 33, 25, 17, 9, 1,
    59, 51, 43, 35, 27, 19, 11, 3,
    61, 53, 45, 37, 29, 21, 13, 5,
    63, 55, 47, 39, 31, 23, 15, 7,
    56, 48, 40, 32, 24, 16, 8, 0,
    58, 50, 42, 34, 26, 18, 10, 2,
    60, 52, 44, 36, 28, 20, 12, 4,
    62, 54, 46, 38, 30, 22, 14, 6
)

__E_PERM__ = (
    31, 0, 1, 2, 3, 4,
    3, 4, 5, 6, 7, 8,
    7, 8, 9, 10, 11, 12,
    11, 12, 13, 14, 15, 16,
    15, 16, 17, 18, 19, 20,
    19, 20, 21, 22, 23, 24,
    23, 24, 25, 26, 27, 28,
    27, 28, 29, 30, 31, 0
)

__P_PERM__ = (
    15, 6, 19, 20,
    28, 11, 27, 16,
    0, 14, 22, 25,
    4, 17, 30, 9,
    1, 7, 23, 13,
    31, 26, 2, 8,
    18, 12, 29, 5,
    21, 10, 3, 24
)

__PC1_PERM__ = (
    56, 48, 40, 32, 24, 16, 8,
    0, 57, 49, 41, 33, 25, 17,
    9, 1, 58, 50, 42, 34, 26,
    18, 10, 2, 59, 51, 43, 35,
    62, 54, 46, 38, 30, 22, 14,
    6, 61, 53, 45, 37, 29, 21,
    13, 5, 60, 52, 44, 36, 28,
    20, 12, 4, 27, 19, 11, 3
)

__PC2_PERM__ = (
    13, 16, 10, 23, 0, 4,
    2, 27, 14, 5, 20, 9,
    22, 18, 11, 3, 25, 7,
    15, 6, 26, 19, 12, 1,
    40, 51, 30, 36, 46, 54,
    29, 39, 50, 44, 32, 47,
    43, 48, 38, 55, 33, 52,
    45, 41, 49, 35, 28, 31
)

__PS_PERM__ = (
    0, 5, 1, 2, 3, 4
)

__S_LUT__ = (
    (
        14, 4, 13, 1, 2, 15, 11, 8, 3, 10, 6, 12, 5, 9, 0, 7,
        0, 15, 7, 4, 14, 2, 13, 1, 10, 6, 12, 11, 9, 5, 3, 8,
        4, 1, 14, 8, 13, 6, 2, 11, 15, 12, 9, 7, 3, 10, 5, 0,
        15, 12, 8, 2, 4, 9, 1, 7, 5, 11, 3, 14, 10, 0, 6, 13
    ),
    (
        15, 1, 8, 14, 6, 11, 3, 4, 9, 7, 2, 13, 12, 0, 5, 10,
        3, 13, 4, 7, 15, 2, 8, 14, 12, 0, 1, 10, 6, 9, 11, 5,
        0, 14, 7, 11, 10, 4, 13, 1, 5, 8, 12, 6, 9, 3, 2, 15,
        13, 8, 10, 1, 3, 15, 4, 2, 11, 6, 7, 12, 0, 5, 14, 9
    ),
    (
        10, 0, 9, 14, 6, 3, 15, 5, 1, 13, 12, 7, 11, 4, 2, 8,
        13, 7, 0, 9, 3, 4, 6, 10, 2, 8, 5, 14, 12, 11, 15, 1,
        13, 6, 4, 9, 8, 15, 3, 0, 11, 1, 2, 12, 5, 10, 14, 7,
        1, 10, 13, 0, 6, 9, 8, 7, 4, 15, 14, 3, 11, 5, 2, 12
    ),
    (
        7, 13, 14, 3, 0, 6, 9, 10, 1, 2, 8, 5, 11, 12, 4, 15,
        13, 8, 11, 5, 6, 15, 0, 3, 4, 7, 2, 12, 1, 10, 14, 9,
        10, 6, 9, 0, 12, 11, 7, 13, 15, 1, 3, 14, 5, 2, 8, 4,
        3, 15, 0, 6, 10, 1, 13, 8, 9, 4, 5, 11, 12, 7, 2, 14
    ),
    (
        2, 12, 4, 1, 7, 10, 11, 6, 8, 5, 3, 15, 13, 0, 14, 9,
        14, 11, 2, 12, 4, 7, 13, 1, 5, 0, 15, 10, 3, 9, 8, 6,
        4, 2, 1, 11, 10, 13, 7, 8, 15, 9, 12, 5, 6, 3, 0, 14,
        11, 8, 12, 7, 1, 14, 2, 13, 6, 15, 0, 9, 10, 4, 5, 3
    ),
    (
        12, 1, 10, 15, 9, 2, 6, 8, 0, 13, 3, 4, 14, 7, 5, 11,
        10, 15, 4, 2, 7, 12, 9, 5, 6, 1, 13, 14, 0, 11, 3, 8,
        9, 14, 15, 5, 2, 8, 12, 3, 7, 0, 4, 10, 1, 13, 11, 6,
        4, 3, 2, 12, 9, 5, 15, 10, 11, 14, 1, 7, 6, 0, 8, 13
    ),
    (
        4, 11, 2, 14, 15, 0, 8, 13, 3, 12, 9, 7, 5, 10, 6, 1,
        13, 0, 11, 7, 4, 9, 1, 10, 14, 3, 5, 12, 2, 15, 8, 6,
        1, 4, 11, 13, 12, 3, 7, 14, 10, 15, 6, 8, 0, 5, 9, 2,
        6, 11, 13, 8, 1, 4, 10, 7, 9, 5, 0, 15, 14, 2, 3, 12
    ),
    (
        13, 2, 8, 4, 6, 15, 11, 1, 10, 9, 3, 14, 5, 0, 12, 7,
        1, 15, 13, 8, 10, 3, 7, 4, 12, 5, 6, 11, 0, 14, 9, 2,
        7, 11, 4, 1, 9, 12, 14, 2, 0, 6, 10, 13, 15, 3, 5, 8,
        2, 1, 14, 7, 4, 10, 8, 13, 15, 12, 9, 0, 3, 5, 6, 11
    )
)


def __int_to_seq__(i_msg, nbits):
    """
    Integer to bool vector conversion.
    For internal use only.
    """
    v = list(range(nbits))
    for i in range(nbits):
        v[nbits - 1 - i] = bool(i_msg >> i & 0x01)
    return v


def __from_sequence__(seq):
    """
    Builds a des_block from the given sequence (seq).
    Should only by used by des_block internals.
    """
    db = des_block()
    db._des_block__data = seq
    return db


def __from_int__(i_msg, nbits):
    """
    Builds a des_block on nbits bits from the given i_msg int.
    Should only be used by internal functions.
    """
    return __from_sequence__(__int_to_seq__(i_msg, nbits))


class des_block:
    """
    Class providing every operations done to a message in the DES datapath.
    """

    # Some variables
    __data = []

    def __apply_table(self, table, direc=1):
        """
        Compute the permutation describe by the table on the data variable.
        Returns a new des_block containing the computed data.
        """
        res = []
        if (direc == -1):  # backward direction
            for i in range(max(table) + 1): res.append(None)
            for i in range(len(table)): res[table[i]] = self.__data[i]
        else:  # defaults to forward
            for i in range(len(table)): res.append(None)
            for i in range(len(table)): res[i] = self.__data[table[i]]
        return __from_sequence__(res)

    def __init__(self, hex_msg=None, nbits=0):
        """
        Constructor takes the message from which the des_block will be initialized.
        It must be an hexadecimal string representation of a 64 bits message.
        Example: 0f564a334af654ab
        """
        if hex_msg:
            i_msg = int(hex_msg, 16)
            self.__data = __int_to_seq__(i_msg, nbits)

    def subblock(self, begin, end):
        "Returns the subblock of data between begin and end (not included)."
        return __from_sequence__(self.__data[begin:end])

    def ip(self, direc=1):
        """
        Returns a des_block resulting of the application of the
        IP (Initial Permutation) function on the current des_block
        """
        return self.__apply_table(__IP_PERM__, direc)

    def e(self):
        """
        Returns a des_block resulting of the application of the
        E (Expansion) function on the current des_block
        """
        return self.__apply_table(__E_PERM__)

    def xor(self, db):
        "Returns the results of __data xor db."""
        res = list(map(lambda a, b: (not a and b) or (a and not b), self.__data, db.__data))
        return __from_sequence__(res)

    def s(self, n_sbox):
        """
        Returns the output of the n_sbox sbox with des_block data for
        its inputs.
        """
        pre_s = self.__apply_table(__PS_PERM__)
        return __from_int__(__S_LUT__[n_sbox][pre_s.value()], 4)

    def p(self, direc=1):
        """
        Apply the P permutation to this des_block and returns the result.
        dir is the direction in which to apply the permutation.
        1 for the forward direction
        -1 for the backward direction
        Defaults to forward.
        """
        return self.__apply_table(__P_PERM__, direc)

    def pc1(self, direc=1):
        "Apply the PC1 permutation and returns the result."
        return self.__apply_table(__PC1_PERM__, direc)

    def pc2(self, direc=1):
        "Apply the PC2 permutation and returns the result."
        return self.__apply_table(__PC2_PERM__, direc)

    def ls(self, n):
        "Returns the result of left shifting the data by n bits."
        return __from_sequence__(self.__data[n:] + self.__data[0:n])

    def rs(self, n):
        "Returns the result of right shifting the data by n bits."
        return __from_sequence__(self.__data[-n:] + self.__data[0:-n])

    def f(self, k):
        "Returns the result of the f function for the given k key."
        bs = self.e().xor(k)
        res = des_block()
        for i in range(0, 8):
            res = res.concat(bs.subblock(6 * i, 6 * i + 6).s(i))
        return res.p()

    def concat(self, db):
        "Return the concatenated des_block between self and db."
        return __from_sequence__(self.__data + db.__data)

    def value(self):
        """
        Returns the integer value corresponding to this block.
        """
        ival = 0
        for i in self.__data:
            ival <<= 1
            if i: ival += 1
        return ival

    def fill(self, db):
        """
        Returns a des_block where bit set to None are filled with bits from db.
        db must be another des_block
        """
        vect = []
        tmp = list(map(lambda x: x, db.__data))  # Copy
        tmp.reverse()
        for e in self.__data:
            if e != None:
                vect.append(e)
            else:
                vect.append(tmp.pop())
        while len(tmp) != 0:
            vect.append(tmp.pop())
        return __from_sequence__(vect)

    def hw(self):
        "Returns the hamming weight of the block"
        res = 0
        for i in self.__data:
            if i: res += 1
        return res

    def get(self, n):
        "Return the n'th element of the block"
        return self.__data[n]

    def encipher(self, key):
        """
        Encipher the block as a clear message into a cryptogram.
        According to the given key, with the DES algorithm.
        """
        kshifts = (0, 1, 1, 2, 2, 2, 2, 2, 2, 1, 2, 2, 2, 2, 2, 2, 1)
        cd = [key.pc1()]
        ki = [0]
        for i in range(1, 17):
            c = cd[i - 1].subblock(0, 28).ls(kshifts[i])
            d = cd[i - 1].subblock(28, 56).ls(kshifts[i])
            cd.append(c.concat(d))
            ki.append(cd[i].pc2())
        lr = self.ip()
        for i in range(1, 17):
            l = lr.subblock(0, 32)
            r = lr.subblock(32, 64)
            lr = r.concat(l.xor(r.f(ki[i])))
        return lr.subblock(32, 64).concat(lr.subblock(0, 32)).ip(-1)

    def __len__(self):
        return len(self.__data)

    def __str__(self):
        """
        Returns the string representation in hexadecimal of the data stored
        in the structure.
        """
        return hex(self.value())


def test():
    msg = des_block("48656c6c6f202121", 64)
    key = des_block("6b65796b65796b65", 64)
    print ("msg", msg)
    print ("key", key)
    # Cryptogram should be 71E36B810C097F33
    print("cryptogram", msg.encipher(key))

    db = __from_sequence__([True, False, None, None, True, None])
    fdb = db.fill(__from_int__(1, 3))
    print  (db._des_block__data)
    print (fdb._des_block__data)


if __name__ == "__main__":
    test()