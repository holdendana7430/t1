代发 wailian999

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2acznwbhx.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwqkwqic.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2snupxnge.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivfrbpon.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ojdqdykt.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2zxeqcheo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwacfovb.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2uzrlcktr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dozrtsrx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lhulxbpp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2gabxwhtb.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2luykldiq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eapgbahp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zwlellio.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ulqlufsd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ycnaldlu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2bzvsexyy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2yalzqfmt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zacafrrb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uwsmkgbn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwrcpztq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lytefasd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2wslzjcgd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2wafipjpv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kxhlmxld.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gojdyxmc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2nfetqftc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2deiyvupy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2bdzsmdrm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pifjcmkn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2sooiuasb.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2zsswczsq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ahrlouyo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifvhnsgt.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2ziqbtlrr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bwksxfvz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2fmifrgcp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2afrmylfw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2abzitgja.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2dmzspnfo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2tldxkxqg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mhvowqkc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cmhnnwsi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ociqcpnf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2jlqwzyzh.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lxgnsoag.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yqdqrtpt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cffyaese.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dissrlrb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2moaepxew.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2gzrvktum.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kmiplmmr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2txlbbatu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2slmmbusk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdkceabk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lfhlurzu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqjjssqp.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2zxwikpbd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2gxiusfky.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2enoeupmk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nfkdltnv.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zynuvisd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2iyswqtdx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2icmzeyoz.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cdzlkwyy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnztqxtt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gcssaryf.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2sjqnonfi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdusjfej.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fffknvjj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2dfmvtxyh.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iuurnrnp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ipbyjrss.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vlguozxt.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rpvgqahr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zbflvmmy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kjvephlt.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zudrjgea.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hzouckbz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dvroumem.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xvjdwori.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhdczeuy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2uxmcubow.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2agvfhtru.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2onwyibis.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hgfwitjn.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mdjfkiof.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2dyqallwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2drntkubz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vmbwufxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wlzayrpa.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nwvuqwcf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2dscemeea.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2duixlcvf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2egyrleoe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wbvlfmwp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nrnwfbqr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vocibdkl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2yamsqqru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hesbltjk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2svhmxjss.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jutsvtkl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vemucmgm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vavxgsep.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iobalkjw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2orglwjwz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2xninhqvg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zfjwhlue.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pkaudarh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2anptfole.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2ycvehrtj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbujldlw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hscoiqag.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2nohrbyzi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2mjydwtlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xtzrlbwo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jtobucpn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2szqqinvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2giwhtwxo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2svwnyiqt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wetaresv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rsdtpaqv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iwkarvmk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2uooyptue.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2vhgnvlod.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbaeqlpm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jssohqrr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2pbheveck.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xentmupj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zgzjhjgd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2lhpqejgr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zyodjoma.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2yrasgkow.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ezwdlsug.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cyerlnjs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2udkmmgwx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kmthkyjn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oprrrdnn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fttoiybv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2twlzyoxf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2acywxsdl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2cqmjwoej.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2iqtzqmba.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ihlrbsms.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xuskbnjj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fzqofive.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dkrdblqp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bkopqfgc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vbucxabm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2whysqqsi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ewzsejit.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2bxwspzvj.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lwnyiivk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2yceqlmkk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kmwuqvbe.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rikgbnkr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gurchjnn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqgveggj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xejduxtu.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2wncjychl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2iaoghzlo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mmfuqivc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gnxtrupq.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zetcbpzv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vdqujcjx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qsumyegb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xpqrnfjw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dtisoinf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpsbwlzb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gqknpeof.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ublvetxl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mezsnyft.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2omrqdwdn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jhmfolep.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2anomscye.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pytjvrni.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wjjbqaon.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fxhnbltp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2whqdpjux.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2neobmpgf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cgdyrrth.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ulejgadu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2okmvyjws.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ficolalw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2opmrpfpv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ipwwuztr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ogumybhi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2anoywujo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hlmzlqkb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2fsnmxqlq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2amydrmla.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bgpinggh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ueqamoor.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ojlhkkct.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2geafufxp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2pmnkjijc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxewja.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gihnfeoh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2thppsknq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ompbxlea.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2epzilwzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2majotitf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dgdkympv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wtmboqss.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2waiyfsfw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2wttdbpac.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bhcfwnhr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uualqlnq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cgmtfpkx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ymoyukho.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ulplapqz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pqmpvnps.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhntwgvu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2gronxogz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fupeahmc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dwaxvorf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2mqozqvys.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bcuevcwp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pjevqedr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uskzdbsa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwgrlcrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2aikywqtt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2exlalhht.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nhdguomg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lahajlbp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jgmzijfk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2pbwonatc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2rmorwuxq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dduemwxo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fajtujji.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sledtsqx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqsnnxju.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lfjsnknx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eegwrdkq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkrbchfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hruyydhw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ringizfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mffigmck.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2bfmoyxfd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2delifrkm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xzrzosty.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hqbkhoay.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2uenkwtjl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2riqbxaim.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ksmoewxz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gugpwerr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mdfgdszf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fgkcocao.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kzaizxjh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2xtopuipg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wjyrdjct.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iprxyctk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ybyvjajm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xccgutpu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2jujwspgv.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2aneoypuq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mixrtgkg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pmnxllcx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2hqowhzix.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gfddddkt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2aefygwqa.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2cepkygme.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qbeauhzn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gfodhrai.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mytdrlje.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mvolrefv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2djywgeqb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qvwolzgn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2oqsuepcx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2kssenptr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ygahcucc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mlcjytme.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tuzoggxo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2evegnzik.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2iewbwfgu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2qjtnikxi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pjllljot.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qquhlvto.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2oqrbvfsc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ugmpaskq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2csavjtpr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2kbcfelql.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rnlpmiga.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bdnjucaz.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pxzbifav.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uwpqaoif.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mskwweyy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vsvwjphc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2sbjsccvv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nofidbla.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qeftxqbq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2iegbtqej.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pbyyumqh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2iicgbkls.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hgqglasv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nqknpurx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2slfktodp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2cthjwzkj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2lbfnufry.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2anumqiel.html


<!-- 参考信息 -->