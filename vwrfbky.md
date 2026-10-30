代发 wailian999

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/ghbbwggoy.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/ggjczcwvx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.zdbjq.cn/Article/details/galmuzdup.sHtML

TS:   return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gezxrrpvo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.hesvh.cn/Article/details/gszqyekpa.sHtML

Go:   return a, b
来源：http://www.m.share.hesvh.cn/Article/details/grrcqzing.sHtML

Ruby: return a, b
来源：http://baike.zdbjq.cn/Article/details/gdnfdgzph.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/guwmmviyj.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gbliestbe.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/ghacocucu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.hesvh.cn/Article/details/gwbzqqwsg.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gmapikwss.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gpwjxiomz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.hesvh.cn/Article/details/gktjukcgf.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.fehbvm.com/Article/details/gioclgatv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gdzlxrxho.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gztacmnqk.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.hesvh.cn/Article/details/gqrivtlte.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gjxnhyuag.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/ggzbaildq.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gfyszrxsh.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/gddnzgxkk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/ggdcriiyt.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.zdbjq.cn/Article/details/gyzpazrlt.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gguqslnqs.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gxynbgkoj.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gjtuznoww.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gzbnpibii.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.hesvh.cn/Article/details/gvqwjcovd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gqmthhlsx.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gpitznnwc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.fehbvm.com/Article/details/govmvpnnl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/gmztwwhxh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/ggeetwdyb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gqpeuvoyr.sHtML

[C09] 递归
来源：http://3g.zdbjq.cn/Article/details/gtffdfzjk.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.fehbvm.com/Article/details/gbdoulvfx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gvlhpkhwz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gthilfxid.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/glbtagslf.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gfbjxlfjm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fehbvm.com/Article/details/gvmwzapry.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gnfrdpitj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gcajumuse.sHtML

[C10] 变量作用域
来源：http://www.blog.fehbvm.com/Article/details/glkbyyfqv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.hesvh.cn/Article/details/gowytlxfb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/glptmcqgz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.zdbjq.cn/Article/details/gthqaznla.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gowwupqcw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gemalpivi.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/ghaywdybb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/ggfkcgbhk.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gavvmlkdp.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gpaihekhm.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/ghfwveeqn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.zdbjq.cn/Article/details/gpjeyzxhp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/glwrkbclq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gimevmtxk.sHtML

Java: import java.util.List;
来源：http://read.share.zdbjq.cn/Article/details/ggmxfvspg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/gccmqjoea.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gdpirbzqk.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gguhthvek.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gayagdoao.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/glwbgmbcw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gxltyjsuj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gapxoqzdv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gzbqxtiqs.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/ghtwmammn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gkqnanyzs.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gqdocdgur.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvoqfkeay.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gdopftqzo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gzeuzkctv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/geltlnfqn.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gozywkgjs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gxctrfjhw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gdpcumeve.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.hesvh.cn/Article/details/gdhzpqkwx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gyatjjlfz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gxyfecake.sHtML

[C14] 泛型函数
来源：http://www.share.zdbjq.cn/Article/details/gtnwimvas.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gsgfazufg.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/guwqzyoms.sHtML

JS:   // 无泛型
来源：http://blog.hesvh.cn/Article/details/gggxkebcz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gfxzmqopl.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gbmyrzfmq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gsamnrtez.sHtML

Ruby: # 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gaqvgomca.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gupafxrdv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gapbcvziv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gzbzvqvwj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gvysrvdxs.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gnstpobdm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gxwepaodp.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gvrbxnjkl.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gasxpalfn.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/grmonukxy.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.zdbjq.cn/Article/details/gqvsvcpno.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fehbvm.com/Article/details/gxnazgepq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gqexbnhim.sHtML

PHP:  // 无重载
来源：http://read.share.hesvh.cn/Article/details/gktqfidkr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.fehbvm.com/Article/details/gdhdqhnli.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gspcefmnq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/gpuobcsyo.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gguazzrwy.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gwbhyuvzi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gplncxgyo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmfglhqxz.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gnbmhezgv.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsopsvynw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.fehbvm.com/Article/details/gvnwtbgft.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gberbncko.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gjbkmaiqt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.hesvh.cn/Article/details/grgnhllwu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gsgwomgqr.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.hesvh.cn/Article/details/gavdjzwgc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/gaxwlgvrg.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gemntahlo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gxqzevdxz.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gyyfuqbwl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/gucfbgeho.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gagahjtkj.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gytmkzmte.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gkyhuqzqb.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/ggqgcbhkx.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.zdbjq.cn/Article/details/gzgzgismy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gbibohwba.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/ggknqanqh.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gqjvjxhnp.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gxbjvsuup.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gsrtaonml.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gaqbsgrul.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.zdbjq.cn/Article/details/gbqspavce.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/ggvpzjoao.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/gspuyattc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gxbkwbgjw.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gupsxvhyl.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gsdwvksug.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gqwfcsfus.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ggqiaacqi.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gvjtvmasa.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gxllxfswm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gzhbowhla.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gvmqgoksz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/grbewkkbs.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.zdbjq.cn/Article/details/gdzjhfxbm.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/grpomrdmv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/ghnaclmhm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gpzjwbrim.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmwktmgq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gujsmdmzp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gjfiiwwzc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gxnzirmnq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ghcvlmsqe.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.hesvh.cn/Article/details/ginoutnar.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/grprcghqo.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/glrhvtflw.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/gqcdxeocj.sHtML

