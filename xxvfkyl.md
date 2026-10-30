代发 wailian999

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdqvqcsr.sHtML

C. 函数与作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gcijlzchx.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvhtcir.sHtML

[C01] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/givxutbvx.sHtML

Py:   def add(a, b): return a + b
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxhvhgn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grsxxlzgv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbtajlsri.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtukxweci.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grwpmlnjy.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteuspcpi.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gcpdyvxrk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goqitzldy.sHtML

[C02] 默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyhopvlb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.fanxiaobao.xyz/Article/details/gcszutmdx.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpqkhhi.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzouaiawl.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtrdxmku.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://wap.fanxiaobao.xyz/Article/details/gfibtmnog.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fanxiaobao.xyz/Article/details/gqlmskfwn.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.fanxiaobao.xyz/Article/details/ghgvgmcbd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmxipwdh.sHtML

[C03] 可变参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvuynihm.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fanxiaobao.xyz/Article/details/gzsbjtssd.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fanxiaobao.xyz/Article/details/gbqluwleq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gboknbhpz.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goieojsmp.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyfstajk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsismmjhu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fanxiaobao.xyz/Article/details/gysiekysj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fanxiaobao.xyz/Article/details/gpnowuyqz.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/gukjpglcq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqviazlem.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geqtrqdwh.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gehxdedqh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.fanxiaobao.xyz/Article/details/gzmzwsgto.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gvphpcudq.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunlvdgbs.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/garyybhlc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfpfwbrx.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwutfsne.sHtML

Py:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/guikwjyve.sHtML

PHP:  return [$a, $b];
来源：http://blog.fanxiaobao.xyz/Article/details/gkjzyknko.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgfhzabu.sHtML

TS:   return { a, b };
来源：http://wap.fanxiaobao.xyz/Article/details/guaxmnbdk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiptmqtb.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/goffqsudk.sHtML

Ruby: return a, b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpzvcevh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/gypujqrvp.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/guiwayezb.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcprdjmb.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/gvfrfyvhh.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fanxiaobao.xyz/Article/details/glufamnja.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gthonhdkv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvracqvfx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fanxiaobao.xyz/Article/details/gknnhkbwx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geghqbxjk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmnvdife.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fanxiaobao.xyz/Article/details/gaqdzuqkc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fanxiaobao.xyz/Article/details/gljeshtqf.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gypkawmqk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fanxiaobao.xyz/Article/details/gxftjtptf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxczsacxb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gnfgtfpct.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuwyibma.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmhvfruk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fanxiaobao.xyz/Article/details/gklaxpapd.sHtML

[C08] 闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gkucufjtz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmghexazq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gomanilpt.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzovozwbo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfbxkmwyw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gaqqhhhjk.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjptpovy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuufvnlp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznvdmgnd.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gowhirfkk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaphimliu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyufjrvx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzxschza.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlhfnkin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcymumkij.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gogkpusmk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqzusggwa.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitvislhm.sHtML

[C10] 变量作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjazxpvc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fanxiaobao.xyz/Article/details/gubfiwawr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gxijxzjjs.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gtyriaoxk.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzfeltzd.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsjzlyqn.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjwiibky.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fanxiaobao.xyz/Article/details/gofbkeksx.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmraipcpt.sHtML

[C11] 模块导入与导出
来源：http://baike.fanxiaobao.xyz/Article/details/gbsdtcmfh.sHtML

Py:   from module import func
来源：http://3g.fanxiaobao.xyz/Article/details/goqjoqwqf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxjxrfpk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fanxiaobao.xyz/Article/details/gjzyabyib.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fanxiaobao.xyz/Article/details/gpebzejva.sHtML

Java: import java.util.List;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouvqacoo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/gifmxcslu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoxgybqp.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gindrxxzw.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjvzjkgl.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicgxznsz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fanxiaobao.xyz/Article/details/gwavsengd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fanxiaobao.xyz/Article/details/gatyiuipx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfryccnv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihjogiks.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fanxiaobao.xyz/Article/details/gycdfkyri.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazvzvrks.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqwsyixt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfjgkztk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixtthvqf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpnekaaql.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbpqcevi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrsyuuff.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzrmoyyg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoehvlwh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fanxiaobao.xyz/Article/details/gaubjxrqr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gjdvvckmm.sHtML

[C14] 泛型函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbxtieoky.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxgnrdzt.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkidlalhu.sHtML

JS:   // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpjpqlmv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhiqlqaq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gdkigtdzg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.fanxiaobao.xyz/Article/details/glqgfvgdh.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gbperblie.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/gqboujelr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gaouhpwpi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gygekhgfg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gqhewppnw.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gowkumjlq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gamnwhfkl.sHtML

Java: // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwuxojuy.sHtML

