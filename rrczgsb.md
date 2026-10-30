代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/gyuxxffnn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.fehbvm.com/Article/details/gsxrnepbn.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gwocyzpss.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gzimipnnc.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/grykxelzy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gswfvxvcu.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.m.share.zdbjq.cn/Article/details/gccmydsdh.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.zdbjq.cn/Article/details/gxbelokha.sHtML

[B13] 判断是否为数字
来源：http://blog.fehbvm.com/Article/details/gljoirgpy.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/gkblqpupv.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/giwceiupt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.zdbjq.cn/Article/details/gwufsfhcg.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.zdbjq.cn/Article/details/grpgmunkh.sHtML

Java: x instanceof Number
来源：http://m.share.fehbvm.com/Article/details/gpfhpfmlp.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fehbvm.com/Article/details/gfgiiueen.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gdwnumrho.sHtML

C#:   x is int or double or decimal
来源：http://mobile.fehbvm.com/Article/details/geusfnant.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.hesvh.cn/Article/details/gvomnbywa.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fehbvm.com/Article/details/geuobwcog.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gaccldjfy.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gssnzhydf.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/gxtkzhssn.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/grzvrdsrl.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://wap.fehbvm.com/Article/details/gjinswnia.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.fehbvm.com/Article/details/gkphggonz.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gveujiunj.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gtlszfuvp.sHtML

Py:   a and b or not c
来源：http://baike.fehbvm.com/Article/details/ghqmliyhu.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gqlngirpo.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gawcdardp.sHtML

TS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/glyfwqmrk.sHtML

Java: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gjqrcedmt.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gaiyjlgmh.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gikbzmfop.sHtML

C#:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gtbntxacr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.share.zdbjq.cn/Article/details/gcqwlyalt.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gqpcfricn.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gnzojzoyb.sHtML

JS:   if (!data) return;
来源：http://www.m.share.hesvh.cn/Article/details/gymrsdnap.sHtML

TS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gewtpbflr.sHtML

Java: if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gyeyjtikh.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gbgkqnaae.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gcipzigwo.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gkyilvyap.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdfggjbbu.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gawcnmmbd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghqwcmayf.sHtML

[C01] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gutlzdrgy.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.zdbjq.cn/Article/details/gkyvctspy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gzlxbgeha.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gvnorpduk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/geaycstav.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gkvaptpas.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/glbusqppp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gbigwkeyj.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gwsbrfzfs.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gjzzkvgwy.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gyymuazam.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gzntpgzdr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gpnsasbfk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gqsmtrzcp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fehbvm.com/Article/details/gtdyznxhp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.zdbjq.cn/Article/details/gebbtmgmv.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gpsviwsol.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.hesvh.cn/Article/details/gzpobtimq.sHtML

[C03] 可变参数
来源：http://www.blog.hesvh.cn/Article/details/gupapygyt.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gmadifcuw.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gcnasidwz.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gceqlboja.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gjjrkxtay.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gjfujskzk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.fehbvm.com/Article/details/giliutqor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gkfalikbh.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.zdbjq.cn/Article/details/grrkinxfz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.zdbjq.cn/Article/details/gsoxtqpwc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gkzosjhhs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gfokmcplc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gjpctlntt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gspasubat.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gcmoxisgf.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/giiuqdmkw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gfmtjffib.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/ghxtikcni.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gtynlakvz.sHtML

Py:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gvocgtxeo.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gqhutclva.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gkioezemz.sHtML

TS:   return { a, b };
来源：http://m.share.fehbvm.com/Article/details/ggirdriyg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gwrrrlwtt.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gknpdgybx.sHtML

Ruby: return a, b
来源：http://m.share.hesvh.cn/Article/details/gikiaioki.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gsoccenja.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gecfembkt.sHtML

Py:   square = lambda x: x * x
来源：http://3g.hesvh.cn/Article/details/grkebdbyv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gkmslghww.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/grmiqiplh.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gxuwweyih.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gpcfufiua.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmeqwvihn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gzivaummv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gnqnujklt.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gzbfokmqg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/guwrgyapv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gqtsbctbv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gxbdmxiyg.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gyscgbobo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gwyvnalwr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gkhvkymns.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gjpebahbn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.fehbvm.com/Article/details/gghjqekmp.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/gbjmxfkpf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/grmmvjody.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.fehbvm.com/Article/details/ghrgfdbtl.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxbpldkww.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/ghjkofylo.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/gfsjxlcvu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gfugmethw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gccfqdqsc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gbxybflww.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gngkonkds.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/githeptqf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.hesvh.cn/Article/details/glcuwwxam.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/guptzxxps.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gahyvwzqy.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gkvajxcck.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/glacekqnl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gyxxpvrvf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gluwaimxl.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbfixjzcw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.hesvh.cn/Article/details/gktatiraa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gzwfnejyq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gmbvkrhvd.sHtML

