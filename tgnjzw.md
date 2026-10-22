代发 wailian999

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fzbitvqe.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2wmynwywx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2zmgysaqw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ygfynvyy.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2zgeowxty.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2spmokeny.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcwlaikn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2apuhnvxj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jcinvplb.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xgxspxzp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vyzhvksn.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yjjvapmh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2knrenenl.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2ftqhdlez.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fhwfbhlu.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2adrfzgwb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2crcbvimo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2nlmtcbwp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2rtqqxqbh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2xvckpomq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2wwqruipn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkgrwfmg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2qhducvyb.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2cdtxpwig.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qwlwouue.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2ayainbxv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ktbvemmg.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cowigipg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2zrotsing.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vojdaxoh.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qcpzvnfz.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2kfhpasbn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2qaiprffz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yougosjm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dewipwog.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gdgptlla.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2beidvmlu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2costmrjx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2bbnttqkl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2dckhkzbf.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2stiwtjiz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2oifdeyqq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yitptful.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcqlvbhs.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2agzpgzoc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qxuwpghs.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2eqbeiqrk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2favaduaw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2tjqfaxlk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2epcjhzmx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kgvmqtza.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxkcqsc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2klxplyke.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zglcjngm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewwgabhe.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cbxrolyq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pgdvdpys.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2genqvfju.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2yxjmjbvw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2rtbesoks.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gtsqecep.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hslfjmld.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vhmmqkov.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wsnrpyft.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2idbsxylj.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mnmqzdjm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zkfaotvs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hzlwfrqw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kwpntdny.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2moqzesta.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mfjzatse.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vqxwjvxt.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yecasdnm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qooacftt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dbbmmmat.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2layiestk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wyfwfisx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwharnvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aivkmvic.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dljdwilj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pzztwljh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2daesksuw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dzyudqgs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2omlmgpkz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wfthedot.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2dnkwfdtv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zkygdxhg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksttxjjk.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vmvkdcct.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rxaafzsm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ckftccfd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xscoemfq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjdxlusu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cbjcwwlz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2izlamnjl.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jxehqcvq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rcnasnrr.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2klybqfmh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mtbgplxx.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kcivdsld.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyqfeask.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zepufwtp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbyngide.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wtlwhygd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2txyzlldd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fngqxcrj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2gitlrwax.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdbwitm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2mnvijtht.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wqlrjlbs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hbqdhnlz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mhsllmdi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cilbeuia.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bzjamgut.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2baehlend.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2qedbedkt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qwgitosz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2fokwboxu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2rkpdcafu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ysleljno.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ywpojoad.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qqizxclv.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ntoysfph.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qrnylyrc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kmnzptxi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gtzjpyfg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2mhukuhcn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2akohkklj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qtssbimx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ddfcuwcr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ktoenmqs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dtoryvuy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zdyczrhc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lhdtplse.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2viztinvl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cqpljruw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xzjgxybm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2uxnypdqa.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2dlgvixgs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2vpiozmji.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hdsagals.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gfdhxqsx.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lsjvqujv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ndpiexoc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2nqhzaxrw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2moxonhny.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gjbbxdvy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2tzmvqjlq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wkmuomvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2skamedoi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaouwhxf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2orxgncck.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfytoubc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2swoeirux.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bcautnpt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vofvrxzu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzblody.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2fgvpqmmw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sizqbnvs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2zydliplo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aybvtury.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2fwsdfcfr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2myxxmwzi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2inkicxnb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2iuehsoer.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fghkvvxh.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ttxdmvjv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ygrbtpfy.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xgmgtvta.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2exmpdyey.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hqirsned.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ilqdvizc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ubaaihbo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2tejvsybu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2zdoanbkw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2uuqnesfr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vueihetb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2tzrqajzq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gjamwvow.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2tivygpzt.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wuwjobbk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2tbeijmpo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fvpoebzf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2rqffawae.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2zlqljgpe.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qawpjubu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2dldigpox.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2sfkllytb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rokntwwu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lvkjomws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2dcbcmriy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2caoqlihj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pfkppdbl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dvlbdiye.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ydqdzeqe.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2uslkxglh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ttbxmhsk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2baodlisb.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2psbkrift.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ihrfdgqu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eeawtqyg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qhnqktws.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2nnxeayrh.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bqxcyidz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ayjmenlh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2egemavzm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rmtjjrqw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cmghxrrb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2agbfgaac.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2adipmacr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2efyhnwvt.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2niazchlm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cemqpdna.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pwoeshlk.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2svdedisf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sjxxdzxm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yrjcithi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2smccgsbo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2kukkuknf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zxaobsnq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2urigrxhk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ztmfvitx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hqxfqrhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tljglkoj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ymstlgst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcszkadl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ivuefgrq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hbzfsevj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dsoprqcb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ixsbttix.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uzsyjlei.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ofgfylqv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mufxvnjw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2seqlucdr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2fjsrvfib.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2jjyjuxup.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dfecnbku.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2neseorve.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ugwoiafd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2tocvmrhh.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2axxaeyou.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jsvnczcl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2dhxtwtgd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2pviomtap.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2pqivaafx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gfmwxkqw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pxvlnsmf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2pgetxadi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2kvrfqodm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2huqglfbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2hlkbzeqq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2fzmiyvgs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wpdeteae.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2lioimdja.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2cpmffnpp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qjunkduq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2bgeilenx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2iygmyxcl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zbggosyb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2wktmkaen.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2dqtpfbax.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lofhrtbl.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2cbmhqubo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vvwaymxt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ucavgkpx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uwdkchmb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2iqbajgxp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2xjxdhvrp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2objuwuku.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ojdlfwfg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xwvbnnhb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2zsqzmmex.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ordpplit.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2aetcfqbx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ztfbeuox.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ctvwsrdl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ibjueewq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2uuozjtaf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zszgnxzr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2dzjekrlc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2axhzdsib.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2ebjchsty.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ziustfco.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qmwpflfb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fihavfco.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rknqqswc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2rnxbljsz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jgnjbsno.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ptoncurw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yfommuyd.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2becainit.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2qbusmwid.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2zpkzwiqd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2fsrvfccq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvxuesm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fpbohjsn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zqqfexll.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cnejvcvu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bzmjtect.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2eixnfuuu.html


<!-- 参考信息 -->