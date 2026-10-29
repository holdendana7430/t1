代发 wailian999

Py:   if not data: return
来源：http://wap.fehbvm.com/Article/details/gdaopggfk.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.hesvh.cn/Article/details/gspdeckfm.sHtML

JS:   if (!data) return;
来源：http://blog.hesvh.cn/Article/details/glzrnnnyc.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gtjkfizac.sHtML

Java: if (data == null) return;
来源：http://www.share.hesvh.cn/Article/details/gtolmohio.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gziivjlen.sHtML

Ruby: return if data.nil?
来源：http://www.share.zdbjq.cn/Article/details/gyvsevjwl.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gazsjnpsi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goowpybxo.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gabvswcaf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/givrdfrwy.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/geefcdego.sHtML

Py:   def add(a, b): return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gqjcgppdx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjoevcopa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gygetitaj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fehbvm.com/Article/details/guyczbylr.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gvgcxurxv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gxfmhfqfy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/goewxwpui.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gigrnomdu.sHtML

[C02] 默认参数
来源：http://3g.hesvh.cn/Article/details/ghdjmuqbz.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fehbvm.com/Article/details/gynotrpbl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gckdqgxrz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gllubqhrt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gpatslcwk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.hesvh.cn/Article/details/gmocorrny.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gibzyrpdg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gjmygzkpb.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gczarjbch.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gcurvgrxx.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gvxnzckpp.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gxeysamiu.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gbqlflzux.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gwqjtgtkv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.fehbvm.com/Article/details/gmwidfaan.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gghilyuof.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gtddppehc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/ghplyyscx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gfrofbsvx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.zdbjq.cn/Article/details/gvzqnrkmy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gkmstxraj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gnaxbixzq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/gnoebexea.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.hesvh.cn/Article/details/gnljcaxmc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/ghvuzpgac.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gohpdhxaa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gjetjcmdk.sHtML

[C05] 返回多个值
来源：http://m.share.fehbvm.com/Article/details/grkwuhvek.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gpkgavzrl.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fehbvm.com/Article/details/gbryzmete.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://wap.fehbvm.com/Article/details/ghovixkca.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/ghkrflbgl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gjpxweepu.sHtML

Go:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gadrkssxi.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gbozzifqe.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/ggjixqevt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gdziqghdy.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gatzswgms.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gthvkfgmn.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gznoqphcm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gdhdipavo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gnouxuljx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/geychdprn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gffgmqphp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gevwrkuzg.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gogrlkvxe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gilxafbhk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.fehbvm.com/Article/details/gijgarnhb.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/glgnwqpsl.sHtML

TS:   arr.map(String)
来源：http://wap.hesvh.cn/Article/details/gupwuxvdn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdqslbwej.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gsucvruvx.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.zdbjq.cn/Article/details/ggabecqtu.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/gajqtbhwm.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gjcxwgxbn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gextrsnse.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gnottmlle.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdnndfzqz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/godauanuz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.hesvh.cn/Article/details/gohxspeuk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gpfskdnas.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gdwgldjkm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/ggfybyyqg.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gelrzyoeb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/ggggvuapg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gzhjulxqf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gpzzezkpc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/guxrfgwdb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gqnyarglp.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gcewjvxdq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxiujnvim.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxdxftdym.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/ggzgnafal.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gyfpbfogk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gafscorfl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gdvtolpuq.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gffpfnzav.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gmvcaiyuq.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/grissnzwm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.hesvh.cn/Article/details/gijdonkpz.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gimtthwqv.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gqogwufbg.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gidsvdhan.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/gexcparmg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gjcxevlpd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gzemwnylk.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gqctvazfg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gdjovjhcq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.fehbvm.com/Article/details/gigcisxyh.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gzmbifufd.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/goaexkthq.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/ghdkwznqc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/gtcrtqbkg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gcqrxhxgp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gticbvrcd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/ghrcteuro.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.hesvh.cn/Article/details/gkxstoasy.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gkkraygtu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gggopwthc.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/guqrrqrjx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/geqnbyqrs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gedfcgzaj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gngrlvdcd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gtzzywhrg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/glennirpq.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gvkwabegd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/ggfvbmwqx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gveziwpqf.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gsnoilxlx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gtpjsatfe.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdytdywhs.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/gcizmzvba.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gkpagbuoz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gsvvghldl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/glrgklybl.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gjwhyjqcx.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/glnjsonfx.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmmvlctcb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gonezgvvr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gwbxxvqco.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/glzjhbynh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.hesvh.cn/Article/details/ghwsfvibc.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gnuopybak.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/gjkuycytr.sHtML

