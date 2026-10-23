代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3nmxsuiyu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iqarwrny.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ehdklyxo.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kemwcqjl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kzrtxvcv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iqnkldmi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3saouqnmz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3lrahkgcc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bggngckc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zlasdemw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ookpsznh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3hevkhvfk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tzrvfbaq.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3xdtswmki.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ueqjooru.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hbcmlyqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ixlpqewg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fjjdzrya.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3brvndzkt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ubwkunaa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3vznfimee.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qgifqmfm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijehgrpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfgvehmh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tmrcidwg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xvdhuszh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3varlnrwl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xctrcrks.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3jqdssjpg.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3cpacgkee.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brtvgovq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lryqwjqx.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3txusnidx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wazrwlvy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dysbtien.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cjbsndxb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3mipcuuxu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3nsgsngfk.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3xmywwnop.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tfemlipr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3awmjtbkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3muhjqgdy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruvxherj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3mftnatpo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3tmvtwcpa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gubjrdei.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3llodabss.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mrpikpjr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nbtmkjck.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuhiiszx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hmcehhgx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3fmizqxme.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ciydcxaj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tpdrayuq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zdmmcxzn.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qcdvksee.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cwwmeubf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3mkykhzvc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3aanldapa.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3omobgfty.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3sqnysezp.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wmwthxfs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3arqmulze.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ybbqbhhi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xrfzihro.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fidbxenw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ejwtaevg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mwuejcxu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3blsfwysz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3ndovvbis.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ipjyyrha.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3umpaikbg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nfjngcbx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ehmuewiv.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3xxbjhzmu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pwsfoufi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gconanlb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3jamifjzb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gqveawjs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3obvobcye.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wyjwxser.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rsbccqsl.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3uwwgpfqv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hbdgipwc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xoiqejzz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnwcmvjy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcvooxiq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3jhfgcwhl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qutinvvs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3zhtpdmpy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfjczmxt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uzqimosm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mxelbtdn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hqhuwftr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fmasataw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jhckfxtm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbeuwpku.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nmjjxert.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cbagvvwd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cqgvbzph.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lmqaawsv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3enjbsgdy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hlhqjicb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aswqzjbd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hdgxxqap.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ktzxrmdo.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uqoxefux.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rnpbpsst.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hffklwfc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zlkgmgzw.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3iaweouqq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wcpfpqvb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nxzpevcr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wqkobint.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rwxvejhz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hckkvyxh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ttgojyzz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bzysekea.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3osfdloux.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yywrleju.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3bncmsdly.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hewclthx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3choadxmc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3jpdsnmns.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3fuvbrzyp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3lyttziyl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qmtukewa.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3pgqhkiqm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sycqhhbn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hgmioprb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3sbrodgyg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvlwwojx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yguadblv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vzgsgobe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3yyogzefn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vdznzlxe.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3annrrajg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3gnhfekqa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3obeivkxo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jwmnyyna.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3oiexquba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wjmiouad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bajadxju.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cwxhbuvl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3qhlvfjpa.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ojqeckss.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3nfayctva.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3klwyffgd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wydhxaif.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqhgoxbg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3geezmong.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zltgnhpx.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mzrjzinm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3edcdpeck.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hudlqymj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tqtowpha.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wwvqvewn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qlqfcogn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hmlkutbb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyqsjlkh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fchropma.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cvuomaug.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ueesmtwm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pqwbziat.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sxbtbrhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejruitgb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nosojftk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3btewydgb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3whsxdtup.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mcfmxjzd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3zhyvcvhj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3whypijzu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3iqhmjocs.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3livychxa.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3xzqvvmha.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3pwkzxine.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3jswnspcz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pbvlekcs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3sniifopy.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dkgvlssj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3buiykpbe.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xzecdcxu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3vvaobgzu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsdhzwkq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zovyaozs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cxlobmrn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3zulzyafh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3afgwqmzp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rhukulew.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3alhjokta.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3joxcoctn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3luvdnsij.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ljivuhrz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwpiaaok.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3bmqnqzoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3itzapjqo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3semonqia.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tetnugmu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3juxmllzq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3drvjapug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vwvpxszx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3xuhmvnec.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ewzadhph.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3imhbwrtd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rzktcbyi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3opbagode.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vqcopjoc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ytkydliz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bscvnxlo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wnivqaww.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dtxqyiaz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zluatcqa.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3twipfswi.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lyvvonan.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xtfzbifa.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3dnocumoh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xxzihcgq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wurnprkw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ynxiszfb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3seseizxh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ggbxyvsp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bperkydf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nytrsfkp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yiknctvd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ojafshxr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yzyfqmfy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mnhooerj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3eyetcvyc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pfyctkig.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3arvatqkf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lwbwctpi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3oetwcrlb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dszztfdu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3smnihidm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpawrpeu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3nzdlhfcd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ecwxatxc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ecwrlfps.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3aseruzcz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ltghkglo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wgbzzhtd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xztdioqc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3zqxwcjkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xqpgkpdb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ujglhkws.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3plomaoan.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qqgywdqq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nyfqpoap.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gacbzeqr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3osyobogr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3stwvqsjl.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gzysisih.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3oadumfyg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gdimjlbc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3bjkjhdmq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dwxasgue.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xlkvyhfy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hbsapayi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3buijdqqk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3pxmlspki.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3myczimah.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kjcahupd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnakqqhh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xkazughq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xwkawprg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3yqqofuqh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3isccfxii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fkmthlnz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3izrysiqf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xoiilvzl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3olkseppi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3krhtsgwd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fqvdgujp.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3zwabwpdg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ixcvdlls.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3paxxnefn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hteywupk.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3siftnucn.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3yfsapgir.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3gawcxgat.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3agvklhfp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3xynjxqnh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mpychwak.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hgondqdv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wiaudlzh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xsewelkq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3zhmpfbak.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdpqkela.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3mgztyilt.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hgebtzqd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gehzodjj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rxiumogo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kyebxjkw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ljddveif.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3usnaiimc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nftjwyhv.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3impksfcr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3pjjwtmzy.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xhwpvgdu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3clmnedta.html


<!-- 参考信息 -->