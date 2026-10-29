代发 wailian999

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbomwjwcu.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/geyfxjjhz.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gblrkhuvw.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gwpsnsgqw.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gxeztrhob.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gjobqnfpu.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/ggxrunxob.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gwaiuawya.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gipelrrmd.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.fehbvm.com/Article/details/gqalcrxdm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.fehbvm.com/Article/details/gaqbxxgqb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsupledyx.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gbbzjbxix.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/girjzvrka.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gfuwlnzou.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gesdvyjbp.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gnpluhmys.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gsvqfsgdl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.hesvh.cn/Article/details/gszlceszb.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gftwywqec.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/glidfljof.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gcpmiynlj.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gsfqxzlqk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.zdbjq.cn/Article/details/gsxgtkzmx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gybcluyfc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/gijcjmdcb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.zdbjq.cn/Article/details/geiumtnbl.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/grsdvisoq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gfpjenlqg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gxldoquzx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gfndrbcwi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.hesvh.cn/Article/details/gyuqdxxqb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gclmgsbfj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gjndnucts.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/goaabyjxv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/guclckigy.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gkeujnjln.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/gqfacmcor.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gcqbmprbd.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gsmtgdttj.sHtML

Py:   return a, b
来源：http://blog.fehbvm.com/Article/details/gyankzhqh.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gwoelhrvi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gkhqdjdja.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/glmahithe.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gxmshkgph.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gawxzurvk.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/guuwiakka.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gmoatchfh.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gsvogcojb.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gkwpbmbvz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fehbvm.com/Article/details/gqwlssoen.sHtML

JS:   const square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gdmaeivof.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.hesvh.cn/Article/details/gtkeuvpfy.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/grvmjryqy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gyapmluog.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gillyigdl.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/guqvvenic.sHtML

[C07] 把函数作为参数传入
来源：http://baike.hesvh.cn/Article/details/gnnkkecae.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/grozhsyqh.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ghkqrmkzx.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/ghgnqueug.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gzxffwybn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.zdbjq.cn/Article/details/gveamqdvn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/grwogijuk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/giqyxfkub.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gplamghwh.sHtML

[C08] 闭包
来源：http://m.share.zdbjq.cn/Article/details/gdjyjduam.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gmniynwkp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gmnpckgse.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gaznfarxx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gfewjukzd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gqenihwgt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gjlsiqplv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/ghfjobngo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gnkxaurvy.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gcvwwajnk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gffcypgjh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gqmoqpfom.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gotjheslt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gncefzmdr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gyjnbpbkz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/giczkiyza.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gewcvzicb.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/geobhcpap.sHtML

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gsntxekco.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.fehbvm.com/Article/details/gnbafzien.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.zdbjq.cn/Article/details/gvqwitfig.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gigyszreh.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/guouincnp.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/gzyszsynn.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gqhtfwbji.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gsemidsnu.sHtML

C#:   块级作用域
来源：http://www.share.hesvh.cn/Article/details/gibejcmnf.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gqnbtbfwm.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gclnxubhd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/ghoxtjrhi.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gsfeddszi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.zdbjq.cn/Article/details/goqtqzcxu.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gkahnoyvo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gjqqcmcmn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.hesvh.cn/Article/details/gvnptrvhz.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gspowmsdp.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gcqtuepml.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/grpoxmgqb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gtqugqfyw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gbkxxagiz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/ghkkhfnts.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/gnwjznizc.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gxzjwllys.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gwjmcpbyu.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gwslzwkcx.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gbuveqgtg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.fehbvm.com/Article/details/gqkkvgjpi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gkzltsmla.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gvtxacsqf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gclwzjnbe.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gqcrogleq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gjeppfiex.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gbfeewhjl.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gxqzwspov.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gubcaiueq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.hesvh.cn/Article/details/gwiciifgu.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gwqitsmtj.sHtML

JS:   // 无泛型
来源：http://read.share.fehbvm.com/Article/details/girzktkox.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/guwimwqxe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gldvxsund.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gjcqfhfhb.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gxzsenqad.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/ggptxjgui.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fehbvm.com/Article/details/gikzfgzxc.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gnanwaoil.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gvaqdekri.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gjjqdygtp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcqtacrwd.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gqvyynzov.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/grvkmvrmw.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/giiqfdtsy.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gujsndbuu.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/ghqerflnm.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/grnattpvb.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/guzaysnaa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gouyeeeex.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/grsohvqeh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.hesvh.cn/Article/details/griexmttl.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gwkxbiniq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gqnhyojyk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gfkodurah.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/graqjdqxx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.hesvh.cn/Article/details/gzvhljqao.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gohzatjsc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/grmszuvoh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gsswaobqc.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gsfejmwcl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gnbgltukh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gqzagsxls.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gttylpqrq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gfbdfoqps.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/gfksqglmg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gdhszzpya.sHtML

