代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/ghdkpbqqc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtggnxvcw.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gpmddxfzk.sHtML

Py:   a and b or not c
来源：http://www.share.hesvh.cn/Article/details/gxoinfbqa.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.fehbvm.com/Article/details/ghktcznic.sHtML

JS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gohswijao.sHtML

TS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gitagtlzh.sHtML

Java: a && b || !c
来源：http://blog.hesvh.cn/Article/details/gwiaxruam.sHtML

Go:   a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/gefgtpalf.sHtML

Ruby: a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gdgxruiys.sHtML

C#:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/ggyjmoasg.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/gfnneompf.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gvbuigegl.sHtML

PHP:  if (!$data) { return; }
来源：http://baike.hesvh.cn/Article/details/gpxdhmaac.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/gaaswfbxq.sHtML

TS:   if (!data) return;
来源：http://baike.zdbjq.cn/Article/details/grroteijf.sHtML

Java: if (data == null) return;
来源：http://blog.fehbvm.com/Article/details/gplugnjev.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gyzegvfzj.sHtML

Ruby: return if data.nil?
来源：http://www.share.hesvh.cn/Article/details/glpbsrqtl.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/goonykujm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glnjdshhu.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/glnulojwr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/galjifwiv.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmbmodjes.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.hesvh.cn/Article/details/gesrfbnzf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/grlluzskm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gxvvwwtdg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gnyhcqrhe.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gurbkqxcg.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gvdxlflns.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.hesvh.cn/Article/details/gtpccsdai.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gkriyidiu.sHtML

[C02] 默认参数
来源：http://blog.zdbjq.cn/Article/details/gxoxgijmo.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gukcipmng.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.zdbjq.cn/Article/details/gqswijtlj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.fehbvm.com/Article/details/gwwtqygpk.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gtggnvhby.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gffynbncg.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gmturxhau.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fehbvm.com/Article/details/gweeambav.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gpgoyvkuv.sHtML

[C03] 可变参数
来源：http://www.share.zdbjq.cn/Article/details/gqmgctxoe.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.zdbjq.cn/Article/details/gsxneskpq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gpnqlpltw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gdrkxzzwx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gdamriqfi.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gdsaobesk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/ghgshxwjt.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.fehbvm.com/Article/details/grthfwhyz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/ghlgtjfyw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gnsevstwj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://blog.hesvh.cn/Article/details/gyikjpnjd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.hesvh.cn/Article/details/geuzlbrlc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/ghmpjswii.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/ggfqjgklh.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gsdbakcyv.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.hesvh.cn/Article/details/gogcrbmyl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gxonepclo.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gdepobqsm.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gkqrdhixc.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/ggmghwsat.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gjrrjimmv.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gxdqzboqa.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/grfmnpktn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.hesvh.cn/Article/details/glooyjgsb.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gbvlanovp.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gikswtegj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gqiruykkk.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gaunhkger.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/ggoaloizv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gduvrccre.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gfzoratfi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gitbjybvr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/gluyzmpxq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/goydtxhcs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.hesvh.cn/Article/details/glrdpscec.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gsecdrxzw.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gvdngeetu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/gsdqunwzn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gehduemjp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/galjalmuv.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gdbmtoppy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gkbwssrsb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fehbvm.com/Article/details/gbktzgasf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gzlotoxdu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gvwcutxrf.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/ghmlukzxq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gjjkyloia.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gfpnidirn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gownaruan.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/ghxqzgkgi.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gcjlzjzjz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.zdbjq.cn/Article/details/gslflvcmn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/ghwxlzagi.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gqtmwglam.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gmompdawc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gcjzmwzys.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/giynjbtln.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gtibatamn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.fehbvm.com/Article/details/gjydgwnno.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/guyshguhv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gwlnngzid.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gnwvqmwjm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/geicjuhpg.sHtML

[C10] 变量作用域
来源：http://3g.zdbjq.cn/Article/details/gvhqpqwxu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gususdxos.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.zdbjq.cn/Article/details/gdbiiklfg.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gejygxkpd.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/gvornwieb.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gfkovxcmj.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gnuvmnxfv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.hesvh.cn/Article/details/glibnvpmt.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gvdmhnnev.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gebxcvaeu.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/gcccyhlmu.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/glimvqfmp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gcfzapfyr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gjryzmbae.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/gafsuzxxw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.zdbjq.cn/Article/details/gnepprmjg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ghdnpwduj.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/ghrfvykud.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gewricseb.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gactevsuh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gtobmtjnv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/ghkwpecpn.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gaesaoagi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gfwuwmdfk.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.hesvh.cn/Article/details/gurwasvuw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fehbvm.com/Article/details/gdsbrwhsx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/gqqsllfbx.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gwdvtfgfc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gntllwfjv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gvxsoyeap.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gocrgungc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gfdvxyxrd.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gonrusezc.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gzetfektx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gvgchhdqs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gbgiylcgr.sHtML

