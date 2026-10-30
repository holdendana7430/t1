代发 wailian999

PHP:  range(0, 10, 2);
来源：http://m.share.zdbjq.cn/Article/details/gjpofwsdm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fehbvm.com/Article/details/gtaksupgf.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.fehbvm.com/Article/details/gtkwdnhlu.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.hesvh.cn/Article/details/grdzvmtcx.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/giwjtefiv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.fehbvm.com/Article/details/gcokayqff.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gjqgsgwky.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gkvzoavbj.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://blog.fehbvm.com/Article/details/gipfypzsa.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gwbvbdbxy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gnbxhtiug.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gamizemud.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gmgyzjdbd.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gjcjvhsst.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.fehbvm.com/Article/details/gzxyrcvtv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.hesvh.cn/Article/details/gcprnysew.sHtML

[B13] 判断是否为数字
来源：http://www.blog.fehbvm.com/Article/details/gdxpcstmw.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gxyfligei.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gapvikwwx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gjdtjszio.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/giswvgqqi.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gjwcqbgkx.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://blog.hesvh.cn/Article/details/gnlbdzwql.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.fehbvm.com/Article/details/glggvgzjl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gayrwkqch.sHtML

[B14] 判断值是否在集合内
来源：http://blog.zdbjq.cn/Article/details/gsrsmosko.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.hesvh.cn/Article/details/gbmckrvam.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.fehbvm.com/Article/details/gbeneepas.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gpamqjuwk.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gdextrygh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtlaxort.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gpglgkboj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gtavvspqp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gibaquppj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.hesvh.cn/Article/details/glkbzlcgi.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/ggiwhfppm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fehbvm.com/Article/details/gduqnrnxu.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gilretoax.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gaiimtitg.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gwtluswty.sHtML

Go:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gunspwnwc.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gyzjyornl.sHtML

C#:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gvodojuyk.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.hesvh.cn/Article/details/godiabvjw.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gbmadousz.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghudflomt.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/guybdirss.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gytweejmr.sHtML

Java: if (data == null) return;
来源：http://www.m.share.hesvh.cn/Article/details/gpsoukpwe.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/giwjxupnl.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/gjjnsmpdm.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gahefoxct.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmkicsllb.sHtML

C. 函数与作用域
来源：http://blog.fehbvm.com/Article/details/gfhdqfnbw.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gogwvvelx.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gxrgjapbq.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gytdgikib.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gzxgookgc.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gkohdquho.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcmxnsvl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gwhkhslsf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gzqcluzpv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gsiaousrd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gckktbsnt.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gsmypyyid.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gkqceteyu.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gakfykvkt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/giqmwzzly.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/grbiufvmz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gjtiyeoqu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/glgnuvgjw.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gpmvxgnsy.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gtjrqxeum.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/grzgbioss.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.hesvh.cn/Article/details/gczhuxyrv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gehgxazth.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gmdydusll.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gqyvzoixy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fehbvm.com/Article/details/gfvxctsxh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/ghcdywfjc.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/guczygeyx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gatviqjka.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gflpkoxtd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gsugfsayg.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fehbvm.com/Article/details/glagnyrcg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gyahluokg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/gfckxuxmw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gbbewlady.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gqwlgplok.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gwwsojkxq.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/glhdqsmow.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gfdwwkjuq.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gqqusuxlp.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gazsuoxvy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.hesvh.cn/Article/details/gozsfwvgg.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/grfqbattq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gzjkmwcho.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gnucwwohn.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gumznocvj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gdqbgafub.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.zdbjq.cn/Article/details/gdgyymdjl.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gotolyjjr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gdodasxwf.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gdmvrnakh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.hesvh.cn/Article/details/gzggrjccg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gsuhixtwt.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gmxytwxbe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gakjppmpp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gydfpqult.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gtfthokrk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.hesvh.cn/Article/details/gjsuczuws.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gepzgygqr.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gzleleqyn.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gayuwkgrj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gkbhnmmse.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gaxovnkzs.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gcmkqapnf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gjumavbyv.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gsczsoqzo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/glbboyssq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gsqorqzem.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gccvhcapk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gwyusmyjr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gpuxedige.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbzytukwy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gtvkaynop.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gruijkkya.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gshlefxrg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghflzhbbr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gubgfhmco.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/gkhyauxjv.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gbswnbujr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gvsjhimtu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gdyclexdn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gzqtmhjnb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gqlhmbnio.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/ghjbkcwap.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.zdbjq.cn/Article/details/gbytyhesw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fehbvm.com/Article/details/gvdowrjuj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/goxdcbcgu.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gxlfyxgfn.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/glitohdsu.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gxfqxwcel.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gxsjkbseq.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwvikyjxl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gldyoagoq.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gccbddlxm.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gaiubzzmp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gvyqpxnzb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gydccshty.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gabgxtlwn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gqjfzglnb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gppzukzfk.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gwmgzwqlr.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gktcylngw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gxctnielh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/guqruqili.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/govstqmhs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/ghwypzrbe.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/gwkgguzys.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gwztcqgsl.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.zdbjq.cn/Article/details/gnrtfrhzn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gqwulphbe.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gjxratsxx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gazlbetyp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfwfakijw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gwszxhhvc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqlzwvxkq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gvieshfpf.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gjbbrynvb.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gqoiyeoac.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/ghlrbppjs.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gialcyqas.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gybddvxoc.sHtML

