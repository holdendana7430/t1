代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2vmofldzp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2zfhpkpoe.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2kxwvyijx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wcpdifpr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knvsambz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gatjsoyo.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wtmpqkay.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uoneukiy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2anmczvvm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tfnhtnkc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2yiliwguf.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2uhwytsqr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cmxknatk.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qzwwkbly.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vymxsnvx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dckycihu.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jfpugewa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zdlakwvl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhzihdfa.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kwhncilk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dnpgsswt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2duohdddk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nzaecpam.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jravdcjg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yzvohncc.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fbrtqkkq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rzfcwnrc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bjapvmor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdeopbej.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2iypinpzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2stqysxxj.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aovrtolz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ktucalwl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2slxyyhzz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2auduxrro.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wviwwgux.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shnjfwqq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpixmwba.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xegmfdml.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gokrtwdw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbdrhuaw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wgicxcsx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bstlqoox.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lbjdtyrz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2quuqlqhu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cqxtsvpp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ptiecuqx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2jtoiewxn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2pkdnvgkb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2irihowlh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbfvcmo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yinsdnwh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fimlfhsg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qwiyvuxl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gheztxdq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ckzrzzsp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixwdmoqf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vmpeptru.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcpuclyy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2btmpdjjl.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2xxptesmv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bwfyeuhj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2leoaryki.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2vmvcphll.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2bffteutq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nneaubhn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hijaddep.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2vwculjvn.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2epgveseh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2idxluebk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2evaqayex.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2soabtbdc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uqyswmiu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fmsszbjj.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pjrztuht.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2tsmdyhdm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2fljfexld.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ttpmfkzp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xwoaohrx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dctsordf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ewcovzwo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zcpaqolb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2okaezsrm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nnopbdrh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qiripoir.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2omgruiwa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2izvgdtwb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2negijhbr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2anuesdbf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rwpzmsvu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hlrajjqf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qmzvfhly.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2xnzvjmqu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oxodghjb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2whpzosmi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fxyfyfif.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2iugbsfuk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2runbzwuh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uuutnagd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2psmscaxj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gevgdfle.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ggeinjcv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2apjgpyuf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qfvkwdpp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2etedtdmn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mreikggb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2imvyggcd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vwvindqk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kypzlesu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wimcsuxp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2krldwsmd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pabdglhb.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dutrenjb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ebtjanmh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2btesqulw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2seugvixo.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2infhyhpj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vrzhbxwp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2izgywvfo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xjuiormb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rbtmjoez.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2chhpisza.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bkgnrupk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zvrderbg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uwkbccph.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2sgqndxwv.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ezlzrtsd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2rjmqwmbo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2icfbfpct.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jnzuqtcl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oanibozn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xstvccwf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2npjiifgf.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rgnnnich.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ejlkdxib.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ydpbvnhb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2sgbevfbw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2iixmyspq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pvtrdzji.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tfplafrh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2owvmujtc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvvxtvrz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2bmfurqln.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gviqwuvf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2srciszby.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2nxrcsvnj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2cqwwrkkk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ctmmqhan.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2dvoumdmr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2oanxhmnq.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2roabjcad.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xyuubbvu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wclolrqy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2depslkyz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2qurajgqf.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kjrlqaje.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2zbgpesvl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xkvniqtb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2njfxpyyh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2cfauupvx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhclyvdv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqulhjon.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cjkumeih.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tkaisevw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2eolvsnra.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bukoxhvm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wkucupvf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2itrofplg.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2skzskcwz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2cjqswpkr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2eufwurjv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yttppgsk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oelhwzks.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2qbfvbgzn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kwoykmoc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjvwlhay.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cuqbvscg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfjxqere.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wjlofeeg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2zzrehqgg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ysvsnwwb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ysefbumq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gcrdgfpz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hwwamskt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wfjlhmnb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rcfwpdni.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2blzfatgk.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2poddoiqh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nmribzzh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2oerbmrwf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2siyogtou.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uulgvbmg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dwacodcc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jlhyhiux.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qhrxxjhb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rdpudolm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2giusxfeh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gnbsxycv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2rdrikzlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2txmvexsr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bfnionij.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pyzrwrwt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rzgvykdd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsgqzej.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jdvnyewu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2khhsxoyd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cxokbcjl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ynayyrry.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2adlcqeab.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qqlktvoe.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2snvwmgnc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2sxrokgct.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qovgkgre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2kafeunuz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2yxuhurcn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2klcfbgqi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qytwiyhc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pdmcmijp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kjffikkh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2oktxuxfu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mftxvtuh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xjtetomx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2udecfhdf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2paplhmqj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zentmbqn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2yrhxjrpa.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zulwhsjd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jykuymae.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lmuknkwi.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nddcvubk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kbxzsldu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2dguvshdk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bvzqvoxm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2mbcvrpnk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2irmgynex.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ezrtixvg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iweflegu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dusuvsqr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ecpmiujl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xqijsgjw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2flwfsdso.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2epzkpbqd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2tegyhgkj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2jsropenb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vhdgqpkx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2duzotrpj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2adnlkion.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bspbotio.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2almeeytc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fepdjsws.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2podwtvlo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2accyqwah.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2peyuaeup.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nnzqelia.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2nhuyhntu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qtgrhpkp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nkwesjqs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ycgndpxj.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2davdsaxq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jeiihddt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2utfpvias.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydbdarvb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2buevcxgv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vindahhe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mmcfxcjd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gprdfedi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uxhwggjq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hfhqodua.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bflfycjg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lafkelve.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2yjnqkpwq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nnvxzxgc.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ibbrsuyh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qjsyqhvf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2drseuuzm.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vybevroz.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pzhnjeze.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2bcjtaejc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pchtxjgl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xmlbqsep.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbefxcw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rajilrge.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2shhltehl.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lojmlnvk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkqqqtgi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2jtlrlnan.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zgllwtom.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gqfdvwhr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2yaesgkcx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ukqnshyb.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ghvihuxk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2anwxbijn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2hcbfsnbi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jjvcaqkz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lhtodsuh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qnmexqoc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vxrcquvr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fnfyghtc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wpopqkvf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zqjtagko.html


<!-- 参考信息 -->