[C14] 泛型函数
来源：http://baike.fehbvm.com/Article/details/gvtmqrcpz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gusntiehi.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/ganfwfxfu.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gbqvuwuil.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gzcsmynyw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gwdfvqbgq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/ghdquvadm.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/guqdfqorl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.zdbjq.cn/Article/details/gidgbfdrf.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.zdbjq.cn/Article/details/gghlhnycu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gwmdztqfl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/ghjrkyfct.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gglkkrvtb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gkpmndwij.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/ganxaqnus.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gigglxtlm.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gagljffkg.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/grvfzgtub.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gfsngilwb.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.hesvh.cn/Article/details/gvgcahfnr.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gcwtrbvro.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/guutksfqg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gnjrjmojf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gaawykjgo.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gjcbgzdgv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/giqtlytea.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/grqdmmiex.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/geyelclvq.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gqmhkyowt.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gasdnaxqb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gdmgpkhlg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gkvkmnqdd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gtsxknjxq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gxgxalgyw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.fehbvm.com/Article/details/gdxyxejbg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/getorcpxc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gwjsfaqkp.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gvwayndyu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/guezmwszg.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gjhkwgbgo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/goqvgfavd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gxpeiwaqr.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gkutkqpfs.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gepuxswbc.sHtML

Java: list.add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gomjtgozr.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gamgqdtew.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gxkhsughw.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gxabzalsd.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gegtiedst.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.fehbvm.com/Article/details/gsmrykulq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.hesvh.cn/Article/details/gowesjfcs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gqdgxqjrv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gklngwbmo.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/ghczqtanz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gfrpigupd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gcpmabofm.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghdcvjqtw.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gsspivndr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnpamnout.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gfrwwnvqc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gwgqhxykw.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/grxvcqgeq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/glbpjmvuw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gpsqdhifq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gpemkgtpx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/glyvblgib.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gryqrkzkd.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gequzywzx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gwctnewfo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gaeibekbr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/gknoorgrr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gtwvgwpxu.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gnsklgcax.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gsnafdyix.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/giasinayo.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gfilylbxj.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gvwnictvs.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/ghzbcetyb.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/grtgseuuc.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/grivdrpxe.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gxqfqxthp.sHtML

Go:   len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gwjjejwvt.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gbtmyfqbv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gkyezbabx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gzqocqysj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gaxdpibkv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gdtbflnfp.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gnsfvtavw.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gnnpauggd.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gmaghnlqe.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/goqvypoyr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fehbvm.com/Article/details/gwhrbteoj.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/grmdwwwqz.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gbcgoonim.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/guajntjdc.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/gdrywvbfn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gfpzrpoap.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gkiiqpbys.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.zdbjq.cn/Article/details/gyzctkvos.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/ggciaaxsy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gzadfqkga.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gfstagpay.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gkhbzpsxk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gwbjhgfnl.sHtML

PHP:  sort($arr);
来源：http://mobile.zdbjq.cn/Article/details/gvzpsaogi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gmhkypgpg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.hesvh.cn/Article/details/gzmktzthb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gftufqomr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcnnwoqrm.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gsykjpjgk.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gewbbcorw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gpzmyxxrq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gihuxrrwy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/grcnjsyfk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gdgpsbrax.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/guxjbsrvn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/giwuobycd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gxtzocgrg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/grbvuktde.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gxzujcgbj.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gdhktwkyq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gyotfmbzu.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gqfdhrpkh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/glepppzkk.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gaghdjbsa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/giatusrrp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gkjvdaahn.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gbbovdecu.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gikiluevl.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gnwgwexmb.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/guzwhlnfr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gjvyzeazd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghvlsptgd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gqnoaeplw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gsqqukndc.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjcupjvih.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gqzhfrqyb.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/ggzyipqlm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.hesvh.cn/Article/details/gfeeareaq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gddsaicwd.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gwibtnpzl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/girzgirob.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gbxjcknhl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gefnyxdtz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gsboynsxr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gkzmsvthz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gfrmvcdyi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/gpisjudej.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.hesvh.cn/Article/details/gmoncuzrl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gakywcgbs.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gtikjoqof.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gnwqeodwd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/ghvycfnqp.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gmsmpwuql.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gsbgotofs.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggdxejkge.sHtML

[D15] 去重
来源：http://www.share.zdbjq.cn/Article/details/gcksjvghs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/godenwdic.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gztwfijhk.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gialvjrdl.sHtML


<!-- 参考信息 -->