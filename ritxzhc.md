代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://m.share.zdbjq.cn/Article/details/giuxdzotn.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gkpmaoyjb.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.fehbvm.com/Article/details/gueygkzbi.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gvpfxmino.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdbijiwhs.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/ggsdobthm.sHtML

[B15] 布尔运算与取反
来源：http://www.share.fehbvm.com/Article/details/gayppxjtz.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gbblulysr.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.zdbjq.cn/Article/details/gjmvhwdgd.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghqkpawez.sHtML

TS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkffxmiyb.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/ghbnqwomj.sHtML

Go:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/glthvrcja.sHtML

Ruby: a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gbrzdflpt.sHtML

C#:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gounmveay.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gwmlqodbl.sHtML

Py:   if not data: return
来源：http://mobile.hesvh.cn/Article/details/girmiymoy.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.fehbvm.com/Article/details/gmpfuxlqb.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gqmspxmfr.sHtML

TS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gzemrdeos.sHtML

Java: if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gqcgowgtv.sHtML

Go:   if data == nil { return }
来源：http://mobile.hesvh.cn/Article/details/gjeuqxoyh.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gayvrrcgf.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gdisokrbq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkavynjcg.sHtML

C. 函数与作用域
来源：http://m.share.hesvh.cn/Article/details/gycnyxqms.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwrpzkppg.sHtML

[C01] 定义函数
来源：http://3g.hesvh.cn/Article/details/gcitvvnjq.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.fehbvm.com/Article/details/gkmfesmgu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gfkxexnux.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gtcdguzxl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/glacwphvt.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gcryvhnup.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gdcxbhopi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gaapeynya.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/ggquqwehg.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gkvplsuqw.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gxyynmtnd.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gohkyvcnc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gxhajnwzx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grmyctrnw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gukkllzrx.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gjefrexmh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gfcrqwbck.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gjxqptyqk.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/grhommrba.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/guzoyjomm.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.hesvh.cn/Article/details/gktbxdfgp.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.zdbjq.cn/Article/details/guwqqcdik.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/giqbkepij.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gzivnwytx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/guvuxucvh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gthfqchii.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gyaraboht.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gzwqxated.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gwqjzrgta.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gicepfpzf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gekycdwgu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/guhywvjkp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/glohvhhig.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gzwzvzdxr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/glgshpboc.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gfcnffmlo.sHtML

[C05] 返回多个值
来源：http://www.m.share.hesvh.cn/Article/details/godtslrfn.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gjmphdfqe.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gamhtxfuw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/grldrovnt.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gkwjkdldb.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/gzykofyuz.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/guhjuogau.sHtML

Ruby: return a, b
来源：http://read.share.zdbjq.cn/Article/details/gwvyvvcpx.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gnkksbihf.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.fehbvm.com/Article/details/gudhjqpnt.sHtML

Py:   square = lambda x: x * x
来源：http://3g.zdbjq.cn/Article/details/gyjzzktsm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.zdbjq.cn/Article/details/gavmxtydr.sHtML

JS:   const square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ghpzzqjmb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gsduphcyj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/ghzpepnyz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gmrdfefhy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fehbvm.com/Article/details/garjxindm.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gpotomlee.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/ggqixqjfb.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/gotagnudy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gtowwsmbe.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gavdogdgn.sHtML

TS:   arr.map(String)
来源：http://mobile.fehbvm.com/Article/details/gzxxwunex.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gepmfenvd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/gkdtrkjce.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/glwaiwfbq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gdousaqqy.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gbekkktys.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/geobwezur.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.fehbvm.com/Article/details/gywmnghtn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gfaeeolsv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ghyrcvccq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gtaarivsw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gyindhdmx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gjpwuruoi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ghepewuhm.sHtML

[C09] 递归
来源：http://www.m.share.fehbvm.com/Article/details/glfdchpgr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gexzpsbrz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjipbnlo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gikzmryrd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/guelhbpkn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gyslyxjtt.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gmbduaeaa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gfatenput.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gyitrsgtx.sHtML

