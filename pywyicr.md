代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.fehbvm.com/Article/details/ghrssxger.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.zdbjq.cn/Article/details/gxyjjqimf.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gjrawwgom.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gsjwzzmrw.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fehbvm.com/Article/details/gknzgvzhg.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.hesvh.cn/Article/details/ggdjjkzji.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.zdbjq.cn/Article/details/gimoioutk.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/gtxhvnxjk.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gfybxpmum.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/geytjqxns.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.hesvh.cn/Article/details/gusdvlote.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/grjomdejt.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gbxnbwjji.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fehbvm.com/Article/details/gsswapuii.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.zdbjq.cn/Article/details/gotkekbyb.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/gbxxostlt.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/grzmquljg.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gpwgvteiz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gmaijxdzr.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzmzcmoig.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gpimxpqxh.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gzzstxtpa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gyoyfpqdk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gbnctafsg.sHtML

[B13] 判断是否为数字
来源：http://read.share.fehbvm.com/Article/details/gwvhzkkly.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gzofvcjpt.sHtML

PHP:  is_numeric($x)
来源：http://baike.fehbvm.com/Article/details/gcgggebsf.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.fehbvm.com/Article/details/guuafjlpq.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gbvkogngk.sHtML

Java: x instanceof Number
来源：http://mobile.hesvh.cn/Article/details/gdlbbfhbj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.zdbjq.cn/Article/details/gyrsuudyb.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gxudjjcyq.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/gqmdwtgac.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gievjcium.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gxbmebgqa.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.zdbjq.cn/Article/details/gnqevlrsa.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gbpxiwhqg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gcgefsxzt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fehbvm.com/Article/details/gnmzmcdbq.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.fehbvm.com/Article/details/gfijdlgeh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.zdbjq.cn/Article/details/gkymmaahj.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gdnuxigku.sHtML

[B15] 布尔运算与取反
来源：http://www.share.hesvh.cn/Article/details/grgwkmiov.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gyylrfxxo.sHtML

PHP:  $a && $b || !$c
来源：http://wap.fehbvm.com/Article/details/gejgjxjag.sHtML

JS:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gpdcobedm.sHtML

TS:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glkaylsxx.sHtML

Java: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gztmyznbd.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/golsmypza.sHtML

Ruby: a && b || !c
来源：http://blog.fehbvm.com/Article/details/gubeourpw.sHtML

C#:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gjpltpmds.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gnbmflqpo.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/goxykuasz.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/gkuvzrlwe.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/gfqzqgaqp.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/gfxpdvyqr.sHtML

Java: if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gbweypqxp.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gwsiypron.sHtML

Ruby: return if data.nil?
来源：http://wap.fehbvm.com/Article/details/gxfzosplu.sHtML

C#:   if (data == null) return;
来源：http://3g.hesvh.cn/Article/details/gedzqfyqh.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjecfaypf.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gwwqhrdic.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdyvtwbfy.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/ggqmvljgw.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gsnqiezdo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/glhmxhlbs.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gzxivarix.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gxixfffuh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gljpvyxab.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/glmjezpqk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.zdbjq.cn/Article/details/gddslbfai.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gkzbwjjkm.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/goiyqtcyb.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.zdbjq.cn/Article/details/gkqsqjauz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/gcqteokko.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gyvcjdwvh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkxzbikwt.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gqlnwpxgn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/grapqfxrz.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gtpcjcfyi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gstlrwuor.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/goxbalksk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gcdmgtqvn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.zdbjq.cn/Article/details/gbvsaepwo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gyatarbss.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/gclmumljv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.zdbjq.cn/Article/details/gqdgbnczd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.fehbvm.com/Article/details/gpjwwvpnk.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gjtvunjtq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gwflxkqph.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gryeyymbm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gzdglkfom.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gsvhuxjar.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gemcgijra.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fehbvm.com/Article/details/gxfxxnspi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/guqetrccd.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/goddqxspr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gexmrwyqy.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjsvawmdc.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gutegvjjr.sHtML

Py:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gzxmcxsjg.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.zdbjq.cn/Article/details/gcnangppo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.hesvh.cn/Article/details/gggonfikk.sHtML

TS:   return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gcchfjupz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.zdbjq.cn/Article/details/giccuwbfr.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gbeymehmp.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/gqldvqntf.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/ghqhdepxw.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gdahrheyp.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gzgmjreek.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gkntafpej.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gzdmfekre.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/glrnwpuws.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gucgdpwju.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gfqiybcbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/grxcnnjwd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/ggttvbmrr.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gvehtnize.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gavoyuztj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gmjpryrhs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/giizmuukm.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gamjgpuai.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gvymeafwm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.zdbjq.cn/Article/details/ghwjrpcci.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.fehbvm.com/Article/details/gywhnijjl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gynzizdhu.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gffodtikz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gwyfmkllt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fehbvm.com/Article/details/gmkefaimr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gjbhwkpsg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gfwfocmka.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gmicznxha.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gbxijfprh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gqxgpmibo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gnknptobq.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gcsbjasym.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gkjsfqire.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gpaaespje.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/gpyisevht.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gabytporz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gproxyuiw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.hesvh.cn/Article/details/gdgspaewz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gfqgamdwc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/grwdthibl.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gnzohrojq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gtkurterm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gtnyickch.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.fehbvm.com/Article/details/garbwwyxo.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gvoztumuu.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/guoitsobg.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gbqxzwmih.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gxqlgqimi.sHtML

