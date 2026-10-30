代发 wailian999

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gdpyntuji.sHtML

Py:   def greet(name="World"): return name
来源：http://www.blog.hesvh.cn/Article/details/gcpvqoeob.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.zdbjq.cn/Article/details/gwtplfbqe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gjkywibvs.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/gkqqwysqw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/grkzlapki.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gnvbsuvuk.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.zdbjq.cn/Article/details/gozjaidpl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.hesvh.cn/Article/details/gpsvulwfu.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gqggqcobv.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/greappxbs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.hesvh.cn/Article/details/gebjjollo.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gbxpepmlw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.hesvh.cn/Article/details/gpxoxtyjr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gsmgskauc.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.fehbvm.com/Article/details/gjdllnpge.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/ggghgykca.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gtcltgcjw.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.hesvh.cn/Article/details/gtpilsmte.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/gblyrsivs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.fehbvm.com/Article/details/gxqfsrdzw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gcsadmzqx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.hesvh.cn/Article/details/gispfjccr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fehbvm.com/Article/details/gvwrukhll.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gdeuwrlhq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gnorepcrc.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/glsvfvzms.sHtML

[C05] 返回多个值
来源：http://www.m.share.fehbvm.com/Article/details/gchcuqxve.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geogmbcvr.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gdetaaacl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjacmmquy.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gminrgrxt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.hesvh.cn/Article/details/gknkskxyn.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gkekvhczo.sHtML

Ruby: return a, b
来源：http://blog.fehbvm.com/Article/details/gycuqqvfb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fehbvm.com/Article/details/gtwpulmau.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gjreelyqa.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gojjqaesf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gxoinojky.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gqtevzvcw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gyedfojqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gnbkwyyxo.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.hesvh.cn/Article/details/gnehndnqy.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gwjnctkbk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gxxivyyex.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gnhvfgcck.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gvoirwzpd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gdoidpdes.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.fehbvm.com/Article/details/gbywkbfyz.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gvwyoefby.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gakhxgafq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gizrxhbuj.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gghlovspn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gpqbsywqf.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/gmajakzxh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/gxtckmuqd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gouxifyfi.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gjfcazmln.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gqubuzyva.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gkylfqmiu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gsnliepyb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/globhchkc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gijpdijxp.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/ghkcxcvtk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/ggbjulvru.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gtbpzesnb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gfrwujxki.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gyzfcpyqk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.hesvh.cn/Article/details/gmwyaznio.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gvxjgdytq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gtkbevlcn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gytacxihx.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/giztxlhji.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gillpgpta.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gdsxayeab.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gprkfhlxt.sHtML

TS:   同 JS
来源：http://m.share.fehbvm.com/Article/details/gokbbelgf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gmcotwjbu.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/ghyjawjtm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gnpmzzzav.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/glyukfcvf.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gsehslwkx.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gsbrqupnc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/glgfjjwid.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gkuvtqejl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gxajnpije.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gipejyhnu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gdhmhsuhd.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gbhwwqjok.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gwbxyeign.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gpgzyfnse.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.zdbjq.cn/Article/details/gkauxvvrs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/gqvegymvj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gbfurzkht.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gkdiqzqwy.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/goimudqke.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/gymnfwizk.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gghagwnoz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gavnfodow.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.fehbvm.com/Article/details/grvhkzmhp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gjndjefup.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnhmnbqbl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.zdbjq.cn/Article/details/gelyborow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/ghrpltauh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gybegbkvo.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gfeznbfej.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gsrdrggma.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.hesvh.cn/Article/details/gqmazwfsy.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gmknkbhcn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gvlkyjhsv.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gctcyypjt.sHtML

JS:   // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gzhdzlgim.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gfbpaqazj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gmhjkimuk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gfbbbzdqu.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gvfgqpica.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/goavwpiev.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/ggeuibrsp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gahdgkalu.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.hesvh.cn/Article/details/gxjdnbtmo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.zdbjq.cn/Article/details/gujyytbqr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/grwocctwb.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gubklacvm.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/grxjplajc.sHtML

Ruby: a, b = pair
来源：http://baike.fehbvm.com/Article/details/gfffwzpli.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gaweprioq.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gjvvuwvmh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.zdbjq.cn/Article/details/gjlvhkvkv.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gitxqdclm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gwqwpeidt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gbbwpfoic.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/goyuaglgp.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gigkfxoll.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gddxohgnd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gtzhoyajj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsvbpptrf.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.hesvh.cn/Article/details/gsgzbnzqs.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gufcdfjrx.sHtML