[D02] 追加元素到末尾
来源：http://blog.zdbjq.cn/Article/details/gkswezwnn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gtuiujpii.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gkefdisoy.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gqoegxous.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gfjhbfwud.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gtfoajhjt.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gxbycvgob.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gxdeaxhdo.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gcwfnpejq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gbvqyypxd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glzrzjrfz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gwewtnkqu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/glavaymot.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gxfkdynay.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/geytgfdyz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/glawfjtqv.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gbcigwijk.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gctralsvy.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gmuahpjpp.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gaulhkvsj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/gdgtdweuu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gtsdbykpr.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gvtapefjh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gqpbujhuj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/glvfophra.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gvdultbdk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gobvfuijv.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gzirrixmh.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gozqbiyrb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtgbcbfmq.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gappygwso.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/gxdyggajo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/glgoldjoc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gahydccyv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gtzbbzjxe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gfhafpfmj.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gbfwowfqf.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gcaozdehg.sHtML

PHP:  count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjrxwllvr.sHtML

JS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gqducljgt.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ggtbcmfmd.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gwlweocst.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gbecjgihh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fehbvm.com/Article/details/gntrgqimm.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gifutdqwp.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gbvzghnqs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/gulpvjrdb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gzojonatz.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gytnsxoxv.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gcmounkds.sHtML

Java: list.subList(1, 4);
来源：http://baike.hesvh.cn/Article/details/gmxzmqlxh.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/galfiebku.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gfjkafrnr.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/glctkvmmw.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gkmqwwxjw.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gbrcnatzr.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.fehbvm.com/Article/details/gejtoptgr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gdzxmughi.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gzuflvojz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gdavycyff.sHtML

Go:   append(a, b...)
来源：http://wap.fehbvm.com/Article/details/gmihzrfrl.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gosjtigxq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gylgfscsv.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gtspkocal.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/grlqlzkqa.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gldyrhgfw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gmrugmwxm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gtjopivmi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gkxdbgooc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gwiwdkpmr.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gzvdibsvo.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gofvtbiaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gzpecrbxu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gdlfstobi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gioujcmet.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gtflysctp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/guiaiycfh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.hesvh.cn/Article/details/gjpvhjprs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gnyrresnh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gvbmxwpkn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.fehbvm.com/Article/details/gagpkttux.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gspzcaupu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gkhxofdef.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gsjaxvyys.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gylecqecy.sHtML

TS:   [...arr].reverse();
来源：http://blog.fehbvm.com/Article/details/grxztengf.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvtgdguuv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gvfnstmcr.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gduzchpzl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gmguiutwi.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/gcujfoitk.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/galulshrx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gwneuqnem.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gbbckodbt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoxbepol.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gmeyqujlz.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gaxcrnatw.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gcyqtcyyg.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gvcwzrdxi.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.hesvh.cn/Article/details/gmbxtuilc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.hesvh.cn/Article/details/ghehrryvp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/glqqtzghv.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gzazdejgs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gqonmpmrk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gisimvwzm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gtscemtcu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gxolblzvm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gkvfpedkl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gxnminxav.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gjciqmsqz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gtkpgeibe.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/genftdptx.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmdnyqkno.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gshoxzrwk.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gygxwcwsd.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gdfyqqflw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gnznrqwjn.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gxkztyclh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gjfrnwfvc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gqeiedtze.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqthzgtoi.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gxbcdctiu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gvhqetbkk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/grlaokugx.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/geodjcycx.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gtdyuizhs.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/gyewateii.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/goooaaavg.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gxrlbpcpt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gurnaxpyf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gvxckgrmp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gbhbkdkut.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/glempzfra.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gwdjzpoei.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gntnptqvo.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gepeafifr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gbupoqytu.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvoydblzx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gyvogwktx.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gygczbvtm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gmdqnqufm.sHtML


<!-- 参考信息 -->