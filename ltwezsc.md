代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.share.hesvh.cn/Article/details/gccyxncen.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcvpumbzu.sHtML

[B15] 布尔运算与取反
来源：http://wap.hesvh.cn/Article/details/gxzmznnoi.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/grexgmoyd.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fehbvm.com/Article/details/gucwfcegq.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/ggfmlrhgt.sHtML

TS:   a && b || !c
来源：http://blog.fehbvm.com/Article/details/gffyoanrp.sHtML

Java: a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/grapunbqc.sHtML

Go:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gcqvvbiie.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gqfenejdd.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfvdyokfy.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.fehbvm.com/Article/details/gzwtcdjcj.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gxvmxuhdm.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gnsqmezhq.sHtML

JS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/gffxxktlq.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gvmoyrbwc.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gmigwyxcm.sHtML

Go:   if data == nil { return }
来源：http://blog.zdbjq.cn/Article/details/gacswsadd.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gezfuuehc.sHtML

C#:   if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/grjerlvhi.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpaarobvy.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/gtrnekvtn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvmueymit.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gobyxfkii.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.zdbjq.cn/Article/details/gywrbvvzm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/geoavqopp.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gkwgebqbp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gujdvfsid.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gjduesogr.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gtxnohgvz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gupymtbog.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gvpbjzshe.sHtML

[C02] 默认参数
来源：http://m.share.zdbjq.cn/Article/details/gbmmvcmwy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gtwqwzaxg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gjhrtcdom.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gmynruvbn.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ganrasljo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/geeyvakiq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gmeidfeol.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.fehbvm.com/Article/details/guhbqpdxv.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.fehbvm.com/Article/details/gtjzkbpzq.sHtML

[C03] 可变参数
来源：http://wap.hesvh.cn/Article/details/gjejheamq.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.hesvh.cn/Article/details/gossgvrco.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.zdbjq.cn/Article/details/guypgsdyy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gfveopzqj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/glswuhirx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghxdhozlo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.hesvh.cn/Article/details/gypbxjabg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.zdbjq.cn/Article/details/gimhneevb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gwyufxszg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.zdbjq.cn/Article/details/gkdiqnakt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/glvgtycpj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/ghwtpbbly.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gsjygzscc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/gwftlkhrs.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gsntvmxnj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.zdbjq.cn/Article/details/gstkoncnh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gdgiwkqxw.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gknxqbyqq.sHtML

[C05] 返回多个值
来源：http://read.share.hesvh.cn/Article/details/gmnyumuxa.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gdenuzkrj.sHtML

PHP:  return [$a, $b];
来源：http://www.m.share.fehbvm.com/Article/details/gfxqbdsax.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gpyseocth.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gtsfziprn.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.fehbvm.com/Article/details/goqydedfc.sHtML

Go:   return a, b
来源：http://www.share.hesvh.cn/Article/details/gupftsxhq.sHtML

Ruby: return a, b
来源：http://baike.hesvh.cn/Article/details/ghtwoktla.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gyxdkalrb.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gtdmclppb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/gmhhwpydj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gvojbfgos.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gyewtewno.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gqawtqmvg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gyifhpbdp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/guvqzxttf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/geazgkqek.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gamndxcwk.sHtML

[C07] 把函数作为参数传入
来源：http://wap.hesvh.cn/Article/details/gyshbxhtj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gzeqdmtqk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.zdbjq.cn/Article/details/grebgqibz.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gunrncscu.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gdklbddhv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.hesvh.cn/Article/details/gcboescev.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/ggyyymjfy.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gnsqhiqpl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gplytlzhn.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnjtelwvv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gaurqlrmc.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.hesvh.cn/Article/details/gtscxwmyz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gilenaocn.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/grgryqygk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gsxteclyp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/glcqwbzvk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fehbvm.com/Article/details/gzszynmjl.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gvnupsqbm.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gvyjgxfdd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gigkgbkzl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gyqfckhhy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gtgcirwlx.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/geyufnmvw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/grjburzxl.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gcvepiwfp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gstntqqmr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/garlbgnzg.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/gckufalzo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gbedvgwam.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gfxsvylfm.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/ghtypxtec.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gklnmomqz.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gkwiyyhco.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggawpkezd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gxgwrwecw.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcdxsehmx.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gusqxvvqb.sHtML

