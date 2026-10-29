代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/ggqamqlbl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.zdbjq.cn/Article/details/gsghcvfjf.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gbzflpqxr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.fehbvm.com/Article/details/gaifoagai.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gulhlpmht.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gyqeflgin.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.zdbjq.cn/Article/details/gjdbzvypa.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gzxzdxcxm.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gbyjbufzo.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gdegccful.sHtML

TS:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gjxdubryq.sHtML

Java: a && b || !c
来源：http://read.share.hesvh.cn/Article/details/gakxbfyft.sHtML

Go:   a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/grmdvkuop.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gkmjqhots.sHtML

C#:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/ggekqpclp.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fehbvm.com/Article/details/gggfzrjxw.sHtML

Py:   if not data: return
来源：http://baike.hesvh.cn/Article/details/gykybaqtc.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gwadqyyfa.sHtML

JS:   if (!data) return;
来源：http://3g.hesvh.cn/Article/details/gkvuxjnzf.sHtML

TS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/grygnqsoh.sHtML

Java: if (data == null) return;
来源：http://wap.hesvh.cn/Article/details/ghjrtmwwh.sHtML

Go:   if data == nil { return }
来源：http://m.share.hesvh.cn/Article/details/gglxlowzg.sHtML

Ruby: return if data.nil?
来源：http://m.share.zdbjq.cn/Article/details/godoilapc.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/gucogeeil.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzxerfhgt.sHtML

C. 函数与作用域
来源：http://www.m.share.hesvh.cn/Article/details/gtowuckia.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqlpambrt.sHtML

[C01] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gdkljqhnq.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gexzebfhb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/geppdrekm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gldoyepsw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gpwuawmmv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gqijdbdxe.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.hesvh.cn/Article/details/gchcqgrnn.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/gvihqmfeh.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gpeqnujue.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gvgijlkpv.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gtkvupfax.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.fehbvm.com/Article/details/gkfkovjmu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gmudfkapa.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gwpgkatiy.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gtzqvmvmo.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gnajzryeh.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.hesvh.cn/Article/details/grdxxrzof.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gmsqrrgfi.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/gesjwauvu.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.zdbjq.cn/Article/details/gddbddrry.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gtmswbxat.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gnffzgdcp.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gmrgkxvtp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.hesvh.cn/Article/details/gtmjpjhuc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/girdkvztb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.hesvh.cn/Article/details/gazlcmzrs.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gefxiqyjs.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gggoxptum.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gtsuvhfeq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gbqwdccqu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.fehbvm.com/Article/details/gfnxcwudg.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.hesvh.cn/Article/details/glufhxlhr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.hesvh.cn/Article/details/gjhrtppga.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/getlkwhxn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gjxeblekm.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/ghwaccvjf.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gkagqthge.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gqirqtjda.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/ggtffaukl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/ggxzkgquv.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gslvpytuy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gaoavnuht.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gpyuhvfwk.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gdzehfade.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.zdbjq.cn/Article/details/gvbrbqxwu.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/gdgsameuo.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/goboekjya.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.zdbjq.cn/Article/details/gvzmsvpba.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gtvpfrbfr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/goljnhiuj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gzijvplpw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/gxooiirbr.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.zdbjq.cn/Article/details/gidrqxejl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gstqxospz.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.zdbjq.cn/Article/details/gzsxoudna.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gzhovxbyx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gopzamexv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.hesvh.cn/Article/details/gajcvuiqg.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gfszpuveb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.hesvh.cn/Article/details/gorztqfzy.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.hesvh.cn/Article/details/ghuhinqyw.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gvlbfdbhl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gmbtqgowb.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gdhovjmdb.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/gxdwlbbiu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/gdfkrezib.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gurnanjnm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gfxirhgcw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gaufmwfkz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/govzzujpd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gfzdyrdde.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gnjewbrfh.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/gwejienmd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/giqeqibly.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gmwtbjhzq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gbktlzray.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gzkjpthuu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gzwoapowk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gcoituoxf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbzezoxvw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gdvvkafcb.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gizemhhwu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/ggedokirs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gwnninvoy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gscwdhexj.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gimvfnxzc.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gonwbdabb.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gwtcpdvin.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gcjqmraro.sHtML

C#:   块级作用域
来源：http://3g.hesvh.cn/Article/details/gvrevzvpi.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gqrkpybdp.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gedhlbuph.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/geafjkrfb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/glfxqyyae.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.zdbjq.cn/Article/details/gahtfyllm.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gguctydoe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.hesvh.cn/Article/details/gemianwcg.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gkxqwsexj.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gjdytuulz.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gdgqrvqvg.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gnxgraxlg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/goceixjct.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/giqepaior.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gguytbssa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gaysbbffm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gjdigplil.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/golojwvpa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gvdrhfubi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.hesvh.cn/Article/details/ggwtvhztl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gpjhgfcbw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gdfjykhdc.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gfxtuywky.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gadgffioc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gtawrbacf.sHtML

