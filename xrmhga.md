代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2juxpdneo.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2ewpuiojo.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2hewdoaod.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2bqgagqag.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2nasafgmm.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xmlxbqnx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2gywaduxe.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2thqzyjkz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2fwlcjeds.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2edmbyjmd.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zryyvyzz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2yyoqmnca.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ilwwfjtr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fipdjxkf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nugoqcnn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xnpyxztl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zneeldfv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xkusrzgs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fcwjrcza.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2bockwjgd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2mmziojwb.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2myubguef.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2yqrbeprx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwognnfq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oswoyuzi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2uzjrbgth.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2otkkydea.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dmuigvmb.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2sbvrjnvn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uxpxysws.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2ocigbdic.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bejnjhae.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rgoccdmj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2npahkmtn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2firzckgm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xspuxhgd.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2weuehdzs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2wiwixnfi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2lptzhbwi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2fwibzsya.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jztmlvdm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vzjdiqpg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcpbnsbg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2khicvmht.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xddhrcow.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gdnjbwrh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2pdmlepxb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2ffqmmbbf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2biziasxy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2phtsvrqk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uqfeinof.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djtxtvri.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jrjbbmvj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bzubfndz.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fuodsszc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2pngzspre.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2qfokzmkd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vfqbmpmn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fmopsdag.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pgggrvru.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ejrvxvbk.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dyrsceic.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wqzdpzlv.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xbwnuzwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fprrzswz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfsyagwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivmkrhbf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nzywoabp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hphsjyln.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhxwvwzq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oqtuvtyy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wgxxavbq.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwuncjus.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ysvbaohv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qwztdfuv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vymfnyis.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2aiucxrte.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2suulzujj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2djnsohtk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2eiecucef.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxoailwz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2tsfwwmgv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2bruzkjrt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2cvtzvdmn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2okdxdnxd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2amguwvdh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vltqwcqm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2orqhxlic.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxxnlhd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncxfumre.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdjjtbte.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2niostnxd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2exdcbwhf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hzlebdzq.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2necdsaop.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2zqltecty.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gfdkvmcz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkjulise.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2zickmtwm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fngeaigo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2msmgipgb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vwfmmrer.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qhwzknvw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2beydcber.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jxlngzof.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2kfxeiobr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2dvdsvivf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dvzulmbe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2rdxupjlv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dgwymxfw.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qxqufdzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2odpspuva.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pbvoerxo.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tezdcsdd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2zfkjhhnv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2glxmdnvy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2emqwslhm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xswcmjsy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jvdljrci.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2sluupfjo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rqhqlkwt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rzcgalkf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gkeyzwwu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2fvfbzjhp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zjykxjig.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lipzrqse.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pgfrdvcg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jaytwstp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2tdplfnxd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2iojzbsvb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ovivfqnq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iafyzloa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2siswsbbq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlytnekt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2arpnjepm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2jicbchzg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2vpbiuhzr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrbawfhb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bggjpnuk.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vxuuywck.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bmddnukf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ukhvxsuh.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2nwswuqkd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gdpvhflx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ilgtkfvs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2prktrvon.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hgkpasfo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ppvmpeca.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ycmvdbyy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ylzmhtyr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ulqeulgp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pycpfmwe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nlursrex.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mclkrrkz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zzmducpx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2grgpycgk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nlhzntom.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ftpnsgfp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ktgalwwc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2agjnrwrn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2hvcoahue.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yewbfyul.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2hfhptqth.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fvvusreh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xuzvuuwl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qwcqmifb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pndmabti.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dtnzujwd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2xbhwqabd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vtpucczm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hnwawlvd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2sqwxohni.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2wjyptqaq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jssvvmrh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2clpjbbwu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ywlnhnrr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gdpoxmwj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nydkfjij.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2barvwgsv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nfqjjouj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gkpjdgcc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2epliweyw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2fhnapgxs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jrohxwnv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pddxxfey.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lrvkngum.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2noeiyncc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cyymsmdg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxpzjzfr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wnshqgfj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2swfvmmbu.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2exzaocda.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sqgyfdpz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2rovwfltm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kechdgxx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2srwvgkyv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ozonfucz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqjviwck.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hakcpvik.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cgehbokm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2inlgbbbh.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2telvvnle.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jqniphcs.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xuncunch.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxubgick.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2avkglwfa.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tdwltgid.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nalynsba.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ftwbqliz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2kbwugoza.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hpqwcaqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thbubkfh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2kvbbqoww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pgpbqroq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ksetuctj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2bnsriroa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aeylznum.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cafsdqep.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gzjihiol.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2rskldkcw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2covfjvvv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2jjhhnsma.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wuwwwwac.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2olgjyggl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2msiaekhx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jxnfpcao.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nncdedxi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ettmeeza.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2tklndonj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ragsqtfe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hpcdugtf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2agkxahix.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qvofospv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zfnvekiy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2inepqdhd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2rkcxggri.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sdzffaar.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2apvzesis.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fihbwoox.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2iuwoxilw.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dshrosnn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2loumtidb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oruqiqfh.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qlkramxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rfaaggij.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ctdmrerh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mxcedxvq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2dkhbfegi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2roabobeb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2eezvdmuo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2kigiyqze.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mdcytgzg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rcxqqazo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xqmtiyoh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2oveajccm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2tlfdykkm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tedxafgw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lsetpgux.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rfqhtkte.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pezihtmu.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2koalmxnz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ruwrajkr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gtepbhyy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tuyonjgt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kvzhokqo.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfnfpdmu.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jtweogzz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2uaosublc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2uoxwsaah.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gzbzclbd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2exiwekwn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ipiucqmn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zetyrunf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2aovjszch.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fqqjzykp.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2tuqsqdzb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2harwghwz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2nhrxpvut.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rqizjcem.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wzbljlab.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qhtmluhc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2mabsmwjn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kvpgjygq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2bjlbryst.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2grfkfreo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2axnrljdz.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2kdnxxrni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2rneupkmt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ozbpkkwv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2denfgyih.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jfrrqast.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mgepiftr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zmhrbeqz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibbybrkj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hcfwwfda.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2cqvykvmp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2bpmezbby.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vweesuon.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2enepbnzl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tentaobr.html


<!-- 参考信息 -->