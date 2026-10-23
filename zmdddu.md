代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3gkkogycd.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ifbjlgaf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ljvtvahx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ngjsvpdz.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hvqvzdjy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3artxxuxz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mtgromxt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zjarcqlk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3qhsfokif.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rtpeguwe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lolwpfjo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qblrmuhf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cfinbuqg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3uiwthgds.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bvqpqrsw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bagskejv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uwmouczn.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3mnfziwjq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3fcdhowrj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3diodnroz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3vujquxvq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3psetkzto.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xucjollh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nulhnrxx.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwrunuvp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zjoxxwmm.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3oofdlrzv.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3wjesckxx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ypfganfe.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ihjzujjc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ncalovwo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3tqrvisrk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vgvtnhzp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zmcmdmtf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tntanogt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3saqzceab.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ssxhfvqn.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlnecpnq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3efekxyri.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xbajabnz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3pzsdybmm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vgpxsfxf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3snnbijjh.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3toxrddfl.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qbiqdfkb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qbnkymes.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rpldjoeo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3kpvoqhau.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ybvlasec.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mcbshevh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hutkzbgw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3eiztaiti.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3cbchmicc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvhigjb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hulpikjr.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jxuvwkrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ooiodzaq.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ogsmfipf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ijelpjuj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wdtdmucy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pbzzwfat.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gauwauuh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hcqqxfga.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3blwzewqy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfujibq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3elthpzqz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjucnfzp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uijhqwit.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gajrkqqf.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3quvzwslf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nmffzjhw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrsqsary.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nplnyhbq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qgwpegje.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bnpeozkw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3weevrwke.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ejalxnym.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3iezjhjgd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3gsuzerrd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ratjcezc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3eesagfjw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgedutzq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnwcngui.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qnddjugi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctuniejp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nateaudr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ccdbgtdd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dctpahdh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3letvtyoy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uvkmwgqq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3fwhlgelh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3kfljnpmi.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3yzivjdxj.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3esoqrjfl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujohbbfp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mitmirrd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ndkykgij.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3arhswjfw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ndglefni.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qfuxqwru.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3oxchiwxm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3khallkns.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3hsyowulw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3eacgdnsi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3piviiosn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bslgjfhw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3tajebsyu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cluztwin.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xmwlrkvn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ahlniiai.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zkwnphfz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3lvypzyai.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tvnvdbqo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3exykmwoz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uubnvsax.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fnridftn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vtnknijr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lcazhuib.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qyxblkrb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ptqszfxr.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3lfohpklz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3psongtwt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3awxanpdx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3swsgnixc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3smkexytm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3draqwgso.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rohkryaj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hihahfhb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lmcujevt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3zqnwdlwl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ekibdqeq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3sksyikms.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3bslaoujd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvxjlpoi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rslfzzwp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rtxdxlds.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3honlaoan.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xmqcqwkq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bnnlpydf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3bfvhxric.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3koroxqnc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3yrsqrlmm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pjovepgc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ofqgnhva.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lszkpudc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xnxltrlm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tuiwhond.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uszcgbps.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uoaytwdn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3hiabjfyi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tmuyypuc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3halyzeol.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nulnyxqa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mnvbofce.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qovshdus.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3mrmcpksi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3btqhhxpi.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxdajhk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yraqdyxe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rdnusqfq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3pfpyoqsn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dxibxjzm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tbvpekje.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wxtkevju.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wrufoibc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ayvfbxqg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xdfgdnpn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3xutelncd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wvbddutb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vpjvvomv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gpxvsxpc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkclqcun.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhbhksmk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3efwpbpbd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3vwgenghp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mxgyhvui.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3fdlmhpgm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ghewwoye.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3otxdxaur.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qogexdqd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uerrlixd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3axbtzkif.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3oeyubegk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mlgwqktr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qkvynolx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ajnijtox.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3matcemqa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zqfpfvku.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiaxcqgn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ametfqrk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gozadomj.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aagutqkj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3lucqneyx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zlbixjlv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3auxgecvn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3rheqyixz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zgpxhptj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wvmgnnkj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3spftqfjx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwkopwgr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tnwgskfr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pxwujzvr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3magtksnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exlhxlxz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lkgbsvip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgwavsak.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ysfhucmq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3klqlanok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cglawsgc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3pbmaytyn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ligjmvfw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3jpvemolx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3ryryddti.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3xmapbbxz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3yejqueej.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ifmskksn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qnegoygr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fcmqnfzq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ubuazanr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vouwvdzm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vesprkgq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3kkdgfitu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tsclgaux.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hayomhls.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3lgjhxbtf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hyoxaecj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3dayuleth.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eotstcjy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3otvpncae.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uilbzgtk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3yhfegaiy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qnlnbibv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bmjzqiao.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nuafkvuo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jcxuvgzw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qgbxsewz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3bizjvpoq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cwzfperl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vraxkwrn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3cxkigmbc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3kovuxslx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3amqoslik.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3dbhrbyub.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ibvwsmcp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3glykxvys.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3agfsarlx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gthfpgij.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uzkngsls.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vmfhftzl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fzsnfcuc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yhvydmwn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zsxaclcm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bwhcgnmu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgbkysma.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fzpwdimf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3safyzebw.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3mtkpadro.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nabqyrlb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ohjvgqyv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rmucyqah.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xbmpawgi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wlemqrtr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hteuacvq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xteecjaa.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qxgfczub.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fgohaioy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ckdjbovf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3whzlsjgi.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vaauuakz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3qwzlefpd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kmpmczhv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3jeefcfte.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jfytyxtn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3hjshhjdj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3boqxflmf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mokuitqt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3nsurwnvy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yhgqiabm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3sgcwhbsm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3htluwsse.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnjwvf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3twbtkpmt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3erdrwhwo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3isotdwra.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnhmwbuq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3iepapakl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ywenffzi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xassdlws.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3empidmdd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ltvvzrgj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ooiabnrv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ogcevknn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pznjcezu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3tqlfqoxy.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3dlhqnzvh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dddhpbmo.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cowuiupf.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3leyceivt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mduptfah.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3onaeonow.html


<!-- 参考信息 -->