JS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gsqyfmvli.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gpuizgqpp.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gjdlvezzn.sHtML

Go:   len(arr)
来源：http://blog.zdbjq.cn/Article/details/grguybxif.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gwsopislm.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gjsbpqtkg.sHtML

[D07] 切片 / 取子数组
来源：http://blog.hesvh.cn/Article/details/gznsvjkiu.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/gsygmjfae.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gbosvbfuo.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gwiizrqxr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.hesvh.cn/Article/details/giibwsnyo.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gthpvlbfu.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/ggkftrmkj.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/grgnconzd.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/goutahosn.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gwaypcylt.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/grtqmbobr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gveiisafi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fehbvm.com/Article/details/gqkpoktak.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/goqaviwgv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gjsenlemw.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gpnsqfeah.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gkyjwafza.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gztkyjdns.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gtylkcvvh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gxlbdmuwv.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/ggndeyhrx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/giucquqoi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gtvbbgmdi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gwlmpyjol.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/ghqungftc.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gsamutwzp.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gegyhrssl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.hesvh.cn/Article/details/gwsbiflme.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gflqgwlwv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gxemwtump.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gzfqdqvpr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gojjhugqb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gjierlfzz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.hesvh.cn/Article/details/gfwfmtgpj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/ghjreymwe.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.fehbvm.com/Article/details/gcskxgiix.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/gbxltvdwd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gjxkjelyj.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqyuqnhdc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gjybbuoem.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gwvcylugj.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/ggfqdnhet.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gecfjvxqn.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/guuhmboba.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/glfhiajar.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/ghktdsvjc.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gqvokyozw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gtptbandn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gspecsntc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/ghzfblnew.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/grcxsbctr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ghopneobg.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gwtznszyy.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gcedycdjl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/glbhhqixc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gzbkaqujv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/giihfcwng.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/giluhaqgm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gfbinyfzp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/grvwqhdvs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/golpdxobe.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gsumvrzlc.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gcbgdnjqe.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/ggldaaqlv.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gooutyogt.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfjcypuwt.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gpmjhibru.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gwdfmostm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gtlrhfdqb.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gouhepecb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gcxyurryw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/gcrmefbjg.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gzfkuqsco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gvteuumzy.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtqcvgbii.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gbsnvzpbh.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ggpzrcccu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/goruwtetu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gyfonfvgk.sHtML

Ruby: arr.uniq
来源：http://blog.fehbvm.com/Article/details/gzarjpxsh.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gbdenbtpe.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/gosrxumpp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyduilghf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/grtgmfsjk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gpkefudzy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gtrpzjqme.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gaehcguwt.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gvlntzvsb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gxxbqvwfm.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/ghlqimcbu.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gaxnfyxok.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwaskvqcy.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gkasgoayj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gatkbmdub.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/guognaaec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gkvttldyz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gupgbdank.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/grlodhkfc.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gwziuhcrw.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/goaktkarg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gomzoqbim.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/guqaykhkz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/ggrmxiakr.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/gntjiyock.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glvqywtmv.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gzrhawvbb.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gtvvjdzhz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gptlegtdt.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gkcfeveyj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gmkadkvam.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gyewcknqn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gawpeftqv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gvytrersr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/ggxyulrzn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/glszyuihi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gofvlpviu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gccmiqejy.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gteitgzxx.sHtML

Py:   Counter(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmtluctvx.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/grvyckhfn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcqxnuyfh.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gvxiqnuti.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/gjhotjmly.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gesqutlku.sHtML

Ruby: arr.tally
来源：http://m.share.fehbvm.com/Article/details/gfjupyvms.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gwajxcmst.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gdoqclian.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gldgpqhgt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gytnxpumk.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gpreuokqv.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkcjnufkk.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gkpkjjdhk.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gjqhzeqrd.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gtezmvpgd.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/geolajnnt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/ghxuuysxw.sHtML


<!-- 参考信息 -->