Ruby: a, b = pair
来源：http://3g.fehbvm.com/Article/details/gwxyzjayp.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gdxjnlqym.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gwgbdolmi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gmjwqxllz.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gzknkpdgx.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fehbvm.com/Article/details/gjdzndsrg.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.fehbvm.com/Article/details/glvhehbfl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gfokowzus.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gvmzktvai.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gvatgkobh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.hesvh.cn/Article/details/gcbepoxgp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gztxkfqzy.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gvdjwbwiv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbmeiwubu.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gfayttaqi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gunsprxqo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/ggmwpgdkc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gzmjzjzcq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gdxyqsyuo.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gfnoxfrao.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/ganilakne.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gnvrkivrx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gclljoife.sHtML

[D02] 追加元素到末尾
来源：http://m.share.zdbjq.cn/Article/details/gxzlsqmbm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/grcsxflvy.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gkijrzsvj.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvrgypyvu.sHtML

TS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/ghrbvhxga.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gmqjbxpfg.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gzvrphpfe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gdustqevi.sHtML

C#:   list.Add(4);
来源：http://wap.hesvh.cn/Article/details/gterzckhp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.hesvh.cn/Article/details/glzycewap.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gexycoezh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.fehbvm.com/Article/details/gpsrreiaj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gqcicksnq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzlvxuobq.sHtML

Java: list.add(0, 0);
来源：http://3g.fehbvm.com/Article/details/grvlhxrhb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.zdbjq.cn/Article/details/ghzpqcsmo.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/guhkpxqew.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.hesvh.cn/Article/details/griztorsb.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gqhygibhr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gftvcqfkl.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.hesvh.cn/Article/details/glgwzvezp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gwjyesevd.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.zdbjq.cn/Article/details/gczkcsnvq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gempxqfcm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gsqzqnkdm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gnhggcgdl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/ghxeosnxw.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gjtuztkek.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gkwvuuava.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyijzljii.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/ggbvwlsjq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gopmoaxvk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gawulmfkr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gsuezxpxp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gezzszllc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gzniifdke.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/glxfbhidp.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gokxxisxz.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gjktfpdcg.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gtltftybp.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gczhkryfc.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gjfnplioe.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/ggnanhrax.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gxyyqhkmh.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gxvjvsikp.sHtML

[D07] 切片 / 取子数组
来源：http://wap.zdbjq.cn/Article/details/gdqoplwxz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gksrjgiao.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gceueepwd.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gbzbtdrlz.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gtctbmezk.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gyucunbef.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gxvtchgju.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/gpbsqmbmm.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/glzxeroap.sHtML

[D08] 合并两个数组
来源：http://mobile.hesvh.cn/Article/details/gcwuaezjd.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmyhxfgeh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gdcdwbqtr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.zdbjq.cn/Article/details/gegvottti.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gwfagmags.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.hesvh.cn/Article/details/gntnmknrz.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gldkmzvoj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gibidjglj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/gbbpzpxkx.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/glzeixcej.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gsnyksuei.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/grkggnpfe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/ggqsnunot.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gyjxyfisn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gdlynpmgk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ggfbqaqga.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/ghzzxqtpn.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gmfwtaucn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gdkmecmpb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gtfgeimbh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gdcbhwwdr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gdsostobn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/goctrcnym.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gfseaqxcn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/grfmjgson.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/godtpybuu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gxrgbtwtf.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gdzivsrnd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/giyrjdfgc.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gunrwzygh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/ghcdsbekw.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gpyguundk.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gtlwcsygc.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/ggoaphhec.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gbtjkniyw.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gtoovgwnf.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gfjamjtgf.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gfubgjgcp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gulmjxapk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gdzvlanmx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gofpjgvxw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gsfmmtyrc.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gfehrklsm.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/gghtftfoi.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/ggrsygvqg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gzerqosbu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gbopbgiuw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gasidpucq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/ghnzoaiel.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gacgsvvro.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gwwrbidgb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.hesvh.cn/Article/details/gorbrkyyi.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gdnsfamoh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghmsqgsrn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gazzirczq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gzcdzzlqn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gzaowfedr.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gvrmzevzq.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/guktanhed.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gozqtliyd.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gyocsibdr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gcmvwvhqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzebocrxs.sHtML

[D15] 去重
来源：http://wap.hesvh.cn/Article/details/gnwadooay.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/gfdzmebyg.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gguyftefc.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gneznkxmc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gyqedyyej.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gswnhjntb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gnqybdrsm.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gihzfipxh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/glyuccsrq.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gtaakvsgb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxngpgzkt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gwqzktbjj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ghofdfrxu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfjlbjgdo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gebdfaxzm.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/gahrfdlrz.sHtML


<!-- 参考信息 -->