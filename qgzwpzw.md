代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmfjqmlv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjszcpnnx.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fanxiaobao.xyz/Article/details/ghcrogblz.sHtML

Py:   list(range(0, 10, 2))
来源：http://baike.fanxiaobao.xyz/Article/details/ghicyukit.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrpqemex.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzhweooz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gvlwfxnrb.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzccpunf.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.fanxiaobao.xyz/Article/details/gcxlehfht.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.fanxiaobao.xyz/Article/details/gqnqiaadx.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwrqxdwe.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/giqvlfkgy.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfdmvkzb.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqdiuejo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glnzbqrwu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/grrzkmwan.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gefpxbqoj.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/guhrepqwq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.fanxiaobao.xyz/Article/details/gfygfbrzz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fanxiaobao.xyz/Article/details/gciyvvcak.sHtML

[B13] 判断是否为数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfakxgdt.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytmwmbfy.sHtML

PHP:  is_numeric($x)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxmpbdjp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbukfatv.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbevogaf.sHtML

Java: x instanceof Number
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfolauat.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/gsifgekvs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/glfgpcwaf.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuatjmsi.sHtML

[B14] 判断值是否在集合内
来源：http://blog.fanxiaobao.xyz/Article/details/gbadlykol.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocfzdfro.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebnpipxs.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/girmcftnk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/glhdftgqw.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnasogwwt.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fanxiaobao.xyz/Article/details/grrovbqtr.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/godqbrwrs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gcsqlxwej.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gfiqnvfuu.sHtML

Py:   a and b or not c
来源：http://www.share.fanxiaobao.xyz/Article/details/gzapediuz.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gdfjdzhif.sHtML

JS:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gsupdbpoc.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudvxjzbf.sHtML

Java: a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaqyvcvw.sHtML

Go:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbdenjbz.sHtML

Ruby: a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gsirhkxji.sHtML

C#:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gvrdmlvow.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/gkfumxtku.sHtML

Py:   if not data: return
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmflikbl.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnluuix.sHtML

JS:   if (!data) return;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdlteain.sHtML

TS:   if (!data) return;
来源：http://3g.fanxiaobao.xyz/Article/details/ghfywsghq.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdlwckcw.sHtML