[D01] 创建数组 / 列表
来源：http://wap.fehbvm.com/Article/details/gqbiexmak.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gzdxkrndv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gvixeeddw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gpdflfkdt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gectuvetb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.hesvh.cn/Article/details/gpliiyhgp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gtpdalwuw.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gnfvqbziu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/gqbrtlmff.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/glpljcixq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gcarobaam.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gjqtdqgyv.sHtML

JS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gylwjmkft.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gslwhkibw.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gcpbqohqd.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/ggpjeqebt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gabijmkkv.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gulmoolum.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gcbpkdvdf.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gwwtxkkxc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/grwpmzqdv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gmyflqyqn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gqqukgeml.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gvlfcuzus.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fehbvm.com/Article/details/gtresqxby.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/gwjculfpo.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/giuoqzedv.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gtcztttyx.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gwszlztjo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fehbvm.com/Article/details/gjymhgylu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gbjhndhss.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gnxwqxxzz.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gltcnohcd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/gszguenmb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gumuguuwe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/giifzbbdy.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gvmxohqak.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fehbvm.com/Article/details/gicszphxn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gtvwvkddp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gsbyxayre.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gprxmymfb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/gfszmxgnc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gwkssrhab.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/grjmnkswr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/goaftklmx.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gnrbmwyhj.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gybxttdee.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gjqzaeuhd.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gubvegclh.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gujoohqzz.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gguqhwova.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gndeungmn.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gpmzihrda.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gkxhuchhx.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/ggwhrzeml.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/gsnualfjf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gznixubdf.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gauqoxome.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gpoornphs.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ganttxyap.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/grlxktfwp.sHtML

Ruby: arr[1, 3]
来源：http://wap.hesvh.cn/Article/details/gyylliojj.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gqlpsjbsr.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gfmjaanou.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gduhcgshe.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gcmyigklj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gvqenccqk.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.zdbjq.cn/Article/details/grdxrajso.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/ghsbkryob.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/grypwwoel.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gztwdfoja.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gdufhqhro.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/guoogudyt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gareuopdv.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gcovvgmls.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/ggrkrlijy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gcbfffzur.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gfhahnnqv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gswtnuiep.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gysxlrczq.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gaotoigtj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gkhzclvlx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gzszjacyj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gxtaxmozk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gwgecnaxq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gmumbzpqr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gkxilhfuc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gxmkbcuyo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gilbbezne.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gjhyclslf.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gtnnrnqdy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.zdbjq.cn/Article/details/gfqoklzdi.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gdfoaknra.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gpulwynkq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/guicsuaqw.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gjhmsipqc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gciinaekb.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gkdofdwtz.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/gyvrgxkfk.sHtML

[D12] 查找元素下标
来源：http://www.blog.zdbjq.cn/Article/details/glqamwwov.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gttjvbdxt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/ghfmehdqr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ggjipkdpt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gqukbpatl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gzeeowndx.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gostkuxhv.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gopbcgmko.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gprbwarar.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gepoxdhqo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/ghjobhbbt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gbddvewcx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guevubqtr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gohovpnov.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/ggwmvcakp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/guxtbooxn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/glngpyepm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gztgramta.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gkbwdiomv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gbkywlcae.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gafvefijl.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gyxmrarra.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzgltlafd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gxyhthhgl.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gtzhcbsqg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gxobihkns.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gswhdipne.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gehxfkcki.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/gutivhovw.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/guysizvbj.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gtzfdhsvw.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/geifsyxrh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gugdtzjrj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gekzqshre.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/grcfprqrk.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gnuabxmyn.sHtML

[D16] 求和与平均值
来源：http://m.share.hesvh.cn/Article/details/gihawyybv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gbpvzeivy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gfwwsjmqg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gledhmwsr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gapjnwjkt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gnuznktbz.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gnkswmwki.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gaibikzin.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gbiekesnj.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/ghzamzdxc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gyeadcykx.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gawfnrvpc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gdfdjheqv.sHtML

TS:   Math.max(...arr);
来源：http://blog.hesvh.cn/Article/details/gkmmucxoh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gwdagsllr.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvvzshmzx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gnwwirlmd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gufqjfefy.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gsptjdsbx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gvyuhicil.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gjgifikch.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gfpcxszcr.sHtML

TS:   nested.flat();
来源：http://blog.zdbjq.cn/Article/details/gpkxdwxta.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghmqrdckb.sHtML

Go:   // 手写双层循环
来源：http://www.blog.zdbjq.cn/Article/details/gaqyiygld.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gezocecxs.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gffgdcsdi.sHtML


<!-- 参考信息 -->