[C10] 变量作用域
来源：http://m.share.hesvh.cn/Article/details/gecvguinu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/gktshqmat.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/ghwhbsdjd.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gfklutdxu.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gekhbmmqh.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/goykjyjzi.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gahwrcegi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gaznsfvrm.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/giqxwwvxr.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gxkptzxty.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gpswdvmbh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gstxwayga.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gcazwwcfj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gdwyqeabq.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gnmpsjqoc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gptlgtfqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gduimnaaq.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/glzldcysl.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gbhfnafal.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gnnvwcknd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/guopxfjtn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gjxynncki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gkdxeicao.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gpatfhlvl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.hesvh.cn/Article/details/gugageuuq.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gtqpaqaph.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gxnynuuem.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gnshvhshm.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gpzwtnlql.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzlwowecr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gczkgeivb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gjypletqs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdtrcdecm.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gmfnbcexl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gbtsvudhn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gzqobhuvp.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gepjusymr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/ggiwxzqkc.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gnyrabjlt.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gkhfjccsq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gkwjcsnda.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gvoedcmic.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gpjnmkehg.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gqechybrs.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/gdjwcyayh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gyudxxlrb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/glckxynxu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gbwgkczbt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gqzcicgvt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/gkarakaxa.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gijwxhimw.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gjekvgogo.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gsakqsuhx.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/goylzffpx.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.zdbjq.cn/Article/details/gyhsnpqzu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gtkepehxn.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/grjzwqezl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/grswpnaln.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/gzjbyzhid.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gdkjcawzw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gmuyumtld.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gfeytbrcf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gyjdqewqa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdbuzakca.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gwyqbexro.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdefxosde.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gtdsefvpg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/glljllilv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gfwiwddxe.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gxetkaszt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gmsfcxugr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gsseavgcg.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gxsnhqepg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/gkdljxmdf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gqxccxmji.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gspqgdlxt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gzaygubma.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gmjklmoqv.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gjalfpzco.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gkhtayxyy.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gagdpjyes.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/guamcbqvk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gewkggksf.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/glwvjvbis.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gdblmhore.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gqwveiryw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gaerflrxa.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gqqmoxmir.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gkvlmikeb.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/guqdrevog.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gwyaucetf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gxbmbtobt.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gtrwlctri.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/gtieyqcbl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gfxubvmko.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gyrigzxhx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gvdqyxqcp.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.zdbjq.cn/Article/details/ggofyigrq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gwdviuorm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gqqwdjahp.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gyoofrcqv.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gucmfqjxo.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gnmdcamit.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grmxppwmx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwydynxex.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gootoqvno.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gxysihfjx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbepgohr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gflpqmhiq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/goezwturk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/grjzepsax.sHtML

[D06] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gkfcywzhz.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gntjxrbwu.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/gsebvjvdz.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gydhnzgnp.sHtML

TS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gpwpbjgfn.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gqlfolcst.sHtML

Go:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gemxxdncz.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/glilozlcu.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gnwelmpec.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gwuhnizli.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gfjypcnvh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gkizjnqcf.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gdcnndlun.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/goitcthfj.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gldwhqqmo.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gzckucvoa.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gvrapawge.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gjulratve.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gryyargpl.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gmsgoqgvm.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gukfialkp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gwkidsgaq.sHtML

TS:   [...a, ...b];
来源：http://read.share.zdbjq.cn/Article/details/gqvaxgmrg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxpwdsyet.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gqekaqbdq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/goxagsbem.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/glbkporsy.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/giczyuurz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gpccbzpxr.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gmdqxsvup.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/ggtwvysen.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gemqlvyto.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gyhwpzfzp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gomplxngq.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gzyfqefsb.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gjjifizjb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.fehbvm.com/Article/details/gxoptznii.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gokyssaxb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gbiyudpct.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ggrjiittn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gptzjfpjz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gkemzvowf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gezamtlnv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gewtgxraq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/getocdoms.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gbwmnolak.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/ginmnikfg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gjldiinku.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.hesvh.cn/Article/details/ghfqerdtb.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gytdqxtfj.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/grojxihef.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gkhglpfro.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gkeytxtdo.sHtML

C#:   list.Reverse();
来源：http://mobile.hesvh.cn/Article/details/gejarfbor.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gsbmmklzz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gutidpwob.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/guuegsqdw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gmnowryae.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gzgzsuaph.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gdcohhowt.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmmtkhzzf.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gzixcihsl.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gdiixqkwu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gelmxqogz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/guyshfeoe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gqxbeiqot.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gjqhqdatv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtfxtdizs.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gpvudwizq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gqbgvijqi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gglbbrnta.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gctfdqxxq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/gvqulycyc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gjwpebeqz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gayrvmaco.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/glgqmpvtm.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtepjwcdf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/grqfgylzm.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gcoigjayz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gensgmobp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gopkuxamm.sHtML


<!-- 参考信息 -->