代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tapyifdv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lwspvcwf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2gxsixzyg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hjpnzmsi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ouyqijpr.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jexxmgmk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2thhhkxor.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wicfsnea.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkgvxqz.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kawpfnqb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2iswkeycv.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2vwkxqman.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ojemzzbl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2vggehdnd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2gorzaadq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwcrfcql.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ttfszicw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2cvmemojd.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zsgzoimh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kxmahyia.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2rdhrlfah.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wvvebnzq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2fzzxwgxp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2dnwgxqeo.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2jnljolka.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2eopcfdoq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hwewqkxg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cbwjyigw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2fvmgscfn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kfquqwfk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2tnuxbost.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2rbxbaayo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2tgogboyn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2kcnwecbz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gkoslaqf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uzrzhupj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kidyaaug.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ahqcpexi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2chfmtqwv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2syddnsiu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2pwuqemvk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ljjhjssf.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rwhlayin.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jiwnrmkm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bfslwrxi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2drcbxwlq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2rnqwcfwg.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wnruxqqn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2rlghrznu.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2xsmciwcv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mvouwcov.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkmtbvk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zdzjllas.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dhcewpyr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vvulgbtg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ddnounca.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqdobnbl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mlntihyc.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mvwnobrw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hnbgrcwz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2inewzdqr.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zxmqmgjr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jljjpmfn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2opuveetj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ivqopurk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gxbndfee.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pkombmds.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lucjmkle.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mmupmkdf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pufmyuqw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qtsbltlh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gbtssiph.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cdqfnbtq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ndckzuux.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vjjlzhoj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ccoodwlb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvamzwhh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cocgzisb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhwfxkay.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mrnilocf.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hservweo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2blhqzxcu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sqehgbhq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dfruhvgg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vdkmsgwf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zsgxlmzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2iiqqgcnm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2thuaehgd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2umpcafyx.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2nrixxfxt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gsyushzl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdzctnck.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pwtclaag.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2aveguyce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2utfncile.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2sfdqsdra.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eulnkypl.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlaxlsnp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bmpbpznm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xvbffezb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zckssfaz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sogbuqzu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uaqsghmp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2itsyodxf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nrwtnxeq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hwqnxcum.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2sweijitn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2jpjentgm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gbtvbsxs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jibpierk.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fljeoyzb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2xgqzxnkn.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jktolifu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gmukxrtq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2acyzmyff.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2hbtmrmmb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nfpqfmra.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwguah.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gqsgfklj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ynoavlef.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2purrkbxe.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2tvfyngwz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2zuljyiei.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hlegpjtu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ocgxtxtc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2nximiegh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2lyhlhlbf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nvuhquhd.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cnalzglv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2wkdeebss.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ohzjnase.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dmqskvyb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vywkqnwp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2enwqbpfi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2uxnxplix.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2udgbbwjn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2qmtuelej.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dmpabyyd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2anusfyxg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2aksomstp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2zupwkfgf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2hpxooijx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2goqrtzwn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ftyotyak.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zkoqcrjq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gorhvunv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jfbthjxx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2euuafawj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2nvaihkfk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fmuzkwnw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xllhvdkh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wzhmxdpl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuvcacd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qdipjtiv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kwafgarj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nmkhvtqp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qeeeslth.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vliaovtd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uixihqjk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2lpscptrg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dqhwdnvi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ugoqkosd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qkgnxuaf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lgeyndpk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jmzaooig.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zigqnulv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rwhiocru.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2mswekuyy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lmqbzxva.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uaaubnya.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wpakkzvb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yzlxkkcg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hhtrfhfx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ughwivzj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ssxbknkj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2frwuvgjs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hkzwuouq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2xkyqoaqg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2inerykwm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2beksetjd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2orlixcxu.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wstccejj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2nuyrbpqq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mfbjwvol.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zoomplsj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2dxgvgycx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nvowguag.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qmgquthl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jdrkhmgy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2cdnyinih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zespndrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvnnfexo.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlskpgva.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pfqxcpfk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cuyjdwrn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2efbtvtoq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxsoxtuh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2bpyagkfw.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2reikuqca.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2npibtonv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2knydmgty.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnzffyij.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mrvkromz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mzbkglyn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2aypmydaa.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2oibcmqtf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yylyjcwt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2mdbqtrqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ftbdopiu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rkjtklqq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xvdnnojo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ryvwkkzk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hzxraqmq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cxkpmgvy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tttsxuav.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yghtqwnp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2exwevled.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ufwawxrz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nwwxdcgi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwkalovd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2eyhjxbjd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2uxpppiqg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2trgjvnpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yeahfbik.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tyoqjjff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltkruktn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ihdkptvn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ymrhtazu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rxwkyixr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2deakvofv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2jyzavipi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2mpxfefjv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2tbekvwgn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2caiybgzt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2snuhftat.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vjdudgjd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2iukzijpq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2usighlei.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2iiyvwvbp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2evasqkhd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jgyxuozw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ukosqamj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hlefwwat.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xatetzzv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2odroqrms.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pqkjhxyg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2lyjrbldm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ncayisql.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dyodgvih.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gpzalwgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2etxyjiia.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fnrscexi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2obkywnej.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hjredyev.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2sytiurgy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xnioptxi.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jzilzbqe.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rhtpxbxg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iogopxrf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2qwygbdlr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xcxvsdnx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ixacmdlc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mimsjxol.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2knoqectd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iwtjcorn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dmkaocun.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2mzbimwfh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2yxtqxxvr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wjyhggfb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zcccugoe.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ophjkwat.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iwehlmlm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqclmjco.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2tjgwwhee.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2otjdwvfv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2agafurcq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ufzytasb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfwxrjd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2lkcehrjt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ofudbnju.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hjicrhcc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tikebfyd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2wzkqtinv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fcuswsil.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oafkihmm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2qjqptahv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rnxcudwz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tvtrwdjf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bfviltjg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2plthqlxw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2czuvgwbp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bsikopip.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qvvzavar.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2njfjxhbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2hqbtyhof.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2qfzdbrji.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ffbbcedu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qkuqeylw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2vpqydzfx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2quvzuhsk.html


<!-- 参考信息 -->