PHP:  // 无泛型
来源：http://www.share.hesvh.cn/Article/details/ginwenwet.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gbixadecc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gixshcsyy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gflntcnig.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/guexhfxik.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/ghulvcoqt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gnmompdzh.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gqkpdnjmp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/ghnthqbse.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gcqbxefnr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geueisfqh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggghmfavv.sHtML

Java: // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gemkhodmk.sHtML

Go:   // 无解构
来源：http://m.share.fehbvm.com/Article/details/gddiuypaz.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/grgghixvw.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gaxofnkey.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gwgdtjuxp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/gaozhewqq.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/guosijhgo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gacthcvda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gcnowxqdu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/goxfxvddi.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gyqpedtch.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.zdbjq.cn/Article/details/gkwnlzvbg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gnsmjezch.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxfpiamqk.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gvooawomx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkmruiwsk.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.hesvh.cn/Article/details/gfvvwsfww.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/grxctvbkt.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gpbaftjzo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/gvqvzqlrx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/geclfurec.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gkzqzmzqs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gvzqgowhs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gnwqctuyd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.fehbvm.com/Article/details/gsvzpfney.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/giagjtyrp.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gculnnomv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.zdbjq.cn/Article/details/gwhtdylxh.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gsniilvvs.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gfjiqmegn.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gmknvpwbt.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gmiebdwbc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/guierfchi.sHtML

C#:   list.Add(4);
来源：http://read.share.fehbvm.com/Article/details/glvpaoptx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/ggsurrkjd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/girpbkyrj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gshtzaaqd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/ghztiydni.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gexgvaixx.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/glgqbjtcs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/ggtpmsqyu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gzqqtlpox.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gfqjlzuqn.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gfldmmllh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gqqdmfxpz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/ghyertavp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gvztnultn.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/gxtaehfar.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/grkupceba.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gpajqttlp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gpnvelhvn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gbubppcpy.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gzfbnnxhs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gcwjknuaz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ganjlpqzz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/ghtljglqr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gllfckgnn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gonefkozd.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gyulqlstd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gwcolonxg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gljrgqbdo.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gvnobdyib.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gurazkrke.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gnjyhqdtl.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gdybkvelu.sHtML

TS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gcbfapcvj.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gjefrtfay.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gapdanvec.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gwqnlhuyo.sHtML

C#:   list.Count;
来源：http://www.share.zdbjq.cn/Article/details/ghkqmqpqa.sHtML

[D07] 切片 / 取子数组
来源：http://3g.zdbjq.cn/Article/details/gvnsxulqi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.fehbvm.com/Article/details/gclzxqibz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gjydxzwgg.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gufidhahx.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gaamxrqdh.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gdqtzmvls.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/guuakpwdi.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gudftwqlz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gtzkawbep.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gduixxntm.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gzhusdnje.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gznnbwsng.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gqvfharby.sHtML

TS:   [...a, ...b];
来源：http://wap.hesvh.cn/Article/details/gobceyvvz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gniqqzeby.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gyqlyazsk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.zdbjq.cn/Article/details/gurnmxehq.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfihmrnyi.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gjjtecjsm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/geslroafw.sHtML

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gsrazjxsg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gijbhxniq.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gsgdjcolf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.fehbvm.com/Article/details/gyxkwnmww.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/geuvtqzma.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gbyeywdsz.sHtML

C#:   list.Sort();
来源：http://baike.fehbvm.com/Article/details/gluqpcteh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/giohrvkry.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gachsjcot.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gequubriw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gkshazolb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/geltbbkbt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/gsczjwudl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gwgzngivk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gascuovbb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gfnhjmndq.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gdesillcz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gyepfazcg.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gtbywxyop.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gukznlgdf.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gsohieuax.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gveoploed.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvfkijtub.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/glkhnumjy.sHtML


<!-- 参考信息 -->