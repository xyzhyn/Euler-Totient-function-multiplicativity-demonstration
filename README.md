# Totient mult. demon.
**$\phi(xy) = \phi(x)\phi(y) $**
## Example
<p>Let's start with an example with 2 simple primes. The example looks stupid but it's easily formalizable and works for every pair of primes.<br>
$2*5 = 10$ <br>
$\phi(10) = \phi(2)\phi(5) = 4$ <br>
$\phi(5) = 4 = \{1, 2, 3, 4\}$ <br>
$\phi(2) = 1 = \{1\}$ <br>
<br>
    5(1) 5(2) <br>
       v v <br>
2(1) ->[][]\ <br>
2(2) ->[][]\\ <br>
2(3) ->[][]-5 <br>
2(4) ->[][]// <br>
2(5) ->[][]/ <br>
        \/ <br>
         2 <br>
<br>
> 5 numbers share the '2' divisor with whole group <br>
> 2 numbers share the '5' divisor with whole group <br>
From this reasoning we have to remove 1 element because '10' is considered twice (2(5), 5(2)) then: <br>
since the two conditions above coexist the group can be divided 5 + 2 - 1 times (by 5 + 2 - 1 numbers). Then: <br>
$5*2 - (5+2-1) = 4$ <br>
$\phi(10) = 4 = \{1,3,7,9\}$

## Formalization
We take 2 primes m,n, then:
**$\phi(m*n) = m*n - (m+n-1) = m*n -m -n + 1 = (m-1)(n-1) _$**
where
$\phi(m) = m - 1$
$\phi(n) = n - 1$

</p>