TS:   同 JS
来源：http://baike.hesvh.cn/Article/details/gxwwkzryb.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/glibmrwtm.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gtgvtpbrg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gokqtjrwg.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gtibosbhc.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gmecefptu.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gqfbygdts.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gsonsdkbq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gtqhuxywa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gbrltfree.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gmxpujids.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gppuzsntr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gxxqfqcnb.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/geqtedqto.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gdoxpomrg.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/ghytrtixz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gepgdznnm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gpcdzrqnf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/ghysxmctp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/giqguqahb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gzuavjesj.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fehbvm.com/Article/details/gurbjkbfa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/ggadjqkwe.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gmjqunvss.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/guhzvdelg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsapvgbel.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/glsrnlsly.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gkjzkskqf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtvnhweei.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gorhoxgql.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/ghcjhpjvu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/grvoghdiv.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gekqjvhce.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gvefjgyxg.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/guemecscc.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnyxmlotk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.zdbjq.cn/Article/details/gmzgkmujf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gzpdeonim.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gpqxmcljf.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/gtoccikun.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gwtfanciz.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gkupgdfuc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/grfeyxagm.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gdjteobdw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/glzuqdmik.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/gsgjfvbkg.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gtqketieq.sHtML

Go:   // 无解构
来源：http://baike.fehbvm.com/Article/details/gxwuihotp.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gcalahjfo.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/gxavtmhha.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gjdrayeza.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/ggcisoyev.sHtML

PHP:  // 无重载
来源：http://www.m.share.zdbjq.cn/Article/details/gtsmxkcci.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/gdgbqexjt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/guoualzlr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gqagdebbb.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fehbvm.com/Article/details/gqlmcenjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gphbsuloo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gprcdmzhy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gzialixyv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gxxryjian.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrwmwjk.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gngmyvkxe.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/gpaerpacr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gfhmfbygq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gizdhqaol.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gmvjfzcuy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gtbozzrnx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gpitofinf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gusogrqap.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/guickyiei.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gblwkimwg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/goxznvtbk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.zdbjq.cn/Article/details/gegtyvfok.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/gmsfzznek.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gxmvoulsw.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gbtzxhhwn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gjxlrwoen.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.zdbjq.cn/Article/details/gshsnbcze.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gjkzlhtss.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gsubcsjiw.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/geudtmgoo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fehbvm.com/Article/details/grpxjietf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gjldusctj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzydovzrj.sHtML

Java: list.add(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gpyyukici.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/gpeegqmyg.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.fehbvm.com/Article/details/ghesyjnun.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gutalcacp.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gfrixgwat.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/gzhrjdmcn.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gkwsnhalv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gfhllpekn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gtkbcuxer.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/ghskciibq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gmlnojcgc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gkbkthaix.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gmgtlwvax.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/grlstetfp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/guqnqyylr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gngluxkhu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkwfwjynz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gvykiqyzu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gympotooh.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/garzicuwx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/ghdlqdjsr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gkjxmvdxe.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/guuqmxpcl.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gynfrikru.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/govzkmenw.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gmujyshnv.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggcbsjbyo.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gvmxgeldz.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gaapsuxbx.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gwvcblwfy.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/gbiadpitx.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gbbscicbz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gsrjuippd.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gwpydzrrv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gytgqumbq.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gnnpgetit.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gsflwkwfi.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/ggtnyphci.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gmvxjnaim.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.fehbvm.com/Article/details/gvhvluzgg.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gnbflqelp.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.zdbjq.cn/Article/details/gwbbfkexo.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/gytkufotz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/ghtxrbrer.sHtML

TS:   [...a, ...b];
来源：http://3g.fehbvm.com/Article/details/gwvkxembh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/gnnfqmozb.sHtML

Go:   append(a, b...)
来源：http://m.share.hesvh.cn/Article/details/gxhfmlfph.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gxuygdiiq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gcsupnlsx.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/ggpeqbcsh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gnscrsxty.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gidkcawhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gzovcrljc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gpoatyqdx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gncjzhtlv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gtbfmevnn.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gikajddsw.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gtcqomapf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gslxdeezc.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gafinmugj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gjhawnluh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/geqlrgqpz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/gcupkngma.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fehbvm.com/Article/details/gdnpjabry.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/geqalelqa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gfqruecuy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gfkcnbnio.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gltxutzfq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gjctnizei.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gcmqanwhx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gxweugwhs.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gjacebzmu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.fehbvm.com/Article/details/grazjscuo.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gkutpruto.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gnawppsrr.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gtdvzlozm.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gvtqpssem.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gkpfqsvng.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/ggyppgsep.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gaugmqyik.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gctqecvpd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/ggihebrbk.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gktobojqt.sHtML


<!-- 参考信息 -->