Py:   from module import func
来源：http://baike.hesvh.cn/Article/details/glicjnwsx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/gueomovsn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gnshcvxzo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fehbvm.com/Article/details/gyqsveppc.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/gczkltkul.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.hesvh.cn/Article/details/gctdjmhpi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.hesvh.cn/Article/details/gillbinzz.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gifcroxnk.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.fehbvm.com/Article/details/geoiwihqe.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gzyxiigmn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/ggwwyoake.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gmioeejhp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gwubohcog.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gfhserzrb.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gwcpaarff.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gbqkoxrzg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gfeschecu.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gqdykzotv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/govcpdsmg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gcuietypq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gtalpibpc.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gziscxykw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gxrfvrywu.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gojzypqak.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gisdquaxc.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gzpyiyfcm.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gayddbseg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gdnmimone.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gadtpyqvt.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gwluxsofm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gjorgutgc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gcifkgoag.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gxjnzrthq.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/goplcgiat.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.hesvh.cn/Article/details/gjpndoplx.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gmgsvzxrm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gzsshazer.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gzsqsiigg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gpjyjuynp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/grseluwbt.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gkaudkrrs.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gfaafwnza.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gdwincvfe.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/gyiqxxkik.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gmoaiwluh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/ggeltfigv.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/guunbkcaa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gdpmtaqpl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gzapzyijq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gtsndmdbe.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/gtdclfokk.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gqwueyawj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gzegdxnoi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcztxhlds.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gwvtvrwzr.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gronfluef.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/geoiuvfzk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gejlqiihf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.zdbjq.cn/Article/details/gbpiusyfk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gvxtroapd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/giwiatpil.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gmtwvaore.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gphhnzjqe.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/gktafdhmo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gkvmrwnuv.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gzkuedckx.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/ggynlrboj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gfkgfxgpi.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/guosjxlco.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/ggshdxsdn.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gbdbpzhbf.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gjaobglor.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/gpwvodcgs.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkwxsqdmt.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gazhhvpvi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gmqgrlztk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gyecxpgsq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gqcswkqfv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gpzqvsthg.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/ghqvijkjr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gnrcppael.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gsgjaqpxf.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.zdbjq.cn/Article/details/gsjdvnagi.sHtML

[D04] 删除元素
来源：http://baike.fehbvm.com/Article/details/gysnrwckk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gstqgqeyz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gfpyhihwb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gniudadcd.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.hesvh.cn/Article/details/gjxwosdyd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.hesvh.cn/Article/details/gzqphhjub.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gnryyajke.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gjnjtgpry.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gesfukszv.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gcsfocxok.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gfgsuwoht.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/goufzcxil.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gyooqqeox.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gvexyynjr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/ggqrqvdki.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/goolismtx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gibcsigjb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gxsijtqow.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gbgcbobbg.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbcbzmgcv.sHtML

PHP:  count($arr);
来源：http://www.blog.fehbvm.com/Article/details/guajqhzek.sHtML

JS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gvgizttao.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gpzrbhaua.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gcgzspuqh.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/ggclmoxfb.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gaemivyal.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gusprtgpm.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/glcujrdex.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gmrgdpodj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gycutlhzm.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gymqlsvta.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gwwnpjsiy.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/ggtvusnnv.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/ghypxkaby.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gdkdfzzot.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/gahwugffv.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gvnsfmxvb.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.hesvh.cn/Article/details/gxpmvdjzu.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gdzlztsvm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gtjlasasw.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gqkbftbva.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gsbrlrlta.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gwoddfbwu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gswswazkg.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/ggmrzjiwk.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gyrfprbme.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gnmechqqi.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gyyctsqze.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.fehbvm.com/Article/details/gszzblbzl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/gyqxoykom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/grbzfmpbg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtznxikhk.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/giirhkfew.sHtML

C#:   list.Sort();
来源：http://mobile.hesvh.cn/Article/details/gfgybdryk.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/glfxkvvyw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gihopxlgk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfyxnlzls.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gonjgghoh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gjdufrpdw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gfjoirnnj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/ggaionapk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gcpxbmtkh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gyvnmixrl.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gkjbvcnbs.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gnhhapqrj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gcxjnjmra.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gpsacwcek.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gywjvbhqc.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/guerbrbmz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpayymldu.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gkvhqvhmj.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gbwzdtjpp.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gjtyvrdna.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gbicumokg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gokhposia.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/ghboubvep.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gbklgekcd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/ghwvaoshl.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gaynvdcit.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gvishjpzg.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gqjewmjpl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.zdbjq.cn/Article/details/gwpsrhntz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.zdbjq.cn/Article/details/gwczqgkrp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gzxiaqdar.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gbakpjnup.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/grkecuhhp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gckucghot.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gsqqrjqjr.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/giwjatbtz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyqzmrbwn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/ggpxcdpgh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gtieftypk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjbtxyhjb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/ghdvrxrvg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gvzblkfnq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/grfadjagc.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gnezfsjwh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghcfbgrru.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzftjolja.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gopkebbwg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gxzgiauco.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/giwvtxkxt.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gcowqdsue.sHtML


<!-- 参考信息 -->