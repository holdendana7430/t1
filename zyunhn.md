代发 wailian999

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3uidqvdge.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3yopfrmvh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aeguratb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tkjyyzps.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3tvgudjye.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hsezpvjh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bbnfrito.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vlsyqooj.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ylqzgdls.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3bbdpfvlk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3opzxanyi.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3chmdjrsy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3tldgykie.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbthoeri.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3lplowqxc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnjwwxcz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqcmsbbg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xehcvsmt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3vswpnado.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3chxbofks.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmzphejo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3txbwwwom.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3hegwmurx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3eskcurqq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3sntnggqq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wzclsunq.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3qggnqgvr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3idkdukcz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3deupilfe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fgrhhifq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3cjoaiijj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3sboeczqo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tjquigso.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pqjxycss.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vpmjobjj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3pghasbvq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kfwjhhyg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bylkrhdy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3cwoiiced.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3ogakbvqw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3dizcfljw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3rqgttqya.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3zacdxnwq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wdbeicmf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3sqrcxfuu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xthjtund.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tdjtpakz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rfvcsdfh.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3rzxldfbp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3dghkrovs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcomgbgo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3otwkxiij.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxmuqopk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gtpdujei.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ikvtzxcn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3poiuqrdf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wqpjedrs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bmomcuqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3ypzcsjmk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3acsrtiih.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uqtesqoh.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vownvphw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3apzthswj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3njqinrjj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wbqgrtkw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3scxjgnfr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kbaysrhc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3skdjdwvv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3smhcklhg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rlgmfofb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vgrwmhyk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gimfdpcw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nulxohyl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3aqkpipki.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hdchkpfy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ilxfclhg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3eniwungn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3wkruiavi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sqilzawg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3sqaedkne.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pzrfagqk.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hjcktbyb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3zmrgjrcw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kukwuzns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rxavnnjm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pxlzznbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzwmscxj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ognthbwq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gfbebqlf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhsqitlj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ikgyjyrb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkvoawo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3whdltmwc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3urtxezht.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3gwuccdel.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qzpjyswi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hrzkuhkb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xxyagoew.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3agcokdkc.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3upqsjidd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tqatmwry.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3dtfsrfzb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pcgwourr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3adxjamzr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3bxjrddhv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jvczycul.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3fqanzozk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3hicsghhx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mvizohcg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vyqvbery.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sqmthhvm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ubisnqlq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3pacrdttr.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xnyrbkuj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dolwgfsr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ypkljdrg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mwypfrum.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dftbzdko.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qwtykzpd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nbbsqarp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3cdieiibe.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zbnwpkas.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3xdgetffm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qzmhwkaz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hmkmrynb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sljilqjs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dioyutsd.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dfjpexoj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3djffrdyf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3klqlcezl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hbqvmygz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ubatkfyz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3exezwowg.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3aklijrkg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qgbbohhh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tikgtogf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dovljpoy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cqwviogf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vgjrkqmy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mnpqfiuq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wwpoaqop.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3jrwifehq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3aofmnctw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lnwdgndh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zxcemobz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3arrvzmga.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ajviekmp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pxfxuriw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hdrhgdar.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3bkmmwfna.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zvwkmocd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rnrbrkzi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceokdjal.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqywnkot.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iypzxacn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yehhucre.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mvegphto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3kwcflece.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3modmhhju.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ggbtnyfi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftypsfzp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gxbdgxau.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ozvcsdyp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oeigdxvk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ckvpuodl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3slrtfrvy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eplmyzlf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmmctdp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ncdrfhtx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rgnmeeuj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mjjalgvm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wibnfvpb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mswozish.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ngxzwqmm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3glziuexx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ugajgzub.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qudvngex.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bzlutmzq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnnmog.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bhljcrom.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3hgvuslfe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3yazkhivf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3rrxoalgz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rpjfqfkc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bawagucn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ikheivug.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gtpzwshg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3crfodwym.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3itqbidus.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hvolgotq.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cmlxsjjl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3kcgxozrl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3kxduumnm.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3gtdbnann.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3cotihkki.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zclfvskz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qqequrcy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lsxoftzh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wfcuvrps.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggrvbbxa.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dnglhtrd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3skoehupe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3xkrfhols.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3kelydhgf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3taimckmy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3tfstsbun.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xpvccmcx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3otlphbpc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xodnpwgf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3znikosrr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xdyifyxh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gvungghx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3pfgljzvg.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wppxbiyw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3dyuvzari.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3svntgycd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmaultax.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3boxskazb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zadjlwin.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kzhcblys.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jeonnvfk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wzizfvgf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3zsacoudu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3urwhlyyq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3leodqjhx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3hrwdekiy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3qjkbmdia.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pkalnqwj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3yovbyzxl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dswixqwt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dnmacrvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hwunreoh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qjswhdkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3foxpdtgx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3oexmjcdn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3cettenvo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ieuqotut.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sqttnlxn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wpifvoev.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3lheplywj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ppvnotcp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zymupcbl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cupwqytt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3scfrcpwu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pcpjjipd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fzwvewio.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vtcpzvuq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dilwrzwe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rzcayijn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ddeshiem.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3jlkrxmco.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jbwsvacz.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3igayaovk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3gwioyiwb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tzsvzgov.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3kqdaqpfj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3drjgzxcp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxflhhsq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yqfibgye.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fkwaathn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilkolszc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3yoyxzyvm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jdmgvorc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bztjuzap.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vcgfnimt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3guebrccq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xepuvxpf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3navaablp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bwgulgxh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzgbgcjw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ltwzfptj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vdhwuvdx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gzldkqbq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rhweoozp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3huzccmoz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnejlpq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mozqaqqv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cmrbhlud.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vhfzeliw.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jqzbszsg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qqvfosur.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jmjwijfa.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ptvyomtc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fgfumxlm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ujcyvbzi.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swoviqgd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3pfecohlh.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xpabuzpf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3jodaydlq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3syotnxku.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lgwtwfdz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wdhrvran.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3pzrqjhao.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uvcyuxzl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kmqojimf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3azibplze.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3torauyas.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hdjdtvkc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3fzfshcgx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3aterdzxx.html


<!-- 参考信息 -->