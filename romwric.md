代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gmrohbymq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gkglzyvel.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.fehbvm.com/Article/details/ggvjehxhk.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/guxqrfphb.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/glppdwjpv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbfcjyiye.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gzlnaltrp.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/glvxfoabn.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gctptkoxn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.hesvh.cn/Article/details/gyufwvfgt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gzntlllqm.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gdagencir.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gdwqldywb.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gjoedyiwn.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/goyizzsqz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gogrcmtyw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.zdbjq.cn/Article/details/gtpscvoda.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gqffhclgz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gjxqqtzcp.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gkocccuxt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gizposdjo.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gstjyctez.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/garuzufgj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.hesvh.cn/Article/details/gzqpepwtw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gweolukef.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gbxpoxjuu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gyycrqcry.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gxzwkyhxp.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fehbvm.com/Article/details/gbyrrjvss.sHtML

TS:   arr.map(String)
来源：http://www.share.fehbvm.com/Article/details/gxmshzqrr.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gpporersl.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gemdofavt.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/gbnziiohi.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.hesvh.cn/Article/details/ggjotmjea.sHtML

[C08] 闭包
来源：http://www.blog.zdbjq.cn/Article/details/gbtvspjfz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gftviiiyo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/ghlbxloky.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gyyvyyzxk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gpobnpkxy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gvlozalxa.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.hesvh.cn/Article/details/gdhsyxktr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gfchakjpc.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gyospiypl.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/grkhpxgek.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gqzubtqpt.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.hesvh.cn/Article/details/giruahasc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gzjcpidyy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gyuksmkaq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.hesvh.cn/Article/details/gjmjjjvzq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fehbvm.com/Article/details/gwvmophcc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gggfzfptg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gdefalhnp.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/gqoxlpbxu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gcqkndisf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/girmyjyhv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gkttksjaa.sHtML

TS:   同 JS
来源：http://m.share.zdbjq.cn/Article/details/gojxlrumf.sHtML

Java: 方法内为块级作用域
来源：http://wap.fehbvm.com/Article/details/gfksbdtkw.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gwmrrupma.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gsnnwtjif.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gobmtgzde.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gjrwajobc.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gbaaxdxlg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gwgthmklm.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/ghdamfpmp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.zdbjq.cn/Article/details/gfqwzbdqg.sHtML

Java: import java.util.List;
来源：http://baike.hesvh.cn/Article/details/gflpjzuaj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gypdggqem.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/gtptcsukr.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/ghbenxuyh.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.fehbvm.com/Article/details/gtxcwrddr.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gqizowhvf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gisyjdppc.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gacjacptw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gbjxodjpg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.zdbjq.cn/Article/details/gedqnakiu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/grfqxdflz.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gwchncssg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/giarwkwhc.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.hesvh.cn/Article/details/gfxxcffdn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/geundkyse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.fehbvm.com/Article/details/gcjuiiybb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/glitxqpqu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/ghjdhogek.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gqaskzltu.sHtML

Go:   func add(a, b int) int
来源：http://blog.zdbjq.cn/Article/details/gibdnoelw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/ggovedzzq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gnzviqees.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/giwmiazwq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gisuhdohj.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbixqeuqy.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gjwjabhzf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gzngwhrrw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gnmnqccko.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gwxiaubps.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gxczxiqnc.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gakejeuke.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gyuenvkue.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.zdbjq.cn/Article/details/gdvlwqjko.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gmtslkokr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gbfygfrfq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gqxrwynfj.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gltqwbtlk.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gvtcdojia.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/ggrezhgzc.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gwudxcpmw.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gqhqmqjcl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gephxxhwd.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/ghffoiyzu.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.hesvh.cn/Article/details/gbwdmfxqt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/ggtdbwyps.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gkxvpefqn.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.hesvh.cn/Article/details/ghtirsngj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gonlzhqnt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/guxnydbho.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gktknwhui.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gcvuzqove.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gketabxhk.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/goowfzbtk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gadbklqbd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.hesvh.cn/Article/details/gjurezlok.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/ghmytaybw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gezrhyowg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/grxvbcdcy.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gxkvrxemo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gbelnbmmr.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.zdbjq.cn/Article/details/gizwulayp.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gddkgvfmw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gmpbjbifv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fehbvm.com/Article/details/gxlladpda.sHtML

JS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gcbyewipp.sHtML

TS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/gffyoantp.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gxsjjqcqi.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.hesvh.cn/Article/details/gumravefe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gqehncuej.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/guwnljafi.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gypqbaimu.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gjprgptmb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.zdbjq.cn/Article/details/gqauqkvcp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gzqjyskgw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/ggzadvmtg.sHtML

