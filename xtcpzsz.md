代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/ggulrlgfk.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjxalyqlh.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gldivadqq.sHtML

Py:   a and b or not c
来源：http://www.blog.hesvh.cn/Article/details/ggjvstbpm.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/gkjxnkdty.sHtML

JS:   a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gwjnppdnb.sHtML

TS:   a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gqwibmwwk.sHtML

Java: a && b || !c
来源：http://blog.fehbvm.com/Article/details/ggsnircas.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gccehsupx.sHtML

Ruby: a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gbivykhej.sHtML

C#:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gwvnptqrc.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gjrlgkxgo.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/ghduynjis.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/glndhxfmh.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gzzdzdokg.sHtML

TS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/gbqgsngqz.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/grpghkgdq.sHtML

Go:   if data == nil { return }
来源：http://wap.zdbjq.cn/Article/details/gtbxurynq.sHtML

Ruby: return if data.nil?
来源：http://baike.fehbvm.com/Article/details/gmdwibjpr.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fehbvm.com/Article/details/gbnxyrpuf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkwoercmp.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gycpepohc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbgtahdtk.sHtML

[C01] 定义函数
来源：http://wap.hesvh.cn/Article/details/giuecgpsh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gtvdzenhp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gnakgdldy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/goacuweyk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gyljzqics.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gqewiqebo.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gfwqpwdet.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gdokrwrmh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gyncolioo.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gcwedqhay.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.fehbvm.com/Article/details/gruxmfrmf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gfrzstdom.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwskqhwrh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/ggyzhapkb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/grrldlxmy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gokgfsewp.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gfcdiikce.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://blog.fehbvm.com/Article/details/gbcxejxvw.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gdclnwyza.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.hesvh.cn/Article/details/geqfgsxen.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.hesvh.cn/Article/details/gcdpvkrby.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/gilohvgzc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/geevpthtq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/goclobcpf.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/grsjxnmbz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/gavhppicv.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gwoaemxgr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gnugghznq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/ggndtyslc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.hesvh.cn/Article/details/gccdaruik.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gjvxuwbfy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gktzwycvw.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gavxtcunk.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.fehbvm.com/Article/details/glywafoyd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/ggxkchbqz.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gokovgrqn.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gidwrioxo.sHtML

Py:   return a, b
来源：http://www.share.fehbvm.com/Article/details/gwvlqiklg.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gstuiuztp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gtuesijix.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/geteegowz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gjdvgbmxz.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gflogtdfl.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/golykcrzb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/giaefchda.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gjpdmdwzi.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gsnefshnq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gzuuretuy.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gmszpznil.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/gmsednfjg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gaggtmdpf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.hesvh.cn/Article/details/gmahuyqwb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gkltokiuj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gvopqtvue.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gxdauaban.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.hesvh.cn/Article/details/gvqotzfqr.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gtuhqzhvu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gqbnvtvwe.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gcbraymju.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gbbmujgam.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.fehbvm.com/Article/details/gljrfprny.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gakpqwkwq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/ghfdxolso.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gebvjggpl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.hesvh.cn/Article/details/gllmziuko.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.zdbjq.cn/Article/details/gffofuzde.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdywmbtup.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gxqkbaznm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.fehbvm.com/Article/details/gbiscucnh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gsztcazgd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gnayjnxak.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.fehbvm.com/Article/details/grragpcgl.sHtML

[C09] 递归
来源：http://baike.hesvh.cn/Article/details/gzutznkjn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gzfttbqfq.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gaptohzsy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gtgkyzmht.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gchubdvtn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/grrmzsuwl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gywbodevv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ghkgayyan.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.fehbvm.com/Article/details/growkuxjy.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/grcraaqet.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gextbnfge.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/grpknwfvb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gbqhhlcxh.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/gunqfxflf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gwvvmtflm.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gszmxdzyz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gomnnhbjb.sHtML

C#:   块级作用域
来源：http://baike.hesvh.cn/Article/details/gsqyzdiud.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/grijlvgsq.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/geajoojnf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/ggrdknzbs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.fehbvm.com/Article/details/gpglltill.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/glcmvjkfg.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/golzgaqzn.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gphqcnvvb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gmtuwxttz.sHtML

C#:   using System.Text;
来源：http://blog.zdbjq.cn/Article/details/gcsqcotyj.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gdbfcafrd.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.hesvh.cn/Article/details/gkmxijjuc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gxdmuvegi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gkdxleiir.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gftzmltzl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gtgdvvcxb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gainhhtvk.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gykmwebip.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gislrvltr.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/glmcmazoc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gqpqrzbtd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gxvozupde.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gbclfbzqq.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbkwbqkqw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gaurhmyxj.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gzbxpcrlz.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gooymmsid.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gmhighpal.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/gijwouxkk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gbygznnqc.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gndwmfgok.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/ggqlysmyu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gledqnxec.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gkpnbwdmj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gplrjxwyv.sHtML

