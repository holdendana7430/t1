代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3svnactrr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cgkryzzg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3nftwheln.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3sqqizzlk.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3gvcecxlc.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cokwyqnn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hkllygfz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3atnhlzby.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xncoonik.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ijkxopcu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kchvnjiu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tqzkkkec.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3uavcuwwm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3doybpxot.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bvjslytg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3cxpopjuu.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kbhrlhce.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iihiepal.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kkkkkuer.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xuoaedrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fpbnpebb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xojueaos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryzkxzbx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3pquvqzsa.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3htjhtebq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjucyatq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wifsedzg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pvvdhukw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3occmpfox.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3emjioile.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pxblvyiq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3odljnlqp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3iiydzhmr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3gbcultjo.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vzmbgkmo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bllmywhb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3djnrrils.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vazogeah.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mqbkkldt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3dmyknmai.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jywzjnek.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xznsfetw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3nfrzxfhu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxihilq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nssvyakf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bthdmplx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lxhtrmkg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3fjfxtywh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hboefguq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rslhrygh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3chawzvzl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3csgcxgbf.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vsdthoqo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fdhkxgyy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3sqptzoku.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ziouhvfa.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3lqqhigps.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nygbmhgv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3zfsmrzfo.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3olfpdnly.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3guektdsl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3hugzucsw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ioxaijwj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uteitkkz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3utqumynh.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zvngztrj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3mfjdcair.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3wvuhjalh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ggdfshky.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xkurwgwj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vmfsjxcf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3exnyrmqv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zqyasalz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fhjcdsjz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nmhlpxao.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rngenbmp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3izokafzx.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3mzoyrpmn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mwvrjrhd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rpwzeutb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3uknbbrxa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nikmjiep.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3cjvbvxru.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3wbyomytb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rrkmhhst.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3lbehzwol.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3mlcenvoc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ntrfurwf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3kvxyjzsb.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tyuobzzp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhtgolmv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3weobrbiq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3zlpmvewu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ghnusgeq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xheuccnl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nkhtpkqt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dqlyvxil.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zrwjgvup.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3homkubpd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hmnekoen.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xffjvdkc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3deuhqrey.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdebtpdg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3mvhxyhxp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3aocesuka.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fzdyjrjo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fncnppvt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dbvqlhzz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3axlnwdux.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3czfntcqx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3acpjhhvn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3bfiygptx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jzuehknn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jtcwzgkn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ndbohfhx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wyozwrnv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ioewotop.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mtugmwpg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3vualaemh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ooenyeet.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3vrvchecb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tbdbtchq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nkfdqruc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bnjabdkb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3memnyntt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tstwmoup.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tydshltb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pkochiwy.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3oevekcnq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fopjbsgc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gaebqhxs.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3msryoqsh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nojkpgsf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3euqllcrx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ysgpnxjp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jnyduuyc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3egkppljf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3odgeyhmi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3dtobkfbr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3icvdjerk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ixnkujha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3xgqnminq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ftxuwmkx.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nmlxiwhm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3olcxfbkc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzyfybg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fxufwpsf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yxfttbme.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3jgzlrynq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fkuzczhu.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vbreijub.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3whjlvbip.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ibhrtwoh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3udskcpzi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qupevpwa.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3togirnzq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3uzggkrvx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3shqaqdct.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gyoudlsd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3aevcivos.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rztpdfjs.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qfmwaitc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3dpyedwre.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3dmuglfau.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pytknxxj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3udnwsppo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3pfpxqexh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3faggizxc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3mikqlqmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icamrmnx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gmfivonl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hbdepodi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yrhsbyqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mcwndsyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sxnzrdhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ctjhmclk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3jzsmetth.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jdnlxryb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3btbpmbrd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mktighuc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pmmwabvj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3xopxfohh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hbwfuqmo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wsicxege.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vxjtockh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3vzfotbyo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3guykdhsr.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oqtiwqme.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3twrjbusu.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3axqjcgul.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijdocnau.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3myiuoauc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gdfndypa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pxenjxyk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3nbbnoker.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jitrjtcm.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jmtwstcd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ldqbomff.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aupfsaez.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kxskyhwn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pnhnifzm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gnsbquro.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3duegcmvc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wbaanwvc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sgtzywns.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3swjbdmny.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ijjiqcid.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rhucnrst.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ssxleryk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3genxsdml.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3itmtrazp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3skplzgxl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3avepfjbd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3iogadnfo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bgwoulmy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tbnunuxo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3koyyydee.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3txkiagbg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3bojlblbw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ylzebdcy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3jhcthwgv.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3juolagbg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ogquhlid.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xjlccdor.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dnnsivcj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zbmcheve.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3qemvgmxk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kryrtctn.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3aoaplxwg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uoyfoogk.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mylktuay.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pzmnujrb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ffcsjqtb.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3ytzkboih.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3iynbehfd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wwmrwhji.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bkejpwim.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ekojlsjc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3osjiieou.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3bbkmfofc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pkencvrb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhbxiwcp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3urfzgmuk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wgmzxswp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3inzitqyn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ydmnzzvf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3oobgboqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3uiggupkt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlbkussz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3aonejhyg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tofkrvks.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3kjazajue.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hnnxstez.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3akwrjkfj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3djltajyp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fjdjglza.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tmieprmw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xkqouopl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xqolputj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kfscxiya.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lbqpnlax.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lsjxcjen.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ykqkkfbg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zbthmcvt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xviaswpv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bthuogpy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nhgmkbfr.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ycscqmmo.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3skamcajx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3jkflexgm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3aiyqayiy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noqcktol.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3liltyhnh.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gosvamge.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lwuesoma.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vdbgbhqa.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqtbkbya.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ujuhpqhm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3nqcyrnwx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3havztgtm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3aknhcrvw.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3udyxjwqi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3mttxqbat.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uipthhss.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3zeaspjgb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3rhbgqycq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3krifqtxb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3hydnqlfs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ezfgjtqd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3lrfiaoyy.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujlwknqv.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rojtpzgm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dhmfuxnc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3dplwkibd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugwynqbi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nrxoumug.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3gzjnjvjq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3aensqalh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xrzdvrbr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3nwubspiy.html


<!-- 参考信息 -->