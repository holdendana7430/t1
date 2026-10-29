代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gkybmmqox.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gjpnlqlvy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gxetvazst.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gacvxtlzh.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/giuggzlkc.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.fehbvm.com/Article/details/gvwxjdwlf.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fehbvm.com/Article/details/gwmdjfmdn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfvokfugt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/glfzpajrr.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gdhmzcipi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.zdbjq.cn/Article/details/gxzyfatef.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.hesvh.cn/Article/details/gbuzlwvta.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gxaaqhmtf.sHtML

[C03] 可变参数
来源：http://wap.fehbvm.com/Article/details/gjluehtlm.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/guqzqqmtx.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gnbfkofha.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/ggqorgefi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gsxzksqay.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gkicwqrqn.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gczpizdik.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://read.share.hesvh.cn/Article/details/gpbleickx.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gybktjfjc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gudkxdzyo.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gglxbmnpe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gqvftagto.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/ggnxebbdf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.hesvh.cn/Article/details/grzkdwjnv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gewsbtztm.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gmyvewenh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gmtzkaosa.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhhntghv.sHtML

[C05] 返回多个值
来源：http://mobile.hesvh.cn/Article/details/gmnnjlizs.sHtML

Py:   return a, b
来源：http://wap.fehbvm.com/Article/details/glcfcpyiq.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gwypjwbgg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gkfjdbhnt.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gufylvzvo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gwlhadnxu.sHtML

Go:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gythtcded.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/gxykeugnk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gxmbdzmbl.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gmflfdtio.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fehbvm.com/Article/details/gohuwoavs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gdpfjmcbd.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gtmgvscry.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gwdlbbibp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gytifkrbq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gdjsbpxko.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gvikeeuyy.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://wap.fehbvm.com/Article/details/gknarjslo.sHtML

[C07] 把函数作为参数传入
来源：http://blog.zdbjq.cn/Article/details/goaiuyhwh.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.fehbvm.com/Article/details/grkiztkni.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gxvfcsgzc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.hesvh.cn/Article/details/gkwozzcid.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gubkzghew.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gbotmhmrn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gubfcfsvq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.hesvh.cn/Article/details/gyhdzjypv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gkyzmydxz.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gutzwoynl.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/gaafxkzjz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/gccsjtnbs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gpersuahd.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/ggdmkpimz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gltdtorxv.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.hesvh.cn/Article/details/gvkxapdlk.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gzwpwhizn.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gkvrwbrxb.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gebiqizng.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gsfwqlvtl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gfmjcgirp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/giedongrk.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gijpmahxu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpszndpei.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.zdbjq.cn/Article/details/gcxnrlygn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gtotuplnm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.hesvh.cn/Article/details/gfhmsqxfn.sHtML

[C10] 变量作用域
来源：http://www.share.hesvh.cn/Article/details/garyninqf.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/ggpilxnac.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/ghvsbexbo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gpobigwyw.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gqkxtwwfu.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gmnqogeex.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gfwtrdjgq.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gbvrllyfd.sHtML

C#:   块级作用域
来源：http://m.share.fehbvm.com/Article/details/gdbnmoowv.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/gjkjfalob.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/gacmnbshc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gtawrsvvf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gmosezvdw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gzwlyrtiw.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gjivurnxw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gatkfpqnh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.fehbvm.com/Article/details/goxwtdcnt.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/glutbioai.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/grhjrpndi.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gjwwyacuj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gkdsvowgk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gtzhkevrt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gurufiqcf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.zdbjq.cn/Article/details/gggxoughm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.hesvh.cn/Article/details/gajxfhxts.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gxmfbwuhm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gekejffcd.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gyujoemiz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.hesvh.cn/Article/details/gyvkkgkgv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gohesnjrs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gjvbbssta.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gnnuhqosl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gtgsmnvdw.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gvyrwrsbk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/ggpivcrwi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.zdbjq.cn/Article/details/gtpwitqcl.sHtML

[C14] 泛型函数
来源：http://wap.hesvh.cn/Article/details/gmceenytn.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gcxyhijem.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/geqknuapr.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gsroznyxh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gonawqhlp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/gwqtriqvl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gdbkzpndv.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/glvpyrprb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/ggwiqjbxu.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gcmsutmzy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gfftfacye.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gcimujvnp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gjgiiffny.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gjyfuilec.sHtML

Java: // 无解构
来源：http://read.share.hesvh.cn/Article/details/gbbawijnh.sHtML

