代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giehhdvnn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gskfgauil.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gclltkpnp.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gsobegjsn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkzabagq.sHtML

Ruby: (0...10).step(2).to_a
来源：http://wap.fanxiaobao.xyz/Article/details/gtoneeasl.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmgwlrduj.sHtML

[B12] 跳出多层循环
来源：http://blog.fanxiaobao.xyz/Article/details/gngugswaq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.fanxiaobao.xyz/Article/details/geisreuct.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjixlcqs.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjclcqld.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gpblfzeke.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gexyfpbue.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gokqrbwxm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fanxiaobao.xyz/Article/details/godqkjctg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhdlqesq.sHtML

[B13] 判断是否为数字
来源：http://baike.fanxiaobao.xyz/Article/details/gxngdzcdt.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxhcfmh.sHtML

PHP:  is_numeric($x)
来源：http://wap.fanxiaobao.xyz/Article/details/garctjeyd.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbxokycwo.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxqncfzb.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gigawrgcp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdkehwac.sHtML

Ruby: x.is_a?(Numeric)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbwnkxehs.sHtML

C#:   x is int or double or decimal
来源：http://baike.fanxiaobao.xyz/Article/details/grtoarajl.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrjzeaub.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.fanxiaobao.xyz/Article/details/gbazwcpqr.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsonkxtg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghccycsxe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gejssthmy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpyrnsjye.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvpmowje.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwksjxklg.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/grdyiklns.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixmwznb.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/goxkzwcnz.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwduiuyyp.sHtML

JS:   a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gicesnhdm.sHtML

TS:   a && b || !c
来源：http://baike.fanxiaobao.xyz/Article/details/gdorpzmzl.sHtML

Java: a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gcgxdrtvn.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gpkngwfzt.sHtML

Ruby: a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflfjrmts.sHtML

C#:   a && b || !c
来源：http://wap.fanxiaobao.xyz/Article/details/givokcaqv.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.fanxiaobao.xyz/Article/details/gskzmidzs.sHtML

Py:   if not data: return
来源：http://baike.fanxiaobao.xyz/Article/details/gvhozunoc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gthqkegpa.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjpsvtxa.sHtML

TS:   if (!data) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gypumfjff.sHtML

Java: if (data == null) return;
来源：http://wap.fanxiaobao.xyz/Article/details/gqlhiamho.sHtML

Go:   if data == nil { return }
来源：http://baike.fanxiaobao.xyz/Article/details/gpzngtspi.sHtML

Ruby: return if data.nil?
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbtzvbpp.sHtML

C#:   if (data == null) return;
来源：http://3g.fanxiaobao.xyz/Article/details/gmidqysgz.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gmsqntyps.sHtML

C. 函数与作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/guukyqyzs.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grpbrhejk.sHtML

[C01] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/ggoxnwttx.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpqoabhj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gtuwpxuhj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gilybsvdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdymsbyvb.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gduxfhuax.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gqgwkbhdy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fanxiaobao.xyz/Article/details/getmmpvkx.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gshkzmxqh.sHtML

[C02] 默认参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjzisqcy.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fanxiaobao.xyz/Article/details/gnucjfgdg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwwlawcte.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmadthqx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gznyfafyn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fanxiaobao.xyz/Article/details/gdxgspylf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbnjpoai.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/grhcaorrp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbzcqaqwc.sHtML

[C03] 可变参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvihndnom.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fanxiaobao.xyz/Article/details/ghewjrntm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.fanxiaobao.xyz/Article/details/gtbfzbdyd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbmffiki.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geecltkey.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfenyulzs.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/gqzcvwtdj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmyyvdwy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbxudoox.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqaikmwho.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybcqprgk.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjidkzqpx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gseieenxy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.fanxiaobao.xyz/Article/details/gkeoodigu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fanxiaobao.xyz/Article/details/gyhbardme.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdakdmtk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjmnxnye.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbndxaegf.sHtML

[C05] 返回多个值
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqlcnont.sHtML

Py:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/ghloyikro.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxvuxott.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwulypime.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjfxamtm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/glqivvqqx.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gndltkyxn.sHtML

Ruby: return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqdutrnv.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbdtxcyv.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.fanxiaobao.xyz/Article/details/ggpyxjfgs.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fanxiaobao.xyz/Article/details/gdayfwluh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahzixmxs.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnyxawzzg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhsoyfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjggzghln.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjrajvto.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtftiyush.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrwpvnav.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gmdwbzgjp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fanxiaobao.xyz/Article/details/grxrsclht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlwqupzu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/goegganxs.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpbcgcsw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzmugiqp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gddnchixo.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyjkojsl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsqhmbty.sHtML

[C08] 闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gskrvznzu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptntcvbl.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfaxietfs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdqdkjol.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gifzlsgeu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fanxiaobao.xyz/Article/details/gdlllyjez.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gorxewlxa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/glejcrbga.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdedaows.sHtML