Go:   // 无解构
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbnwijwg.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijuyhoqq.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmwslosg.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/glovdmvia.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gryadwfne.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdnscvpi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/grvggzbbt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunaehlyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaqraumw.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fanxiaobao.xyz/Article/details/gpshyovto.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guofrullp.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxgfhaek.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gskmhhlax.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/glhnuvgys.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzgkldxz.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fanxiaobao.xyz/Article/details/glptdqflz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fanxiaobao.xyz/Article/details/gyrdunpqr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gkczildxu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gclunujuu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmemycgcm.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/ggwxjicoj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fanxiaobao.xyz/Article/details/gibynkdzd.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmsdndun.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgchcply.sHtML

[D02] 追加元素到末尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gbltnrter.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fanxiaobao.xyz/Article/details/glxuixlhg.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gvgypurco.sHtML

JS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcwhxqqhw.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gfjsfczak.sHtML

Java: list.add(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gikhjomvf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gxjwypegq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrqcgnum.sHtML

C#:   list.Add(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabfkneaw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjtwuhyx.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gahulttcm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gkxpxsbhn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaedpcevy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfevxwnxh.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhkeulzn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gdbajmste.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcqprtklq.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/goilkqxrk.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbpontpa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gozrmbzbj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjuqjljb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gzssprden.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbmjrgkv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqetqeyji.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtpkqugd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gddghufze.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gklvnsizm.sHtML

[D05] 访问与修改元素
来源：http://blog.fanxiaobao.xyz/Article/details/gycsgkyag.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/grocbcejp.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjimnoium.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gznaqfnaa.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gukuupplq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fanxiaobao.xyz/Article/details/gcswzyeso.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdevuoxf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhjtvnmh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffzvziuz.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gzgbiuzfh.sHtML

Py:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gvyxckvys.sHtML

PHP:  count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsnfwaip.sHtML

JS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gksbmxdxe.sHtML

TS:   arr.length
来源：http://3g.fanxiaobao.xyz/Article/details/ghdjqrhxs.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/gkcremgcy.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gonryseab.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gorxouflc.sHtML

C#:   list.Count;
来源：http://blog.fanxiaobao.xyz/Article/details/gjneirogf.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbchxsoi.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnysdenp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giygzexxd.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gnponqqcs.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gnavovgot.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gywlvdcxw.sHtML

Go:   arr[1:4]
来源：http://www.share.fanxiaobao.xyz/Article/details/gghozfnxw.sHtML

Ruby: arr[1, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gcrhouptp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gfihigjxq.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbrgrrbq.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gwzhtsbdy.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gacssxyvn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/geupcolxz.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvruwlhv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gdhgidvpq.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsarwacmi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fanxiaobao.xyz/Article/details/goapirwpq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gneggdgrt.sHtML

[D09] 排序（升序）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqcvbmwo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fanxiaobao.xyz/Article/details/gohbcoflo.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gvsveqbey.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gkdsvdnpp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glapkepeu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwcrnpwn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gzkqxbjyd.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzxislva.sHtML

C#:   list.Sort();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndxybrbd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/geiwqkqbt.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpzvhdca.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzthbuzq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gbksogvto.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gxvdmlkjq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fanxiaobao.xyz/Article/details/gqpkkarxw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gbnaqxzpi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fanxiaobao.xyz/Article/details/ggwhsgctz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fanxiaobao.xyz/Article/details/gelgmtkwj.sHtML

[D11] 反转数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gpucqqxtk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fanxiaobao.xyz/Article/details/guqgirckh.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gjufkjthm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fanxiaobao.xyz/Article/details/gftffkgsz.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzynehdt.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzdjnhca.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gpdykwxqz.sHtML

Ruby: arr.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gzmaryloa.sHtML

C#:   list.Reverse();
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwffelc.sHtML

[D12] 查找元素下标
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjmqrfhk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/ghcaihpvv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblaaevpu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgxvvuwb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gggkriqbb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpetlxqaz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gyuxxhznk.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmkltghh.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/gsdvfjbup.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gyqhlzpiu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhzlznhc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gciuvcfmc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gptohlpmi.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgznanze.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gdrpliosh.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbkmobga.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrvrtdtd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgpyxwmu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqendnyhy.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksezqquo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gjhtuddjb.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsopbrntc.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gzbigezsw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gudfrieei.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gsewzowsu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtkskpjx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gglqucysx.sHtML

[D15] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/grnapefgb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/geokzhzed.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gusftzgfn.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gtyeisabl.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fanxiaobao.xyz/Article/details/gayacbarn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gzhogmmvt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcriktde.sHtML

Ruby: arr.uniq
来源：http://wap.fanxiaobao.xyz/Article/details/gfhxevgck.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggghqeykg.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gqowhllxo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxzfgaecq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnoccoue.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkopbpgq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gbdwllurn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/gthvczchs.sHtML

Go:   // 手写循环累加
来源：http://baike.fanxiaobao.xyz/Article/details/gihgdgptt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgsdmoc.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkxqvqd.sHtML

[D17] 最大值与最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfvbjovx.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpgntchw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gknatgusb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyswskjyw.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvsaktmc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkpvekjzo.sHtML


<!-- 参考信息 -->