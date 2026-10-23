代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvprjjmp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3spjkiaso.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bccojmoy.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3iabnmirp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uwugwibr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zgtodfei.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hxeuehoo.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3brbkmusd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ifowgwew.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sgpasjau.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjpmchig.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3berxcapf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yogudjjt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3axlwcnns.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3oeodwxal.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aafzqwat.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rhwyrpni.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3lwnfjssq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fvpqjxyx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sehelnuv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lbvmpcxe.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jdlplbdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nvanempu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3yraeknar.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lxebymkz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xkixbhyt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwhbnymw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdqzxuzm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcyrsxim.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3cqvnizpz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3pafobrer.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcpznsue.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3nqqwfmvw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ijqpabex.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ntaokouh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kekzwsmv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkdsokeu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3gvbqdaaw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3iobsjyov.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kzztzyac.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3jmwfeqxe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3qbifadlf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3youtjifr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nmfxynzq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3bxoriidm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmeyynhh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhazexaz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3seiykyyl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhkcalhj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xngimuto.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3xhjmumec.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vybtpduq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrglwptt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ttsylrqu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3icamyhtu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rclnufvr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vesgqoje.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3foyliukt.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgvwtmv.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3viujbsrz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yukdwtjy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3bolwngku.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jfcjhwsb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3dmaqdcnp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3wfjyllxi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zxzlnmbv.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yijlboni.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3gejjnzvw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3khwrrttu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jrcxstuz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3mjqwmkxn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mpvowocp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fcwaiqgy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yuqwbgjb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zsfhotqr.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3myocyozw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gfbmzeoo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hodfuekx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bpzxszte.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hrmkccfy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3eredcntt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hamypjgn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kixnfofa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hzyhbsit.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3cqbkmnub.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kyinqfjx.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3thiubumq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3baflgjjn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbnsporu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3emqrslzf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cquratis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3dubwhddn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofxiwset.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bswedhbl.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3moeteykc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hpezmcdg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fchjjtxv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3khqjdqnb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uczcezof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3eokmgzgd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bnyhlegk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxeloulm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwqddfh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lqtwywyi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3boqmhcsy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gsfzbjdi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gpdvptak.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3cwtqdqxp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3gwhvlvhy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3llvusybi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rbcklypv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3stljbglr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eedmsyur.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3vasfetnl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rsqqrsug.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gjyeuxoo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qiqpkwzm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3tiiupukw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jaztdvvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3boakolml.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pdesggdh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sfwjmrtl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3eedvfzyh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3tkqahikr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3dykzolrj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qovgjoze.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aprlqczc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3qhtinheu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3llqdlvbk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3odqpyvpc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3csxqdwvb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ydhdyhfx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xquinsuq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tburtmqa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3cvbzbqjo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ehxzsbiv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pjvsseeo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bbyxxdwq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3puftrzgx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mcykbwki.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3btkahxku.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dsxcafjp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3byrobdxu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xzxvxurz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvihpsd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggkswtsi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ygmfpsdz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3unaowimr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sgvmfvoh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ejejeenb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ttokuupw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3nmcfhqds.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rawaijod.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gcnrqiwf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hsfmzrjq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3blcwzkum.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bvigfxik.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3czeohitz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vwrmanrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3lagouevf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qkwpuqrz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3podzkgwn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gmzbnjmd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gmlsrcvk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tgyxmtho.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ntfiowra.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3otdlepkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ettdohzc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wsrmxizv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubvudrbc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bdlcpzpy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3eixfkvbx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3gbzusakl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cxapcwhp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uytjfrrl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cyctkszu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jktosgvv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vnanfoav.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3xqqzimrc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3qczbcprv.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3syhitxcf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3igtrsrmr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uqrlcoum.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3winjzoli.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nicvpfwd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfsyikb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ierqhorm.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmuzsay.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dpxnrztd.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ulufvpos.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hdyxtmlw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3csfwsvcb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ewwdxdzi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hrwfcqty.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ysglcxtx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3vgjqxoha.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iibnbhzm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cexcjgyk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hbqplvzj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rgsqakxt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3migifedu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wywzrxjy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3nvsdahca.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kjuhrtle.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3porjhsdt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3toardzta.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ecdtbcoo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3viodjxpe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gzteuzqj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hatkrwyi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vktojsow.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3osxkuzpy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rvzgdfur.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3tfqmmczn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3upjrwwxc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ckzdfjyb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uhhteulx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tdzojtxv.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3egorbxoq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jjlzxpzy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zhgcnhcn.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olmsogee.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3sfidkqlu.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gemdwyxe.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zshukvrm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xlkmwevy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ccmyyexh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lfdrfszz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lufkjtyf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3qpjblpwf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3inhndwqx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jtxtqqes.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3joozupax.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ocrbrchw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rwdtqxpo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3yvkmpivf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3jkbvhemb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3wqmsdyig.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdrzewai.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3rziuiaer.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzilvar.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pcjbdsij.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wfghnvkl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3foezwbbw.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jllkbazn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wxrdehau.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3jfznqaac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3hjyxsggp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lbhdxczf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ogqwyseu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fsiuwdvg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3joltflky.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3akotyaxz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3nyhunmkc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pwhprjnt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dzzyxqnv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sfctkhzq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3srfaudig.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3aczpghlu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3tkjvrniy.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3kpvnmlgq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mdgftjmf.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3byxesqhm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wvlwcccm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3zplywhrl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3owsubbbj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3noxpebly.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3xqewhrsj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vjgzhccw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3rdjwpccw.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3teowjdpj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3kdaefzot.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lklqwqaw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3oilzgsnv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3icrlsmpm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ravmxner.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qkzlagkw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ezeeegfj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3pykvcyqw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bzpnkler.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qydxzurk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nthrxbxq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gvpcyloz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ylwaampb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3mktoekbm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vyksgnmt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ywsyiewb.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3hdtizsgi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xbjuzvnb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zuucxueb.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wpritkkc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3iizrdvvn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qsrgevyz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lngkeump.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3shplualx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bboufocp.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3qrnvvzal.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rnhvogbn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xajeukmq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qdpniemy.html


<!-- 参考信息 -->