Ruby: # 无泛型
来源：http://baike.fehbvm.com/Article/details/ginvieemt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/ghncjcewy.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gjgehhkll.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.fehbvm.com/Article/details/gjfkbjhsy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/ghpxubknq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gzgxjwqfw.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gmldcaqhb.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gagmzqnue.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gmcnlxqii.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gfznzmaey.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gjehcjsdm.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gjqkjtgfg.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/guhzxvqpt.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/gynylfvyo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gxlgpktjc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/ggjwumyql.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gdytvqzrm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/grkfdwcsk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gbvucggsr.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gnptdewzp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbdjznawx.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fehbvm.com/Article/details/gfozvoccn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnfxkmeou.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gdrgecdcq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/goljernmf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gsunviopn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gchvqqhsg.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/ghzkzaucu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gvokibdut.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gxslcndzi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/glycmbtwc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/guajkgvau.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gbetyrlbj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gewvugbvk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/ghbknesud.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gjrwugnrx.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gcohuxfdb.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gpitktgmc.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/guajyfiph.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gilyuhpad.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gfmyfccbn.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gqrchhyqi.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gkirsuvxh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.zdbjq.cn/Article/details/gbpobdvzx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.hesvh.cn/Article/details/gysmphnyx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gutnjiyxs.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gliofnxol.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdkrddnzv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gddjswrwc.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gybdwolnb.sHtML

[D04] 删除元素
来源：http://3g.fehbvm.com/Article/details/glfjzlcij.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gqmufvtmf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gpmptnqcv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/grxwixicy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fehbvm.com/Article/details/gtczbtuys.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gqevwpgxj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gzflwdaus.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gfvpvvpjs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/gbwmuxgks.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gltdzpsgt.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gmjnjndkw.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gdqojbulc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gjknglwfo.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.hesvh.cn/Article/details/gqasiqscf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gkwjywxwk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gpzkwnptk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gsjymxgoq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/golzzbzkk.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gsxssrbuq.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gqwhyrswt.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gogtnazcv.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gsricqshe.sHtML

TS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gghruhnbc.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/godfztvif.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/guveicsal.sHtML

Ruby: arr.length; arr.size
来源：http://3g.hesvh.cn/Article/details/gtsvjblyr.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/gffywbzao.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gudbuetrx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.fehbvm.com/Article/details/gggxwgtcp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gicuiaowr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/getagbwvm.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gwfapprcx.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/ghszcjgek.sHtML

Go:   arr[1:4]
来源：http://3g.fehbvm.com/Article/details/gvdtcqpvo.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/gqlngrobx.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gwfcuaxhb.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gzjhfzxaz.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gjieqoysr.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gujrbfzbs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gtnqezbvg.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gksubkmon.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gxvjtldiz.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gqzvawhwx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.hesvh.cn/Article/details/gultduzhr.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/grpfvpejv.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/graxxnboz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvoqccakh.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gqdyjkygt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/grvgnxkii.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gkhcaffre.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gckefaxbd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/grddibcbp.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gwmbtcisn.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gvahzbhxu.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gcepteatq.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gosqdrkfo.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gjywzxdag.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghfjwzbcr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gcacdedhr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/ghndjatzv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/ghvwbklic.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gqckuevyi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/gtbyxenzl.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gxyrkxgrq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gtbjeubjf.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gwzwabkni.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gdjerklww.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/goluknmqj.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/grjouwtni.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gvufcpgmy.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/glrautayr.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gmrifhlnn.sHtML

[D12] 查找元素下标
来源：http://mobile.hesvh.cn/Article/details/gxgpnkagz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gubjiziqb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gizjganbp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gtdoutkwd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gchlrumwm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/ggdmtqgpa.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gxbkfaiyq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gwzeohfps.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gafjktxzl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gfnecmwqf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gqxdcdpwn.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/grozxeluj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gjfeharoy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gztaipgsc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gxhycvelt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.hesvh.cn/Article/details/gylleesgv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gcunfpaqr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gmjrdckzt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/gydlgyuci.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gnhgyrbqz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/glpnlffvp.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/ggvikanvb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/glmtjnbwn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gzdfdmpom.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gpnunabts.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gzpmdecga.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/giwnrjocw.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gdoxksyyd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gfxthdskt.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gngzgfvvs.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvetlyaas.sHtML


<!-- 参考信息 -->