Go:   if data == nil { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwujchun.sHtML

Ruby: return if data.nil?
来源：http://read.share.fanxiaobao.xyz/Article/details/gikdmakpx.sHtML

C#:   if (data == null) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gwofevwvh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfelqbjns.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcjqrqck.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glewsiwjl.sHtML

[C01] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/grrowgncc.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gejiywcwk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdscynxj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmmpzpaz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdmnmmcq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grpjydybl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/gkpwrcsmo.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fanxiaobao.xyz/Article/details/gcscntscv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/glysabvuu.sHtML

[C02] 默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gfkgzvtrk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fanxiaobao.xyz/Article/details/gwagrqwiz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvicbhhoh.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgmehton.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqtjrjji.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.fanxiaobao.xyz/Article/details/grlanburm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbuaztrxk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcthezaqm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcixbzyy.sHtML

[C03] 可变参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfweuullk.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmuzryhy.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwczpybsp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwsekbcp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnvnfrec.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjevhwhh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glasrozzs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqdiiffy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnwpkgdu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkzwdhwn.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwngreuc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geexuhetu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkxaqthes.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gihnqtmpf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gyborpmfr.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fanxiaobao.xyz/Article/details/gbtwwhzeg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdymyaka.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsxhxlx.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gwztnjrqi.sHtML

Py:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjrumbvg.sHtML

PHP:  return [$a, $b];
来源：http://baike.fanxiaobao.xyz/Article/details/gckrmvcba.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/guyaijhnv.sHtML

TS:   return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/gwnjffhmx.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdegtosfx.sHtML

Go:   return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/guzemujne.sHtML

Ruby: return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciydjpyd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckumrehx.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gopwknbze.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gcxarueul.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fanxiaobao.xyz/Article/details/gezsokvik.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnrpxgdsk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gxoilmymw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftjuvutk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbspbjtuh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fanxiaobao.xyz/Article/details/gztzzwtqy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrjazdwv.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fanxiaobao.xyz/Article/details/gcnfawacg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fanxiaobao.xyz/Article/details/gfiknbuxw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gcchcbeae.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmylsryep.sHtML

TS:   arr.map(String)
来源：http://baike.fanxiaobao.xyz/Article/details/gkrnhowdr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpppusuw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gfqdjonla.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrejyjhv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexwttqv.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurcmmdjt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwhqtjnq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqsleywk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqujiqjrt.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlxnrqek.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkkxeiec.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapwqmpje.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebiigmoc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfzpbrsad.sHtML

[C09] 递归
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoveubvb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzvhjcia.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzamulyuu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fanxiaobao.xyz/Article/details/gtujicnvt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gusvvnchb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhhxobdm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitehdqls.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/grwhddbwl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/giclsysqa.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gkwsfkxxh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gbabvrrar.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gxoewijfj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpqrfmcl.sHtML

TS:   同 JS
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjcyapy.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilzstgri.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfklfkdc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmbooqpn.sHtML

C#:   块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gtldcbdrn.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gowjzooli.sHtML

Py:   from module import func
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbdytetpo.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/goktbisge.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqdkluoc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fanxiaobao.xyz/Article/details/gqvjydzbi.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/gvqjkatto.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.fanxiaobao.xyz/Article/details/grajwzahy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdomoncap.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gverdjawz.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fanxiaobao.xyz/Article/details/grjywsprr.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnsvaxjy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsckrrnm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gabweoppp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gxbpnzgqy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxpvbqfh.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuzluwou.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmxivhqn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/golcedvka.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gnofjzwdq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fanxiaobao.xyz/Article/details/gsslpwxgo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gymeezwpa.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwfxathv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gawkvsbbk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gihdnyite.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfydyrea.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fanxiaobao.xyz/Article/details/gosvnciek.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gierfcjsz.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfbwsgem.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/gmdkxuqct.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gvidjpvjz.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuxiydfi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcigrdwy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaeninbj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fanxiaobao.xyz/Article/details/gtewvvinc.sHtML

Ruby: # 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gxnwccpht.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/gccvqinxr.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjspayowp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gyelurblo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gzhcfobwt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtoskbbwk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gafmsmuru.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjuontha.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/grpobhidi.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gegmfhupx.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/guxuiylnc.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gfwssqsqt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzrchncs.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gionqkbxn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/ggcsunbuj.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fanxiaobao.xyz/Article/details/gnivowkyr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gicolfirf.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkwqpfpf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gksyrgevs.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfzpkmvc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gkokmbzla.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjfclos.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmctisc.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/glkdthlid.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/glxprxcec.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gromrieqr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/grhfpcajg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fanxiaobao.xyz/Article/details/gujijxnuz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gzhbposww.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdmwqhgc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavczcsfq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fanxiaobao.xyz/Article/details/gptssgejl.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzvhvewi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fanxiaobao.xyz/Article/details/glgkxkxog.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfmibaam.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxymnhksm.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghvuzpehi.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grxlcnyzk.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvelkaqvd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwdymnmh.sHtML

C#:   list.Add(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gdkuniseh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gtuftoypt.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxtlxvml.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/golismpew.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfedrsqo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gtmypacrb.sHtML

Java: list.add(0, 0);
来源：http://mobile.fanxiaobao.xyz/Article/details/gubftrvqp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsljmmzxh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbuadmss.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/glvjafahl.sHtML

[D04] 删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkikrvcot.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprwxocnn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gsqamhpud.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmffaizms.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkujkhfez.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fanxiaobao.xyz/Article/details/goesexupi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkzymptc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gkxvcffuk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gnawajxsy.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/gpunxvunt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gfxceeojo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbwmjrfj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gyirnlkhi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gadeazlzm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gpbmzydjw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbwnucqh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gzygmzikx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gscjkdtjl.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjkkquom.sHtML

Py:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/giskdvdvc.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnosxbxvv.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbecgbrcc.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gcaaausaz.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbjbysjc.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gllbvkprx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxoqzsqq.sHtML

C#:   list.Count;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwexzagea.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgqwpvhi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/grvbbxvsc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtmgwaxus.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gwvljcmll.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gprxlsnaf.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnnesbke.sHtML

Go:   arr[1:4]
来源：http://baike.fanxiaobao.xyz/Article/details/guofafnxe.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/glfrgkhex.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksabgtvb.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gnurlbwoa.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvajlann.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaieeiagh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbzywswm.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtleckebs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gagnzvtkn.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gggtepkhw.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqzweakfs.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmhyykkr.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudettahr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnykozkv.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gaetxfvwq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gsthtgeku.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gxajyophi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmvweult.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfitxqcab.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gqmhrooql.sHtML

C#:   list.Sort();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfxmeyjk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjeyubiro.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwsjkeqv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbfpsevp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fanxiaobao.xyz/Article/details/gorzqrgku.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquhmcjgr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fanxiaobao.xyz/Article/details/goklxfrcq.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/goxvnrdzk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkxydqdi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkszpcgy.sHtML

[D11] 反转数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwfohiot.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/getvvtdkc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gaoudctej.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaferwam.sHtML


<!-- 参考信息 -->