[C09] 递归
来源：http://wap.fanxiaobao.xyz/Article/details/gjbqskbdv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gpbsykcib.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtkpqfjs.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkenqtspi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gtlvpanbi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gqvidasbc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fanxiaobao.xyz/Article/details/gyocjffpg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlrcclaz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gkaeskjzw.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/grjtxorsm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gviccxued.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fanxiaobao.xyz/Article/details/ghwyclurl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhudgdvz.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpmttbme.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/grmroefey.sHtML

Go:   花括号块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhbidvkw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fanxiaobao.xyz/Article/details/gneuejfbv.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gvjjuzseo.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gnwbkoijf.sHtML

Py:   from module import func
来源：http://blog.fanxiaobao.xyz/Article/details/gcrmvlsdw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fanxiaobao.xyz/Article/details/gerfgpcqy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/gynigamha.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrvvwlmx.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/glykrurze.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gowtzuoxw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gmulacuwx.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciptiboi.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fanxiaobao.xyz/Article/details/gexuwwmhk.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwiipmdao.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/gqreytccm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gjsawwkhx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gpdqqmqtc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gwopmhudg.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.fanxiaobao.xyz/Article/details/gxjeolhdy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjzjriby.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlhcawam.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxlnrmm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gjhodhpxm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrythhet.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fanxiaobao.xyz/Article/details/gniievnxk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsjmhdnne.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gvzhkocjc.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnybiow.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/ggpaubqlu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdusawcla.sHtML

[C14] 泛型函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdgsyvka.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fanxiaobao.xyz/Article/details/gqpgjqlix.sHtML

PHP:  // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzbrxiyq.sHtML

JS:   // 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/gqlamxhqh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzniqqoxp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gacfojapi.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqtojdap.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxjhhjcx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gcvuxonbw.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/giueauvdj.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fanxiaobao.xyz/Article/details/goxmriudz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyepwmyuk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvmelvbk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gvngxqxuy.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvrkpmab.sHtML

Go:   // 无解构
来源：http://baike.fanxiaobao.xyz/Article/details/gxevzjqez.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxhgpapq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxyeuabqa.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gikhmykxm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqkdyqin.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gikoheiyw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/glghxtrvx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpwcfgiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gutmdaohv.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/gjoamsgem.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchhnztpd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gutyukvgd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/glflsiiih.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gttazurlv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gtzpnbihb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fanxiaobao.xyz/Article/details/gecvxawez.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/godigclgk.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fanxiaobao.xyz/Article/details/gideuratj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.fanxiaobao.xyz/Article/details/gedrvabke.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzgosbgb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gngyvbswk.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhlqldnp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtopqzpn.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnyivegx.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gocjvneah.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fanxiaobao.xyz/Article/details/gvmpmgjeg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/grhhjjlcr.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gvpzoktqd.sHtML

TS:   arr.push(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjxdxhrf.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gqzhupgvu.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gpazxjgyu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gydswstkl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejkazgkk.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gapymuejn.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgfedgrz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gfobshnnq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.fanxiaobao.xyz/Article/details/gszwnkjjd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmurwbvj.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowsmtxlc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnbhvkqm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmrtrogb.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowigsnxx.sHtML

[D04] 删除元素
来源：http://read.share.fanxiaobao.xyz/Article/details/glvdqohwj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggihckhec.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gxdaxyxto.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fanxiaobao.xyz/Article/details/gsrlzygcy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyduwcmew.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqickkxko.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqdfjebw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyckeugyk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrinqfyz.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gjxdjczqs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gyyjckcmj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fanxiaobao.xyz/Article/details/gigjbpkbv.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gogdvzvzj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnzuyqjw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqynibtb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/ghzpkxgio.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsezhpez.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyttbeik.sHtML

[D06] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmngonvd.sHtML

Py:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqwezjnv.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gntmvfhot.sHtML

JS:   arr.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvngvdptu.sHtML

TS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzjzrmvz.sHtML

Java: list.size();
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuethzht.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/ggpbcxbft.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gfvteuder.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghevohqsi.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/gldllvnth.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsrzqimf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfrklxha.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gagiqtmem.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gybtomztd.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/glaarfnye.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gnoxpjudf.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxrjytfc.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmaywflq.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gaomxsebh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbebelix.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzweamsz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyytclfjy.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gicpjchcy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/grkratxkx.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtatopgn.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fanxiaobao.xyz/Article/details/giqckfmqd.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gknmexdgm.sHtML

[D09] 排序（升序）
来源：http://3g.fanxiaobao.xyz/Article/details/gbpwhexls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyzwmkvq.sHtML

PHP:  sort($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/glffbfjzi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrkqqnbc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgpmtkic.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevblkbxf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmbkltx.sHtML

Ruby: arr.sort
来源：http://3g.fanxiaobao.xyz/Article/details/gkebxabez.sHtML

C#:   list.Sort();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjmyxutw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fanxiaobao.xyz/Article/details/gjsalvjce.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjghbtlad.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyqnrurn.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gxareuwww.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guperxeoa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxpamqbc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/galzuspjg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/gvhxapwjh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/giesapqwh.sHtML

[D11] 反转数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxmxzazz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/geqalhpcn.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsvnnkbdm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/ganjlazno.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjnkpjqe.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapkqdjiw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gblmctkpi.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gssdjutfp.sHtML


<!-- 参考信息 -->