Go:   // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gfwsatdkj.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gyxrsjdja.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gfrzbwzat.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.fehbvm.com/Article/details/gxlyfgkwe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/glethxglf.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gupdexecq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gtsplckrp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fehbvm.com/Article/details/gjxxfjncg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.fehbvm.com/Article/details/ggbcberqj.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/gshisxwdg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/geikxnoql.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.hesvh.cn/Article/details/gpitztwwy.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gyahfwqej.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/godlquyrw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gcexfofec.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gmrfhjjjm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gtycozhfg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gtjovkajz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/giecjscun.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/giesqrxkq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gzyetujen.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.fehbvm.com/Article/details/gopiosrlk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gcjjpixqt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/guybdncor.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/grpuvdjth.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.hesvh.cn/Article/details/gdbldfghn.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gcpumosxn.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/ganjqeksb.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/grdsoqyej.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gkesuzxds.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gvzjqrctt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gkiuqxvea.sHtML

C#:   list.Add(4);
来源：http://baike.zdbjq.cn/Article/details/gxdisxgen.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gjkrttxvr.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fehbvm.com/Article/details/gcgbycjfn.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gpzigomeu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gbksdkxfv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzplytuil.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/glrmvwgtw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gbxuicrrd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.fehbvm.com/Article/details/gngwzzrjr.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwepnkoru.sHtML

[D04] 删除元素
来源：http://www.blog.fehbvm.com/Article/details/gkzwxkkin.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gvruemhwy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtkjvohem.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gjevpofow.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gbtqmhecx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gdskmbilz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gzsoauucx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gztxofjoe.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gxqvhsjff.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/gjoljhymy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/grmxnnqne.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/grexswztp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/geulbqehz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gwokrehmi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/gooygrjbt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/gzwiemqwe.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gualqwwhy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gotxspyvm.sHtML

[D06] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gxjcfzihj.sHtML

Py:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdyelkffd.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfvciisfu.sHtML

JS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/ggswrumdo.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/grhpxhiiu.sHtML

Java: list.size();
来源：http://mobile.fehbvm.com/Article/details/gtyaznmvq.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gaaxdmgeo.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gjxrfebbg.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gxxfvzfdl.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.hesvh.cn/Article/details/guiaauxlz.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gtjjnltcj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gdaeqmrev.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gdubwlawn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/guftemisn.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzacwyjmb.sHtML

Go:   arr[1:4]
来源：http://mobile.zdbjq.cn/Article/details/ghgendfak.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gboterpuk.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/giftettye.sHtML

[D08] 合并两个数组
来源：http://read.share.fehbvm.com/Article/details/ghdcdirae.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/glulpjtxd.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/ghztxutih.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gedqrhqbk.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gxjmmzapo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gfwgdrpkl.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/guucfqgkt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/gftycejpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gcsudafqr.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gpjvzkhcm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gakabawve.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gunfpsmox.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/gppayyjav.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gdkemxslp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gyfdszdcy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gvcyhupxo.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gagrtsaqc.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/geijvxmdq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gwgdmbwak.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gyqeojomp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.hesvh.cn/Article/details/gcbzeigbv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gpcjthidf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gawtscpdd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gkttfluze.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gxupyxrtz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gpsqguihg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gbylwgslz.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/givmgareo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fehbvm.com/Article/details/gitafawdg.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gmawiincn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/ghouujflw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gcelcbnid.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gujumudwj.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/giucuqffe.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gdyxsyqsm.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gtynyfymm.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gdmhcxauq.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.zdbjq.cn/Article/details/gjlhtlfxi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjedxkcjx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/glzlefzji.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gsrhsrwwq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.hesvh.cn/Article/details/giqpqryes.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glvljlphj.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gksqgdpky.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gvefotufk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/glqsajcpy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gernqtjce.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gccnxsvnx.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/ggkaqqdcn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/godmbtowk.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gamoiphxi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/goxkgmipn.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/guanhpofn.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gmjacwewy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/guqjtkyes.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gkunxvkgp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvuxictpc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gvupiochd.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gpsliaach.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fehbvm.com/Article/details/ggahgvzey.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gsedytsyq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gyiaqabbp.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gumxippgn.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gzdwhllxw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gtbfolowd.sHtML

PHP:  array_unique($arr);
来源：http://3g.zdbjq.cn/Article/details/gslvyenra.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gskqsxzze.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gtmfkbifb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gjkntegmz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gqgixdyce.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gnjtnxoji.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fehbvm.com/Article/details/golntmhoj.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gxlmjncte.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwkxrunlo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gakbcyjbe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gqndnnxrh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gnljnqafd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gqtwyafuh.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gqvsqrokz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gjctjfbcg.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gzsnrwcxq.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gldvqxksl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gueepdynz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gndfalape.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gkcqnkqlw.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gqwvewkme.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/ghomiusix.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghjmwaarf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gptszhzir.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gcviebklg.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.hesvh.cn/Article/details/gduqlmeev.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/ghvpswkmy.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gozotvshb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gqpkoywnx.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gejnewhdo.sHtML


<!-- 参考信息 -->