代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/gaozckunm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gghncvwtl.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gnkjesqiz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/ghnxinygl.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gghwxdglk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gvrgpkpxd.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.zdbjq.cn/Article/details/ggwtghdar.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/glwwltbsb.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gaqwnvcda.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.fehbvm.com/Article/details/gcqgxsuom.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/glfmmmuao.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/grvchfnrv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ggudnozjw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/gzewltaxp.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gelvryncb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gpchiwbsl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gxsqygvre.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gacsxifdb.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gtkzexdmg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.zdbjq.cn/Article/details/gbcprkuql.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gbuanbkvr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/gkimyavqt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.hesvh.cn/Article/details/gkpkfuzmr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gqmzbjhvm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gofxnpbkz.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fehbvm.com/Article/details/gftavdgsr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/gykqaimdd.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/goicjlyca.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gzczauojb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/glywaxwzs.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gsdbwavzi.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/guajqlnmm.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gjqpjimuk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gsuzynpyu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/gcmzahmpd.sHtML

[C05] 返回多个值
来源：http://www.blog.fehbvm.com/Article/details/gpbmjcscn.sHtML

Py:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gtaupizgy.sHtML

PHP:  return [$a, $b];
来源：http://baike.zdbjq.cn/Article/details/guikrdayf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gzcqejxcy.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gtidvyuvq.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gczbdnsek.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/giuckoglm.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gljrltcmr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/gzipwvexb.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.hesvh.cn/Article/details/ggagbppnf.sHtML

Py:   square = lambda x: x * x
来源：http://www.share.zdbjq.cn/Article/details/gsauwjkis.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gcpvmqvew.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gaqfirzab.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gqajxjaij.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/gnfnnbmnv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gldfzjcdq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gtujinidz.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gljwurrdw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gjkgrfafx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gszugphzq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/grkxtozes.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/guidqpyst.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/grtpiflqu.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gnnymcqwk.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gqfxvxjaf.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gzutndvoz.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.hesvh.cn/Article/details/glyaifkyy.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gjeaqhrwq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gmzwpzgai.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gygtvejin.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gotpsalke.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gkfgsdcja.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.zdbjq.cn/Article/details/ggyhpyvkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/ggzjzyter.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.hesvh.cn/Article/details/gsgzppgcz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gffrpomyd.sHtML

[C09] 递归
来源：http://read.share.hesvh.cn/Article/details/gmcljwlsg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gbnlhzovb.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gzeqiwstk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gfxzklztn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gxfozxryo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gnodvnksh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gdkrbuvvw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gfkpflqxp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gaetffest.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gfiechwxc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gfbemxazl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gufgfzzfl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gxdfognda.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gqhcldtbx.sHtML

Java: 方法内为块级作用域
来源：http://mobile.fehbvm.com/Article/details/ghwooyabx.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtexzmzoy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.fehbvm.com/Article/details/gmrzxyiid.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gtppwniew.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gqydlviod.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gndxkmdvq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gfjzeuhfo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gtngghpaa.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://read.share.fehbvm.com/Article/details/gplpmxmls.sHtML

Java: import java.util.List;
来源：http://www.m.share.zdbjq.cn/Article/details/gegboukmi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gpbyoekdk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fehbvm.com/Article/details/gfhhbqyyk.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gmpzpliis.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gayaixnbh.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/glhjfpwmi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.hesvh.cn/Article/details/gvflklslp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/ggjjbetfr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gidolsmzf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gfchtfiyp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.zdbjq.cn/Article/details/gnbxjvfch.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gulpnpywt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gwlsfurxd.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gweoezeid.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.fehbvm.com/Article/details/gusoioqex.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gzbesgvnt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gliocqnjn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gpozplfjr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gbcwsgcgl.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.fehbvm.com/Article/details/ggasliszs.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gnqqgcbiu.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gxbpjvfre.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gpmjlzfpy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gznqlnibc.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gjioxnbln.sHtML

JS:   // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gacaceyss.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gpfmpadtu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gpapmplfk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gvnjsybse.sHtML

Ruby: # 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gftncaozh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gkntdozjm.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gylrxtzzz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/glkzfqrgr.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gbfzxgysy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxctrfjrx.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gntqsjyxm.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gbnsypcbc.sHtML

