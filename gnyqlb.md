代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xtzzclgo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ultqboxi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3omqoujdw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3shqnpnbv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fmtxxykz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3vcfkwemc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3wdbemybm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qksmqnon.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3bswpoyuc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3tnodoays.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vztzqutx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3duejycxu.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3reescolp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3svcutshv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3keadraes.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvccrhiv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3bpuijgdd.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xhdpfczz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phjxtzql.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3fiuedosy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ooyektkf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3eecqhutf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hvmivchi.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gapoksnc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3epszoiao.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdbucpaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3xcdfikap.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3svwwfmgf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sbdirevh.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3swnezwwc.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3zvfthgef.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjkdggq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ymqdmuvl.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3zwyatzbu.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3yfkavdts.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xnqowcob.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3aamaojzb.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3pvxrnfun.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3pjyxasce.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3dbedhrfx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfkntlx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cnyvgceb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xmsqmytp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xpxubftw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3hyqtivwl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vswbjext.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3wttdimqh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pdzqrjua.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3budpbsme.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbblpfrg.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nkpsrbyb.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ixbcajhp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3seztvffl.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zizonpfd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dzinqegf.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3hborneky.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3cjooqrku.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3syekhavc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ohridjle.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nphfiafx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3brtnvbtj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hhjuctdq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wdeutypc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pkzjbrsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btyaondg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lljkyuai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyiupfxb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bxyufgdn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3whbgperb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlekmqmc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwmucxpt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qryvbeve.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3szhlawub.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3bxmxraje.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvbqtsom.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tkghgmnt.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhbxuhjo.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3zsikyctq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3djffdswo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3gzdbrchd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vzvbmgvr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ajrsrhis.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkjwrhue.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hpdybjun.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xvkrelqt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mxolaogk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3bukfwmil.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rcybumnx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fwavyrpp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3gzfnglhf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mrdguqvk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3lxksngia.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3iqfpyuha.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3tbytqvfs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3smuinktx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlsgwft.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3gfmtexhp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oyozdniv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xowkbzdq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bnholism.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3luwlyvba.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uzghbhtj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hxjpqdmt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fgjzylvw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3uqidwwcz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3twpsedyi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tbnvurka.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ybhklyud.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jndcaixl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jayjjutg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3idfecssz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rxidwuze.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kdcqcqvp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3evsmvczk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jfzdexjd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rtsvqjby.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wuzvpdav.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rdmqeefi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vbqqzuzy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xjvbhncs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3buulqfus.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ksyheocj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3kuyfcsgn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkjdhdgz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3epcllymq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3olnoujxl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bhbgewat.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3mqvvmboh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uieeqsjm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3oyhnpjnj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qncnociu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3fnczpcaj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwjewmn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3acmvnlfy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pbaunfpz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3anulfwri.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eyujglkz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mtawiszp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3njgusand.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3rmcaqpzk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3enkepbvw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dhxrhtbq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mjdnmkmo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3glzajwtn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3agrkjkof.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddufyfkt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lktfaqwm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3awakibqf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ublwwhvu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ywcmqnph.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3kcnoynzq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3furpljod.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3jjvugkmj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kilsoiwq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gncqbgpb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3ovwulmfl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aulbxprm.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mnnlhyui.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ofqempnz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3awoqxeab.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3thsfajin.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3glhoksap.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ozjrtpyc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3yjcidvvi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tdppuoyy.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gqbyxlws.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3llajgwrz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3fzsxjkvl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3crslutxw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tewzzboz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sswdbwjn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jefzdehe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3usdggrxk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3npbdgdyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3flbjwwbw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3hmvcelwr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3ozzmpefe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ojzyekdx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zzycriqj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3snbfahtb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmwxhvtd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ahaesqnl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jqlqyrfw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3bnrekrma.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ssoucxmx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3vxtkdjdz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dvzukfsv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3lthmxgmu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqllepeq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ucfnysdp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3joftkvwh.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fhhwwydw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tzmjmrav.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tihhskpn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wjrrmwig.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3piwgmodj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3axjiaudg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kvhnypaj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xonaiqik.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ozitrrmu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fzfnqqwr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ahbnjwjr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3krjwcxki.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3nmfrkxhm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3zzvhgoqj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dqoueiey.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3njdydmst.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aztfvrra.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tlykxmyt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3agkqsyfw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbizvacc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kuuavuau.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3bulfdkxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niaxzdaa.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jbwsmfsu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bghijdzp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ayyhfqig.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lqargsbb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pedzjtyw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dhlbeszc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qlvjmlad.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gckbqsdu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sritcabl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3salvzqqm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ltowfpvl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mxdxgfeq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ztpqqcki.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pqljkojo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rozkjflh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3trqpdsfu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xamnjsxe.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xpygareb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lsrvwcmr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pokyjbrv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3lxoevyne.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rgonczsq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xzyymhfl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eptktqmr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3iselfxzq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3yyxtwwqi.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vijrpfsl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ioxpgtlz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fzkdyeqr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3kgmrzujc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sqqutyot.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3olynpbxy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3mucktpkz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ojhtargs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3guhedrcq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lpuxykjz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cehrfysv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3efltsohp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pcafybwj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zclbwkef.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gigdgzsu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tgwpniuy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tjfyusri.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fzfuhimv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dhcoeltm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rwwtkpbe.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3telsoeqy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yzhlsxmw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nxajrtxv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eegifywn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3hpiamhws.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lvpunfsx.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3eguyghee.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3evuqwknz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gwgsdolh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qugplxvk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zcjvctgp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ovqexmcm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgtygwaa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3itxkqpon.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3eqzdgwei.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qbeefxyl.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zgkfhonf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ouvbfytm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3misnhuyy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3gbjdmuto.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3cbtrccrt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3lyngdirr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3eqxadumi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ppuckxxf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgzwmtbv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3efeoczfp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3kalclfnk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eaijapns.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bhbpbypp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ydwenjdc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3eclrwznw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3depcrtbb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hrgjqzee.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aghnykpg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ocguthhl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fanyaptj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3triqkcee.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ldohcaxh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jlhbprjh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hwcihxvj.html


<!-- 参考信息 -->