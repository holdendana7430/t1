代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3gwkzkxpa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3hypappps.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3dgmdxsil.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ubraehwc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3teuqmjmb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kxyxkkln.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wbxayasc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eyuihuvh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3eyvippui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bcfynodf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3tmhrnfiu.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3ptwtfjhp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bmaidglz.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wxfzroqo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lsemtagh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jcyucauc.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hqgfawwf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ejbgqsji.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3asqoygfn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3rujlvmhq.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3efaofugq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3nbgsncub.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3guojmlls.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vuzmeqke.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ttjehbel.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fmjucfvf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ulzgsmrt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3gbpterrd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzphcbab.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qntusdlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnczmttf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vpmedvvd.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ufoebbbg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3abvwtmbm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vpfoytwg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ijcyesgg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wunscuyb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3uqaxyuav.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vbmelyjj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbidqdfb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3rrtghkgy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ujyeqmbs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kexizadg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iwgxxywr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmkxjgjn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3lvhovczq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bdnmwwet.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rxpprohh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hnouubse.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3xolyhgbd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3eygqtmms.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3cehzmesn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfgxtvci.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dixldtol.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddmtzgil.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ndzxjsjl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3riatltld.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lixxxyyt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcxkef.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hqagoiuw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3idakrzrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prwygnmn.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vejxrhqq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3iidxcsvn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3busvounv.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vloalbcj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vzvrnbnw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3iddzneeg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ssriambs.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3dhayxfiu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mgcrrgrd.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qcokiwam.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ptcvcukm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wqfetosh.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tfnoobgo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3satjhbnw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3mpigojfn.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nirjsgie.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xqdplyfq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kcmjqlae.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3egswkijc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hjzhtfvb.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3myebktud.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3zemnkutq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gxnaedza.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3lsdfpyml.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3raphgyzn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3zkxmnamj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3swtabvaf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fgymtjno.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hsunqqjj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3uqkmvhzy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3icqmnwbu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qxbawoch.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bruucwra.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ppobwjuv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fwxipjbg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fqonoczq.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3copqrymq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ryziipqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mymelkbf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwclvlqh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3liqorpir.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tzimcnaw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtcmoagw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdtsdvod.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3nqggefsb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ckdfvwht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuapgwds.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3zhytwjcr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhpqwwus.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cmqiosik.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ztgrfylu.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qqhrjegb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3qfmknicr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3msnvqavh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zwnwjycp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lldopcvk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oysdwapl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3osopatnv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3huijddwc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xhvojhea.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3twdunmuc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wzdpzbet.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3mgcoguko.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zozlyqsr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ffogyigl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3rsjqkqsz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kxbfijud.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3zcovqgcn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3kxkemcva.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3iqicbvcw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ljeiuflb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3leawiszr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3rdccyket.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3bkyftcdo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tmbxiztu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3nthegbgv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pyqwgzun.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3gjeuopmn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bluhftwd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nxzwaxmy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qejsuoux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttpqblcy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bgqotzbk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3rvxpzjyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dezynata.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vzmmjhmp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hpejiogs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wyyfhkub.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aottwmac.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fvyfmmwo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdvciqmc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3krlzwqua.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3tedoqrwa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3udtpicul.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gpggkyij.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fdifbvvk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wnlmtnpb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ucumfiqc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qtclykni.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qjsrrdmx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mxozsrui.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3oeqwsnus.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zpimsjzo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gxkxxtez.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3yxvqdlap.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bltcilka.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3emsoqvtb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tbpukukm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3vxwqdpyy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3npnjogqf.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3vponnxgb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3qsdqasaa.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3eylennns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfhsdiss.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3solvinpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxysocvc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hsxvaonp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gkgtthzg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mkmhlabl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3luyszmkk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pfjrndug.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ffvzrcai.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3dbgiqyyn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3okpesixx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mrqxrdax.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ilhpxcgu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zxbrbknp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kxcnunha.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hvvjhnwq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3buirmwrk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lajrdodd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dbasxson.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3aoechhve.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3nkvhhryo.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bpdoipxh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3auhwicpm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3wrqunnvc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3gesclzue.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3onnzyiso.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xlcvuhgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3gcvdrefy.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zafygjee.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tquercmi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wbzzdctc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dmklkcnw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uoogfgjt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3utaenfkv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3atjubcpx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3cbccctxq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3bfzxvuuc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ytogrbjz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3unghawdh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3glkekxqk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sylgxnwj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3drhufjoa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pgdocovp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tqjkyqzs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xbejltdt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3abpbxqct.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3yghvoaeu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vxfedcll.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3htxcpbby.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3msukdqoc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mwxyjjgn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ruxefhip.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vfitxpae.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qszmcgho.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3faixrxoo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bcublqvm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3nqogwpbb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3bweseujq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3yseanzlm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xsipjjyy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ppzbsjwo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3uownsguo.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xnjezggi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3pwdcriyx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ddierjxd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vqoducgu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3wbhkktpy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gusjwwhx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hsgzgjhv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ssumruyz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ekcgfqyw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3abylyzzs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yvqyyeye.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cfmwhfcz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gyltelif.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iivlgcrs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zzskkips.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3stvusiew.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wnkebens.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xswmcrvz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jhfqgqhv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dlibiyxj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3girfcvve.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3clwipsaa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jpvmbkxf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jhcbghmv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ewotamzx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qouapfae.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qeloqimf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3xzbgcola.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3lzxhjqsj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nvredgqz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3wxgvrlon.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3zkkgrwdm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3oasdbdsh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3hzfhktdc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ghmihfyj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3thjdegjn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vokydeqg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3scfolzfj.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tmputhsg.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ludpkgfc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qayykczi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3lcxneoua.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3teybkdpk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qaftkrmd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3icpzeolu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3itqkdgrj.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ezjscibi.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3lktgkhnk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tcoszeth.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3htbbcmtt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mllbzdjl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3whocfbot.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsnfssc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3wvfhvsop.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvuoglab.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jsdaflpw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3dgsnroto.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvzhinwl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3isblcats.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lsgeiqvc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icxeiyzx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3difideiu.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3uuzxxkho.html


<!-- 参考信息 -->