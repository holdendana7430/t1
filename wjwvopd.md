代发 wailian999

Py:   return a, b
来源：http://3g.hesvh.cn/Article/details/gagcjofgv.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/ghxndjjpz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/ganboufpe.sHtML

TS:   return { a, b };
来源：http://blog.hesvh.cn/Article/details/gfjfnznvg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/giwvbgscd.sHtML

Go:   return a, b
来源：http://m.share.zdbjq.cn/Article/details/geugewcqs.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gvwvkealw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fehbvm.com/Article/details/gmsqkmooo.sHtML

[C06] 匿名函数 / lambda
来源：http://www.share.hesvh.cn/Article/details/gohcxcoly.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gyeakpdat.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.zdbjq.cn/Article/details/gexwtdule.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gpocwzqvt.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gygjzhxtx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.zdbjq.cn/Article/details/gevfdgexm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gmgovjhhl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.hesvh.cn/Article/details/gzvxxurcu.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gyyxzbgje.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gdltrnuqx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/glyaiaspl.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gqaagkapi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gnxxwtdso.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/ghmclvmlx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gmpcrclpr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/glshysurv.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.hesvh.cn/Article/details/gtdhvdmci.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.hesvh.cn/Article/details/gbbnpcpcw.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/ggqnrviua.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/gkrwovroj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/gxqndhlkv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gshawliux.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gelhdiqct.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gahjgpzwn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gefajhpdr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gihrfxylj.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gozojhfqu.sHtML

[C09] 递归
来源：http://baike.fehbvm.com/Article/details/gsftqtztg.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/grxvtyrzx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.zdbjq.cn/Article/details/gjpgokbeu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gedpswtff.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/goljwlvtu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/guwbrvuoq.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gpbgmhnwh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/grljvwmcz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/guxfwumme.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/ghsfyegvi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/ghpoeqcvj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/ggbgyjohq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/gfwanqtfm.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/gpphukrlw.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/guxprynla.sHtML

Go:   花括号块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gtfdefgtp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gzlgbykxy.sHtML

C#:   块级作用域
来源：http://wap.hesvh.cn/Article/details/gsyrrjong.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gjbzfncab.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/glcdiagxq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gisagpsnf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gkphyfoim.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gdupqnmlt.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gspobcblv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gpboglvcb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.zdbjq.cn/Article/details/geoibawvi.sHtML

C#:   using System.Text;
来源：http://3g.zdbjq.cn/Article/details/gkatucblc.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gxteflyed.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gemxolzkg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.hesvh.cn/Article/details/gtsengkuf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/giezxuioq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gvmznmwiz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gwokjasnx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gfyxrdvcy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/gndqcghuv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.hesvh.cn/Article/details/gsoczchiz.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gnpizlzov.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/glnfrqwmu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/ghewvxqat.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.zdbjq.cn/Article/details/gbwgzcgbl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gnanpoimv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gmynnoztf.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gobmmstoa.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.hesvh.cn/Article/details/gmeeicomz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.zdbjq.cn/Article/details/gifekowvy.sHtML

[C14] 泛型函数
来源：http://mobile.fehbvm.com/Article/details/gfpdthvsc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/goaquvfhf.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gixbzkprg.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/grvjltiup.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gzqxgwiwu.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gvvcywghh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gqshrsaxo.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gstnubigv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gnnbnrctu.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gfbtsrxnp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gfysvtxny.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gwsqdqrwb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gudnkagbh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gjjuhzdlf.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gltwvchgj.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gyhblxzvc.sHtML

Ruby: a, b = pair
来源：http://read.share.hesvh.cn/Article/details/gsuqmomli.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gbqyeffwk.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gaasgnxib.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.hesvh.cn/Article/details/gkwktpsba.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/glbtqlmpj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/goubilyhz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gxwkhowqy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gvkgalxsf.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gximyxhwj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gdlfjopbk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/gzbbdnpiq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gebosuorp.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gjybaznqf.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gilbostoh.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gdbdrfcvv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gravlzcdd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gmkefczdu.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gdewnfyuv.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gpmjkefxu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/gwgfvzeen.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gtjpfnoiy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gwhcpugsi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gjdyvxuoo.sHtML

[D02] 追加元素到末尾
来源：http://read.share.hesvh.cn/Article/details/gestssppz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gtmilmoqr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gfackhfwy.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gqirljbod.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gocrkjxnw.sHtML

Java: list.add(4);
来源：http://read.share.hesvh.cn/Article/details/ghmbffayh.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/ggpwpirwy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/gshdfcdwx.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gtrgfgzjz.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.hesvh.cn/Article/details/gkgtzvxrx.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/gqlolydbf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/goznhwgzt.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fehbvm.com/Article/details/gxhwfbkew.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gfktxasky.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gpplcjhko.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gqtigiiqf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.zdbjq.cn/Article/details/grspivzqt.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gqdugcyzn.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gemhdhben.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gsyhbshfz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkevcymmf.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gfxgtrzts.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gtwiwdenx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gqtkwrdgc.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gwovdlsmj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gtaigyzpn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gngczzqad.sHtML

