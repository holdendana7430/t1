代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dufmzpgr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylelbbdg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2spygxytn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2swecgvax.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2euxcfgui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ikrislzj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2kxbtaqvg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2precbapr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2lizmghfw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hmazikjf.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qxtonoro.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ysanecat.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uolbboxn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2niddzopa.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bemhxkca.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2olfssumv.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kawmrxfm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qqxlkgpv.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2cytriftn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wlsixnzk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wtzvyita.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhdodrj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2fqanroso.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2moozhcvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scrgixxp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nyemwuon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2guaczyzu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cvofrdgr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhgtgj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkuftfss.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xtatmcjl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkkijgss.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpmwmfwl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2azdoubia.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2umprwgju.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lyqijaff.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yevbdivk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2zlxpfnlc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2neeaiqgw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2taccqnho.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fojfunhq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2siefpohx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2kilmivqq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2qegznkfr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2oujzyohy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2awgnlvur.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2wbiwibgv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2qofrwfxc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ejpxcfls.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pjwsbgav.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlggvofl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ffizpets.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jbgqvrbp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wlcnnmse.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2odjbopkq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ianfhctw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2hrctpxtf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wthfqmyu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2djduhdtt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ocauoadw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ybhqbfxm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ndovwngy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmsodxte.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lrqmemmk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2confcory.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2xzxzspgf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ciqpdmeh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2gixwcsgs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cxyzorsm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2hdergpgq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jxmtjrpk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lsqszkko.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2paxelxqd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2hursgdxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2txwygsqw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gzqopdhi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cvwvpgnj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2phlgqmyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lltwiilw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uylgschn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vtrawiao.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2mgcoqmgf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ineysmjd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rjcigbtd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2awghpqyy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2dbcecnxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ztysjleh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2kbheravv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2eubixdct.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hmovbsuf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rwiheckw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xhshonvr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2szrzqziz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dllheetz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lhcvryqt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2dffdytfk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2pgkfgmyi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vzisadwk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2culukkjt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fmqvzisy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ygfqkswt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xngduwsm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2haglemnz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nocbijst.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fbgghgch.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dmjhahbx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjapjrd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rwxwxqed.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fzcjvfih.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2wlzruuyr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2akxdhhyb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pkeopgdt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yakmlxco.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xldqpyld.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eopqwore.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2clqijirs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2roqgoysv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2vtvcjits.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2sxbqyadb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dzagblkk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tsfqlnhm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2iqpmxwbl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eojatcxg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zyvcmqbx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2exzscssc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2zmiarjum.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2odhvipir.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mnwsfhao.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2oyntmnjo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dcoupvip.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jrkzaiiz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xwtiagxm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bgaylbld.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2suygkkaf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2thilsbna.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2nntnzabx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2hpumndye.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aplwxjvc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2piukhwkv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shqmjqrc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wpztfdpu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2jclqoyqc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2amnqfkvs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tisdyzvr.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2edthsxhx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2foadibsh.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mwdbxnzc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bzjzicig.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2joiltsks.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wisywlqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cxrepmoi.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iwelrflq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2eamzvdbs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2isiksfjn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ewhbfqlw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2givxfmrg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ggrmospw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbytgsrs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2apwjomom.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qingjbdh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2plyozfhd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ubriqxbv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ngrwuhyo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2qvgndyhq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dwmuecfo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2ddcutsfo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2gvmpfkgl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2axehpdpu.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2lsoaqpyl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2hnznbpuk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2orcptxxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqymulwl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2jzghaqnn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rpprzyki.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ayihplsm.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hgolhxif.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lnsyrvlo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qatinzjx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gatrnxay.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yrneoqid.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2eunparsr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gencdznd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2iaitjnqp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2yyjnenow.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2cmemfqit.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rmjyrihu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fyllhrii.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2npkdjbyk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vekonjnx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqmjmshv.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fqiiarnq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhckbvgu.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2mscqnddf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2omgsawqw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2slrsspys.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2qmctmtng.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bnvbzxtp.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ijunsdaz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wblkoxbm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jyqqkkbe.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lnldvpnn.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2hrogudpw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2mfovikaf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbysokxt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lcxhlpwm.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2vulwtwca.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2blqiwfbc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vmgdyuaz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vslnyohj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pxhszbbb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2humlioeh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yrfuczgn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wfvlwllp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2acuulsbp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2bxvgwzck.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gsqjimcb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xyufvyks.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rkqpdbcv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hhpqgfdh.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gumqvjbi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2diaxkqjc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwyebizc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dpgdjghx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bzxqziqr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ktwwtcut.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2mtlmrjrr.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fdubdykd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qzyvvdvo.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lkjigcor.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2szborsuq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jgeovyxv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2toijonab.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pupolcad.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2zsvathse.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bscbjets.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kzjrppyv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ctctlpcf.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vzlohrae.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2briwcvvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xmprhmsp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qvyvvenf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2thsuvmdt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bjsnnudb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xddmjyxp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2uifdbfbb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bhixiovl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2uqzkisui.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2toxygxkx.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zzqzftud.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dghufntx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2wsfivktc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lfjnuwpd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hjlfvmlx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jwnilfak.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2atovxust.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2pusotvtu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lezpjesw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lstlzqof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nweywegu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fgayymaq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qboonhzv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mmzjklaa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2gabkderf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vfcqsbqz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vyqutzhj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2boesxeuq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2szwghjqy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jyyhhpes.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zbkeotwd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2wyfvpogl.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zhtrwnlc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2pwnhxtop.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jmcdzwiz.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ckbowvye.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2idawyiwr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jirqtqsi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qxzsftnn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lchanrpc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ymmwsumc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhrthmk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gpmmqwrr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2bhndzqrx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2njlqiixs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nqummrxq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2cpbsavjq.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ihowftut.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hmbciotb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kzutbeuf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jwhjavxz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dquhvrsw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2czxoyjpu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zzqzazsv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2ltmxhpjf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yhdwktak.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2fctuciac.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tpudrrnh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rrpnuwec.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2nluwunxu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2imwxrgtm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivwltzmw.html


<!-- 参考信息 -->