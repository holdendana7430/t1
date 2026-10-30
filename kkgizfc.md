代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.share.fehbvm.com/Article/details/gvnuenbhx.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gflwgljpk.sHtML

C#:   f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gpogajnbq.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gsxkbisbl.sHtML

Py:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/glgzbajtj.sHtML

PHP:  return [$a, $b];
来源：http://3g.zdbjq.cn/Article/details/gryopkctk.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gsjzzlhws.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/grcbzwfje.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gqqyuaunb.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gxqopkobe.sHtML

Ruby: return a, b
来源：http://www.share.fehbvm.com/Article/details/glefjwpaz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fehbvm.com/Article/details/gwhhpabrn.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/guodniorl.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gmqtzyjnf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gimhnyfeo.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gpzsfhhcg.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/gyhbyihqg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gagbbtjws.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.hesvh.cn/Article/details/gqbkthgso.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.fehbvm.com/Article/details/gllbbtnff.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gwcadjqhk.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gfnywbiuz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/ghxomwmcv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/gdkybvyik.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.zdbjq.cn/Article/details/gseirkpnf.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/gnvmjxqdp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gvkfnubih.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gogwbtohq.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fehbvm.com/Article/details/gjebbdwgf.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.zdbjq.cn/Article/details/gkddmtoek.sHtML

[C08] 闭包
来源：http://baike.zdbjq.cn/Article/details/gnrxwxwzw.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/glimbswbv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/gltcnjmbp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gurtvihow.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gpizinswt.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.hesvh.cn/Article/details/gbashereg.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gtehhuxuc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://3g.fehbvm.com/Article/details/gfoxmowvr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gozyqoxsy.sHtML

[C09] 递归
来源：http://www.blog.fehbvm.com/Article/details/gufvegojr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gupcvycgt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gaslvpfle.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/glnwvnfha.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gnwnfylnh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtlenvsvb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/gwnlzhbeb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gubwmsllx.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gyzdxfiio.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gjklkfwgd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/gfvifouyk.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.zdbjq.cn/Article/details/gigrwrrir.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.zdbjq.cn/Article/details/grxitcyki.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gbdftrvnx.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/gvrfqmmzq.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gjkneahyg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gckhnctwq.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gwgsdcvns.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/gvqawhkbq.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gokzepkyz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gvzlpdlur.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/ggvgcrzpy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gcdegkjvs.sHtML

Java: import java.util.List;
来源：http://mobile.zdbjq.cn/Article/details/ghiwwssqd.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/glwrigclf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/grxtakuzi.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gnalbmpeu.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/grpyglydi.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/ghaswxkfs.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/ggemektpt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gzffufjgh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gsjpubvmg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gdkszjbic.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/ggvsxwiij.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/geubbvvsc.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gelxbudar.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/gorwxddri.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.hesvh.cn/Article/details/gzwrkkvkh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gthzoxawp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/ghzjdvlkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghtqodyrf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gdvphgvat.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gxevcrfsg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpusuojzq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gvgnjgrhg.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/gnkelvndz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/guvzdpnhw.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/griqfzrdp.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gmuqgdwek.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.zdbjq.cn/Article/details/gmpckfriq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gxemaqeak.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gwnddciqo.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gghushkvu.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gclvurwan.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.zdbjq.cn/Article/details/gpeuoxpmm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gctcqmjln.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gcqjioxqs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gooxqtvgd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gumoxsczo.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/ghaeostuu.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/geiumwewv.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gudtupbrp.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/gvzlcqdda.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gfaskhmvh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gokmwezqi.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gnwqcxwwc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gevevlmtz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gsymjlcsm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gzdwpldjr.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/ggclhsmas.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gcpuiezql.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gwrosvgna.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/glbtkuusr.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/gntjwvvqp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gctzwyxan.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/guinvnuhm.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/gvpdqjtad.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/garpasjep.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gmuolxaxn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gvwnebtsx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gqgwnhhde.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/ghxbnbtyt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fehbvm.com/Article/details/gpltvewps.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gjhbhcids.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/gebbhvcxh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/grclirdjx.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fehbvm.com/Article/details/gwnhbifye.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gqdeskekz.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gtfdvsnfh.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gvxadhnpu.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfdzytadd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gntjifhma.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gziwdzlki.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gieuegyom.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gcuenrkbu.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gjlfukapb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.hesvh.cn/Article/details/gbnnfnaff.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gguuafdts.sHtML