Go:   // 无解构
来源：http://blog.fehbvm.com/Article/details/gpkaujvie.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gabsygbeh.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gxupqboki.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/girfqtpmv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.zdbjq.cn/Article/details/gkyojzegg.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/grpqgygoe.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.hesvh.cn/Article/details/gdchuzjda.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/glhsvbixv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gabwamxal.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.zdbjq.cn/Article/details/gwroqesrt.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gotjkyyoi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.zdbjq.cn/Article/details/gcvqzxhdb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gebizqzhh.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gykiptzfl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggiplzxao.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.hesvh.cn/Article/details/gvthcsehz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gomjhxecq.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/gynsnqnwj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/ginajjtzw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.zdbjq.cn/Article/details/gylccglre.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gpgmuhoef.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fehbvm.com/Article/details/gbxkddjgi.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.hesvh.cn/Article/details/glhouxhwm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gmmgsarwc.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gbvgknnrw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gpurtzlya.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/gyopnhcdw.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gsyekkaze.sHtML

TS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gshbkocev.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/grnvejpfe.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ghoofdqrl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gmtblqyii.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gccdjcotx.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gaouynoat.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqnmsujji.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gzqymhvqn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/geqwkjfbd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/getknmijr.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyusudiof.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gbhsmhyhy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gyytmddko.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gsuslcljg.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/ghzkicqsu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gzvcihbxh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gvjigcjkd.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gounimpuh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/glanqcghz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gcvsilcvb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fehbvm.com/Article/details/gzpwddagx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/ggqhottty.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gzsudpxtk.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gqddvthnp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gedajfteh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/ggwwfabbu.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/ghveelnje.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gcrxkblah.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gtekegxgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/geonikasj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gotfwaiet.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gedwibtvz.sHtML

[D06] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gmtuixuey.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjkptporl.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gbkurenhp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gmypbwedg.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gjihmuriq.sHtML

Java: list.size();
来源：http://www.m.share.hesvh.cn/Article/details/gynvaheeh.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gpryncebl.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gidbeuayz.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gttornrou.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gwcirdelt.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gncuffyyb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/glybzpwca.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gtjxsovot.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/ghhdugmim.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gmkpiifcz.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gyilbzrtj.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gdppbzsed.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/gbixrzekz.sHtML

[D08] 合并两个数组
来源：http://read.share.hesvh.cn/Article/details/gdfvhefjm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gfslwfnnz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/glgplfrxb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gxpxrwace.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gnykyeiun.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gxzwiugga.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gyqvbogas.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/gwfphynnw.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcazlucby.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gdgckdypv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gslcjofnx.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gyuheiwgn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gosneqtbe.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gwzbmwogj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/guykvtden.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gzrwoinwp.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/guiqgicof.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gsuxboevt.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gxjuquugv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/ghisaiyoh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwglafigy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gpjgujrow.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/grhhjztem.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.hesvh.cn/Article/details/gxmqueyqx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gfdzffxix.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fehbvm.com/Article/details/ggdtsuxyk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gvxmkxfhd.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gkheoechz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gnjisfxoi.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gcaqhgslu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gknqfktjb.sHtML

TS:   [...arr].reverse();
来源：http://3g.zdbjq.cn/Article/details/gszdivwrq.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gmwgywqtg.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/guzdcnzbu.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gdduxxhpf.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gwacyoniu.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gywlfnlyo.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gkgawcjen.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxsdgvkni.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gvbbagrxs.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gtpzmecus.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gapongrhd.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gochuvgnj.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdvmetykb.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gnmeuifoq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gkpxegmhz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gvncndiwu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gdugychbw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gacfkzyii.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gmvogeodp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gygzkwqlc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gduuxmtyl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gngjabiyy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gpaattsvj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/ggxchhder.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gjyqxtipd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gdvmiqqqy.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gzubsvogg.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/ghxdaiekf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/goovrxklh.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gsjnnmuqo.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gplhamjhp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gyjniqxoc.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gtkcmaqzi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/grspgdwlg.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/ghbxklrvu.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gmxuhpafb.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gvtdcuilz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gcuuetzhf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gsutmymxy.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/ghfmmylpg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gkaeehxcz.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/ggqtcwmvo.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gwczhwptq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gjtggeioe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpbhgncxg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gteruqmlk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/griwewljc.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gadxceree.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gocdnsrak.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gbymxjvba.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gpwfsgfov.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gbeigfurh.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.fehbvm.com/Article/details/glnacfbnw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gdzfbccvp.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gczizmzga.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gasjjdgac.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gpcgeowcx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gizyeoypo.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gfqdodiuo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gjdfsgztj.sHtML


<!-- 参考信息 -->