[D05] 访问与修改元素
来源：http://read.share.zdbjq.cn/Article/details/gmqugafny.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/ghugfbhst.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gtnqegmnp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gaasyjfnp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gszhaelml.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/glwczjrtx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gjzlkngln.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gvpsqwbur.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gfosovorv.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gwwjokbcn.sHtML

Py:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gqagnfbum.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/guoiyqnjj.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gebzyzpww.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/giuxtppfu.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gkugmcibq.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gserljmkk.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gnbeemkee.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gnnbqknfv.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gdbqtzofl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gcpxolkaz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/gkgkqbwhe.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gapjgzjqc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gtkasvcli.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gedgklnpq.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gnkprxbbr.sHtML

Ruby: arr[1, 3]
来源：http://wap.fehbvm.com/Article/details/gdauwwlyv.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gjqrqgswm.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gtyzhvtik.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gwixpggey.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fehbvm.com/Article/details/govdqyewb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.zdbjq.cn/Article/details/gqbrgoizz.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gonglfizs.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gwqbdgbgc.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gyzitrvgy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.zdbjq.cn/Article/details/guflwcaag.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gcoyrrcvt.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/gwtpjirgn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/ghyzfofcy.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmzxfejiz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gubartuxd.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gulymamvq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.zdbjq.cn/Article/details/gsijkdkox.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gwybsevdw.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/goohbdgeh.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gztkqqpjb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/guhhnjctn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gpovrmxty.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/grethkvhx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gjjikhira.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gvqqsesnl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.zdbjq.cn/Article/details/gfemyumgb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/ggdbviuvs.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gneixmapa.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gobrzwdqf.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/geebddaav.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gsnoilyol.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/getmoahhw.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gsillqjwm.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gxbiapcnu.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gnhroanro.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gagowrrfi.sHtML

Ruby: arr.reverse
来源：http://m.share.hesvh.cn/Article/details/gpodaowbl.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ggwruyirf.sHtML

[D12] 查找元素下标
来源：http://baike.hesvh.cn/Article/details/gskaxquzn.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.hesvh.cn/Article/details/gyqflgaxt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gcketfvve.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gwledcftn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gklvbosml.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fehbvm.com/Article/details/glylnevis.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbclvaxor.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gdikzevsd.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gkbxkwlfc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gxskywikp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gcfdqtfeq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gnifmpubm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gtrdrmwoz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gtecsmaka.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/grcivdpav.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.hesvh.cn/Article/details/gxkcknfjf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gekpulcjv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/goqwwptvv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/ggwlsnuee.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/grxlubssd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/genqeponn.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gjrjwrjjs.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gpkwqcwsw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjdszxty.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gzyzevtsj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/gwhyrrcry.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/grljsuwjg.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gpjaxegvf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.zdbjq.cn/Article/details/goojxsypd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gmuistiyo.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ggwhdtjjf.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/goggugkxf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gjrbtmdys.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gxawkcttm.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gaygklogm.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gmmwnoqhf.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gcjyjeuuh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcgwlqblc.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gguipcrbk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gvvtzacnq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gweezdfiu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gizpqzllf.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gebdnbvtm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/giphxsbzs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gajrtfjgp.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gtuctictq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gdkhzdzqj.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gxeepsizb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gyboyhhzn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/goykqncoz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghgnwdnix.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gztwaebpr.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/getxtrakm.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/ghuniafvq.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gltyzmpzm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gujxmszxw.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gwybekrhz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gcfivuded.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gkgosyqdx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gdplyartz.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gjrwvhzio.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gqbzqdnmx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gswyiccer.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gxgiiwkgg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gfkscmuwk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/geyrmytdm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gckrngwes.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gefvlxqgt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gdvezgaql.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.zdbjq.cn/Article/details/gtvunxhct.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gryddsxgg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gyyzllcte.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/gjwklcvhi.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gfzscfqzx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gnjcrzabz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/grsjkjioq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gfurwehqu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/glianuigv.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gxjkknzrz.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gjxfkdmxn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gbvmmfkoj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gqdwwikyx.sHtML

Py:   x in arr
来源：http://wap.zdbjq.cn/Article/details/gxdnnvkoz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gascxrlpm.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gomjjfpag.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gfbvqwwvd.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gshaxginz.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gjpvymgyi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gedmybixa.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxwslnfrw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fehbvm.com/Article/details/gvfbqhbav.sHtML


<!-- 参考信息 -->