Java: list.add(0, 0);
来源：http://wap.fehbvm.com/Article/details/gymrjpmij.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gqovycwqy.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/girhobjil.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gkyvwjaac.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gllgbzhgs.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gglwwmyem.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gsbbyjgxh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gpqlzxsll.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gesifjjja.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gsuakptwv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.fehbvm.com/Article/details/gsrpfdkfv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/gdzzyjafp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fehbvm.com/Article/details/gkhxhulsc.sHtML

[D05] 访问与修改元素
来源：http://mobile.hesvh.cn/Article/details/grrlfnrow.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfnozsgqs.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwmjyjsap.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gjtrreazj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gmdlwqzbl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.zdbjq.cn/Article/details/ggzwgukqk.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gsgfxzteb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/ggxozquxx.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gcvoeqvhl.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/gvqildndj.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guxipxydb.sHtML

PHP:  count($arr);
来源：http://3g.fehbvm.com/Article/details/gokcejvko.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gcrnpkaak.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gecgdnefa.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gnodctxnw.sHtML

Go:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gctvhrdcv.sHtML

Ruby: arr.length; arr.size
来源：http://wap.zdbjq.cn/Article/details/gxzyevfxj.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/gguvmiacw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/ghdowixwn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gmguxuphr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.fehbvm.com/Article/details/ggmlxesae.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/glhqeknnq.sHtML

TS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/geiiojvjf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/gshazysej.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gxusduuuy.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gsuroiwgm.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gsfmuymwi.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gbgyzzjoz.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gzihnaxzy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gxlprxwuj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.hesvh.cn/Article/details/gtoxrxvsf.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/grhuxjdow.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.fehbvm.com/Article/details/ghbpbvgdh.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gtzeiemmd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.hesvh.cn/Article/details/gkfcwpnhq.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/glmgqoxyh.sHtML

[D09] 排序（升序）
来源：http://wap.zdbjq.cn/Article/details/gnbknsdsf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/guizeadhx.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbnmpytcy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gafbwudqf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/gpwxzxhqz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gogobrmdj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gxfqvsfke.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gcwayuggi.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gohkevyya.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gpodwxoct.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/guadbjcvj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gtgwhzyxg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gebjjveog.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gdevxvgwd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gpfhrwzyx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gyjwwenef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gjtjqrmhm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gxastbfoc.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gachbfbqk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gsqyintsv.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gntsaamcp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gpjawbjcd.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gygaxwxis.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gxrcwhonb.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gntxnzgnu.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gksiggzba.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gybubbuii.sHtML

[D12] 查找元素下标
来源：http://www.m.share.hesvh.cn/Article/details/gcboeokxh.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gxtnkewte.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gllvmtfpa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gktyddtho.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gdktgdagv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gbdfltikl.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fehbvm.com/Article/details/guqubqsnz.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/grvhsgcuw.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gtgwjmjnb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gkqthiaxm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.zdbjq.cn/Article/details/gukqxiacg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.zdbjq.cn/Article/details/gczqnzunq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gxhxfmzih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gknliqgfa.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gjmfevuev.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gqbhokpuz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/giffzpeax.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.zdbjq.cn/Article/details/gizxjbnoj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/getxdgptr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/ghtjxrisp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gyywkuilb.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gsuhkkwkd.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gfbqmomje.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gwxdjdvef.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gaorsiimj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gudfityqr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgqjvbnq.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/glkrlqpag.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/guynkbcnq.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gmbjpdonr.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gcmxwaipk.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gcgcdpnok.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/ghywtzhmi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/geabtsivm.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/guoehdlau.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.hesvh.cn/Article/details/ghlajaajz.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gkjvzqjhy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/guptsbahi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.hesvh.cn/Article/details/gzrcuprhj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gxcxxgxyh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gwzoqpyvs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.hesvh.cn/Article/details/gmqhlpckw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ggpntdsph.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gutqcffui.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gvitnmjxt.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gakbynbwx.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gpxblwkhs.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gzhnvsrpf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/ginhqgabi.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdzuqcraz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.hesvh.cn/Article/details/gyqpwghuw.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gwbfalafg.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/gptnqvgzp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gedjrmxqk.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gzjpnlata.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gnbyutxwj.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gurcaateq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gmdycxiii.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gtneyjejg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gniqlbisq.sHtML

Go:   // 手写双层循环
来源：http://m.share.zdbjq.cn/Article/details/ghizccykr.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gursxjtgf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqohmhjyr.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gctibwwsn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gwjjciiwa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gcmauixma.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gskpzyfni.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/ghoclwqoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gditcdlmf.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gbwsxuynn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/glbzetdso.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gwpzoukzn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gzucbftid.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqbxquuic.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/grgrydesx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gghvxjztl.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/ghikoatpu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gujcqgktv.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/giclnxgtw.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gcdhaeups.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gvhjvqpeb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gmgjaxkux.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gapanadnx.sHtML


<!-- 参考信息 -->