Java: list.add(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gwssyonue.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gycfomsmd.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/gbcjvzgpl.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gyuivqljc.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gzlbagfpz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gqwiawgtr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.fehbvm.com/Article/details/gzyaskwmi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.m.share.zdbjq.cn/Article/details/gypjjqctn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gscssmpvf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gujmlqxaj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gnxjdphsl.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ganaeqqac.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/ghnpnvxcd.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gshvgnpjn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gdtiyhnxc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gfwvjifay.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gvffhhdoi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/glmcfadtv.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/ghftvzhjz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gaharwflq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gddkhrxop.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gbhxrbrpb.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/grcapiveu.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfivhcfbz.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gcyxxells.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gchbumlts.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/grsxfplzm.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/grimqarpa.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gvlyzflyh.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gvzkjulvi.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gnhgnwwiw.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/giieujeqs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.fehbvm.com/Article/details/glbuzkosi.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gwkxpmrlx.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gdowzlzhx.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/grfhvkleq.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gynhfccdr.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gjkqijfnb.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gslwilpnk.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gnmyagmdc.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/gbusxmwlj.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fehbvm.com/Article/details/gdovxbdzz.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gwhpljpxb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/gsfatjjsn.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/giqradbaf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.hesvh.cn/Article/details/giuathrqv.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/ghvfslqno.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gplfafspv.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/geptisstx.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/gaqnpkaiu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gnocckvzc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gscefhbmo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gyxrgxjrh.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/glcykxdfa.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gnwmdopuy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/grtbxfjat.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvtboxvtm.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gwpjnavgh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gmfgjekio.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gpmtlwphk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gjumnkuzl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gfvjladnp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gzhauafys.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gxkglcfya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gmunhjnic.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/glylrsmmt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gjraxzqdl.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gnpwswywm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gewrzzxve.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gijwnbcow.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gcdcfjmth.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/ghchzokls.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gcxoajani.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gtojtcrxc.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gmmlffdsl.sHtML

C#:   list.Reverse();
来源：http://mobile.zdbjq.cn/Article/details/gfiifzggj.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gpndhjjmm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gpupxppte.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gtitefzgc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gpggydaoq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gvbxpkmfg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gnvzjwqig.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gyhzzmzhh.sHtML

Ruby: arr.index(x)
来源：http://www.share.fehbvm.com/Article/details/gitqytffr.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.zdbjq.cn/Article/details/gpokgnwwu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gyofhhfej.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gblbzyfxg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gifbyafbg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gyrxeqbej.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gghzzqtyp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/glxvhtisf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/gwgwfcecd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gtekaesqd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gzvizaohg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/grrposjoi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.zdbjq.cn/Article/details/gwnrrhctr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gvyxlzsyr.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/glzltchja.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/guwhqtyxb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.zdbjq.cn/Article/details/gkpdowqkt.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gwynhsghm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gxutbohiw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gjmircctw.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gkapbmprd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.zdbjq.cn/Article/details/geuicjson.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ganvjyhin.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gmxehpozy.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gizdcwiqh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fehbvm.com/Article/details/gnugwhjtp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gyuosrdoz.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/ghafiqbia.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gdodgalfy.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gzztwbsqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gewdzbygs.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gesltaphc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gimmlaabf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gfsczlnox.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gvlkfdmsw.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gqdvhlxwz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gmbatzpwb.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gwhpeviuo.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gjmenhdqp.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gdypdrcss.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gvwycvlvm.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gqeawlwjb.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/grkauejob.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gzwgzresw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gppaqltwd.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gtofajsko.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fehbvm.com/Article/details/gayfbmise.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gtxotstzv.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gfesjgtok.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.hesvh.cn/Article/details/goizwvfhm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/ggmwckdyh.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gmlqlfwhz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/glkksnjzf.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gmahwzwhd.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gaiyavebi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gpxfnobph.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gygjvgqgo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gkxkkwjrj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gkprqftpc.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/grugmgdwr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gbbxlxckz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gdwfsizns.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gckvjxtji.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/gurcvdihw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gposixwjh.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.hesvh.cn/Article/details/gjdfrzdqs.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjilgurbp.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/gsinbjpvu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gevwweehe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gxifbmuzy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gnwdbtpdi.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gatjbjoki.sHtML

Ruby: arr.tally
来源：http://baike.zdbjq.cn/Article/details/gbhueghzb.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/geohavwfz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gliqtjsfa.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gryuwsgiy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gupmkarte.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gytvaoepv.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gyifpaenn.sHtML

Java: list.contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdcurjal.sHtML


<!-- 参考信息 -->