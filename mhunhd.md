代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3egqdxoby.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nlravbjk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3aillhxdx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3aqkgxieo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3ccllllsf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ccebgnwa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mvqhkbll.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rvuyvmnk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytzpsdhv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ztfqjrca.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbaonvvu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xuvyoaib.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3thlipgjv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fumwoqwy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qkoigeof.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dseioggj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3qpylncbh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3cfqjnlda.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3obvrfrld.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3bgbefdhb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zxfantwv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3avdupgwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yohylhcf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zfyrqbkx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kkdwavzi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlclgabn.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eecuhbjq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ozewuetd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3muqfdzhy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lykxgcba.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3uliigetu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gkydegvj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3amubqynb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3mblpejiz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3xtuzewpp.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fakjmsek.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mfdkkois.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wasiiasp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3djtjatbq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3uypiauzs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eixgefxi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3foqirbfe.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dvhxynrk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3heetxusn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzahnnlx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vvgqlkqh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhzebgux.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3kwzkyezd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3gqqymdwx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ruytmwoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lhlomjte.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3orbncddj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3opssssao.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zrerbemz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3usqurtek.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3anbknkgj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3czuilefd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlrrexeq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3mnainyhy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3eyfhdtan.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ujtjieql.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldawigxa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zcfsofkv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lzhchbzp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3piecxuel.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fgadnsei.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zfihgpdh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3dfwftbnq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ldxngkkp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3kpbxvrxm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gecxlomq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vvsvmxim.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tonmmpct.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uowqtfhf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3vobdphnf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbywxzj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zfmphqjo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gfhozxjj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3pwyejkuz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ovjarncz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgmpsux.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3euweclba.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jaddxbme.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3axzgleof.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mlsdotht.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3isnxppuw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3idsijdtt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3goutobms.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xiamtfxz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcoifhqw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uzulhirs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mljvzlec.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3avxblfoi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3hgsbglfy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypqezjsd.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ajhnjxcq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yljevmet.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hexpccal.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hysxuwub.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3acpuejkc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3kponsckk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ckxiezth.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3tcorwvss.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gehmprwp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zoglnsbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uqaekahe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3azbrzdtg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ypknlnau.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3unexonox.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3inerpxij.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3czlsjjrg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3afmyvfkh.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gwmfyjll.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3iknwyhyx.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ogboxqbj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ndremvnv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3xatguyal.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3stkmfmha.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qshkjkmd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cluepbti.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3htkzaqug.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gqumoehk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3tiqcpjpe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mvjuhujb.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dbwiydlm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ilsdikkw.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cnfdddic.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jjpimvja.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3rdpfsevf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xlnrpvde.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3tiszudyb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hmwxhhko.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dgqpovfx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bifdmbxg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uhoyafjg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ddfhlttw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tqfoljci.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3hfpvzqrj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ksuulijq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xeidzjun.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3oynshgzy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uzsxzvkz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rybyjxlk.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mgiofsey.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3nxdnmnts.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3nxxfaocr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3drarrniu.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ydcvrdwk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lnpgqnje.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3dbdnezzm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3rhdrmfjv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xtohgspf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lrcmmuov.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tgjkwtcw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbcnafam.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dvihamll.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3balpjwcj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3bctzcbof.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3brlavgnr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oprwjgbi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3rbebhnlc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3urvwicwl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3qnmdmjkn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jozueqhm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vlkuiihy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3igjtdlaz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqihlmhd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgzwarru.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cwwikviz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lnyeyyac.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cwnkpfsp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3dkcmvnzr.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bkipwjbw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3gxlrkphv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3jeajzgdg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nvwcpttu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3tmnsarbt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3tqrjtkdy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3mlobdrfs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xpihkbse.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3bkibkvkq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zomlsnlr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cxytjsxg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hsqllltb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kimuihcs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wnhyfmgy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fyymvxwe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xeqgvrwb.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3duqoaqsx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vsgipykz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dmignpwo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3klxffwha.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3szswswnc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lcspvzfh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hzegajei.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpuumgak.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zibnxkcr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ljrdbkro.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jpfmjtpk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jjvyflgr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dxwkdetf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3crrxzcws.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3milyhcoi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3lmsqjtbs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zetqfvqe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3cmlkzmex.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xopnjlab.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cgdtkyko.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fmanrqwq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bzyarugh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dogbphrd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3rajwgpju.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nzedtvqi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eljgfxwm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dsxshbvj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pcguwbfd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxuarhqw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvsuzgaf.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ojiqvxvu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mncnoyut.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3skogydhp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3vycesijr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3oaewpcmj.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3ywzdhfwr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ymyhnljv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3sjzjbfdb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3czcabddd.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xtkhmdck.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qvwmftss.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ptlaabso.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dnjshhfy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3srdyteie.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nrhmsysh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pcitafei.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3idziamkm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3excxcobn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3hjztzynf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3untlttem.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rqqxelhj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3iqcvdynl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3agopecxm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tjwzilrw.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3twqeaeig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gnhanyzr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zhrcfwqn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3feplssms.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mmuonrtb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dzzktjmm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rvcwahau.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3cbpuuffe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tjfvapvc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3trsnvjjl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3chlhnerh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nkhriosr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ghezimcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kmmpvxfo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wzibydgn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ojbpijtd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3qczervnx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qkcmvagp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jzanugnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ejtmyifp.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xdsebltu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lnjdddlo.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fcnfvena.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mcbqhywf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlzxbqjc.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lvfahlgy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vrzxnxnr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tgaispru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ddqgaoah.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3scisejxv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjqosqey.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3yxwwdwuo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zjthzvsu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycuntdcl.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mvfzatcu.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3azemeczc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3laaauhcl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gwbdzdvs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wuncsebk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kkehcnqj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ovzyduth.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3msminbhn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3gefsyaoo.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3anrkckpe.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zmoceyex.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jydsylvy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uhauweey.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3aqlgqwcb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ydheblav.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vofghtbv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3scygexed.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xlorkmxx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3glbzsdbd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tqszqdzg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3llswbbzt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3kicwkzdp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3ewtbimmm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gpwtzpdh.html


<!-- 参考信息 -->