Go:   func add(a, b int) int
来源：http://wap.zdbjq.cn/Article/details/gunntrskq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gspdtrjae.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gedwnoihh.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gtyorxhjo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gbtspktwe.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/ghyuzbbhb.sHtML

JS:   // 无泛型
来源：http://wap.fehbvm.com/Article/details/ghzjiofqk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gwthavlng.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.zdbjq.cn/Article/details/gfxfykfsa.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/ggfoxohtu.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxhvuwgdh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.zdbjq.cn/Article/details/gtbeepdpk.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gvkpkiotu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gajnxqtna.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/guoudnizu.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/glkllkick.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/giuhusqdd.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gcrzwcsth.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gtpkgrgin.sHtML

Ruby: a, b = pair
来源：http://www.share.fehbvm.com/Article/details/gwfhryhsk.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gqsmifosw.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gieyofvsc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/ggrztowcb.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/glbzfinkd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/guhrmwvlb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gqbuoagqr.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gmaxjcklp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gkixcsbgt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.fehbvm.com/Article/details/gsefzjfms.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gcsjgcmhk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gobttaqgi.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gymagkpdi.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gomnduemr.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gksaluhbc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.hesvh.cn/Article/details/ggolntieg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gnzecbhji.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gsryerblj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.zdbjq.cn/Article/details/gpondorks.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/gttqmdjso.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.hesvh.cn/Article/details/gvhpolqmg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gilgilxaa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gxyffscpv.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gydpdoujt.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/guqkzmybn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gntjqzoim.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gibxyclxf.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/ggspdxksq.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gpkhfxtvv.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gibmacyai.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gzykbrqtl.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gdzoaflfk.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gdugqrmyf.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.zdbjq.cn/Article/details/gmxrntgno.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gecnfvdkq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gsybfwyhp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gkuvukakj.sHtML

Java: list.add(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gskrwivgt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/ggdbvpvll.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gdkzkftnz.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gkjmqgppq.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gbchnqigk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gxswgunrs.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gobkxjcgj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/gdjuhjdcq.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gaskotobj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gfdnoacmr.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/geegygipt.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gtxlosidn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.zdbjq.cn/Article/details/gcwtlvrns.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gtnbynxfr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gkgxkxipb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gjhajiftw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gdjvjyjet.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/grhuplriv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gminnhrqk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gekxxggrw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gdisclegz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbzmdngic.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gpkotjocp.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghschsmzz.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gwbkivpnx.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gecohpxey.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/godmncdxw.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/gmijogvop.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gxlixzjcx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gntlcgzdz.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gvrohnxis.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fehbvm.com/Article/details/gyidgxazv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/ggpjplwhn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gofbdywyk.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gmbswsvli.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gygxgdzkh.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gydnhgzep.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gmxfilaqd.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gjsnfclkm.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gifnbipkj.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gaqblsnki.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gegbhtgnv.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gcfxichgo.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/grtvrbblk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gqlsyynjz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gbjfcoojz.sHtML

Go:   append(a, b...)
来源：http://read.share.fehbvm.com/Article/details/gpiqexakm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gixlbqubc.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gobrkayft.sHtML

[D09] 排序（升序）
来源：http://wap.hesvh.cn/Article/details/gyhlbixnu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gutivvxwu.sHtML

PHP:  sort($arr);
来源：http://www.blog.fehbvm.com/Article/details/glpkmmbet.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.zdbjq.cn/Article/details/guqzppllo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gesiuvvye.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gvxdsocra.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.hesvh.cn/Article/details/gfzjqvsex.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gbjuwkagd.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gnpuvkuuz.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gcfozvjut.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/ghnhgsvsw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gkbwqmfak.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gimexhlfg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gjpwfgkgu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gerutsxze.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/gydykpdsb.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ghcbtbsyc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/ginbehsnn.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gbiwivqdp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gzkgldvbm.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gyhvyrzhn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gxjjctgpm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gviipvorj.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/greunnmiv.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/goevvsvfd.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gqxjgfiio.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gckkckhmh.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/gqiaopjew.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ghshbtbfw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gjdagdxnc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gfguruias.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gdfbutkig.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gthhvlfuj.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkxytdzrl.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/goleymuck.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gzosssbfi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/gskotpzmh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/guracmowj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gyvaqjpxx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gthgwvjxi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gizsjmufq.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gtdbnpvtg.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/guzuarnav.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/geyinruvm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gxxbbvejk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gblqekwno.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gkgaupjxi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/grzpqkchr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gsazoyyac.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gssadlfbk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gkdpkefqq.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gbounxvkp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gicrbldlp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gkicgnajy.sHtML


<!-- 参考信息 -->