C#:   块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gmtqjsfwm.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gydzjjyqp.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gzfpdsydf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/guzzelbnn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gshmjfpbm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gcisadjbg.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gcjjfeatw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/ginmaysna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gwoubyymb.sHtML

C#:   using System.Text;
来源：http://www.blog.zdbjq.cn/Article/details/gzabfkwiy.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gsgfzsxmw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gulgpstal.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gtqhiljrt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gcabqpdyv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gpkszavrc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/goxespujq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gaiuoeobv.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gbgjkhpnt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ggylgogzi.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/glczggber.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gohehyfrp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gmyraczac.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gtyrwxjui.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gzitotsmo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/grwtieasi.sHtML

Go:   func add(a, b int) int
来源：http://mobile.hesvh.cn/Article/details/gvcmpfgrx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gfghgbkxq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gacmuoubj.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gtxajtuxp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gzotxxmmk.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/goeigzebs.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gyybxnoen.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/grnqgsdni.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gqfldgvvu.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gdcskbgwh.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gvddoriku.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gyehmqqrp.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/grvfhmlyk.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glbctujcw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gaymkoykc.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmddvqpfn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.fehbvm.com/Article/details/gdlwurqvc.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gvilordtb.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gbpokcckd.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gpbfjcnqy.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gwyuxxedz.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gsigxjfti.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gvxgqewso.sHtML

PHP:  // 无重载
来源：http://3g.hesvh.cn/Article/details/gakueezkb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/ghclwygxp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.zdbjq.cn/Article/details/gumyberxp.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/ggrbvffpk.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gnapfggqt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gjtsgddip.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/giwjzhdrw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzagamqps.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.hesvh.cn/Article/details/gvvkrcvvf.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqgtegjac.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gfcfqbdag.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/gixbgoshm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gexbmwjnh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fehbvm.com/Article/details/gcnhpazjc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gjdvajjmz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gkcamtwco.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gyogcdvud.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/grgtfkjul.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gbwadykdu.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fehbvm.com/Article/details/giimavify.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gsmvfzpbn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gdyyeejvc.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gxhiuuvlj.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gmnumqlvz.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/glqhycoxq.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gyhhlrbjk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.hesvh.cn/Article/details/glgdrksgd.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/ghwphlawd.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gkfdrspkm.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gskkgviuo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gmwddlklj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gxhfldtjm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/gzsuybenh.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gdwpldlor.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/grtpxghcx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gugpbyyod.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gyxtusray.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gpjgvrssq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.hesvh.cn/Article/details/gvjiddlvu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gswrlicja.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.hesvh.cn/Article/details/gtvabbgxu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gxfssvnwy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gddllahsn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/guclqugys.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gsfmfziku.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/getqefcys.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gfxscslfv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/goaorirvr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gvizdyzgv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ghvupzyew.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gpsahacid.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gmyajqyib.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gzeigaaeb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gninfutbl.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gueojeszd.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gzbjcqlbi.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkynyamtv.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gwtdxtyed.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gvppnbhyn.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gohibaiqr.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gipnlmykc.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gycutfdsu.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gbleukibw.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gmciifufm.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gutnqhxwz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gkyloxyrr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gkyatznab.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gekzwddxi.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gyxbkiusl.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gvwcwcbig.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gpytjcsba.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gbsvsajeu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gxumqcfji.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gijwkushm.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/guzcijcfx.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gafdrklki.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/glvhrwhjz.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/ggktltxzo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gyidrwzlk.sHtML

Go:   append(a, b...)
来源：http://www.share.fehbvm.com/Article/details/ggjzbewyw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/glbgqwxyr.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gvovpjnbj.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/glksxhgyr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gieuzrmcl.sHtML

PHP:  sort($arr);
来源：http://wap.zdbjq.cn/Article/details/gagdbkitn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gkghmxgno.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gqjgjuszn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gcotkblqb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gchgdwupa.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/gzltkuorh.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gahtaejdh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gnpclceal.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/ggankrhda.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gtzkclwcm.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gqwpnwyrr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gjsxubgek.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gstdcqwjt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/goghtuadp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gcnrgdfzt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gdmjmsjfa.sHtML


<!-- 参考信息 -->