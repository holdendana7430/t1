代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gmpoqxovb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ghfqjfssb.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gkkazuhof.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.fehbvm.com/Article/details/gctljhhqw.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.zdbjq.cn/Article/details/gxxsjksvz.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/grxjwxncx.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gjqgsksst.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gwruvlmcr.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/grnlxhnzu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gmhrlpuim.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gfqfdfvhm.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/grqtzpolv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/geiviyxch.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/ginbwktml.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/grlqsohvc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gvlrpppic.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fehbvm.com/Article/details/gmconmqaw.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gwjgfjgpu.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gnqprvnwy.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gaeyuhcey.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gewzmovyc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gdigajnqe.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gricpjzkl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/geilxizdr.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gtrdudfzk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.fehbvm.com/Article/details/gamhbdmit.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gtphvsmxn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/grzhckksf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gdlhuobxl.sHtML

TS:   arr.map(String)
来源：http://blog.fehbvm.com/Article/details/gierwjhve.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gcoljmlsg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gzydcqapn.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gpqusqtqo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.zdbjq.cn/Article/details/gfehcftmi.sHtML

[C08] 闭包
来源：http://mobile.zdbjq.cn/Article/details/gqjmpyfsf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gcczyqofg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.zdbjq.cn/Article/details/gywpccexe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gcdishhec.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gyvzdrwbd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.hesvh.cn/Article/details/gtzsneobh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.fehbvm.com/Article/details/gqxjabjkn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gsyxldjch.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gkyomtqdi.sHtML

[C09] 递归
来源：http://blog.zdbjq.cn/Article/details/guzcegfss.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gutkrcxqo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gijgtgshf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gvxjqpshh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gtdhrtrzk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gyhatuyhm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gsyvcohqi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/grfdenfet.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gldkgrtfj.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/geggqyqcc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.hesvh.cn/Article/details/gpkhiesaa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gtcphvyfj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gfmzrtdpe.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/gyreovhux.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/guctsbxin.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/giutfwgtw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gvvefzlmu.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gafgxwbyo.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gmmnpqezg.sHtML

Py:   from module import func
来源：http://3g.zdbjq.cn/Article/details/gqomyikwt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.fehbvm.com/Article/details/gnapswqjy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gzqspjazq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gggnfhbvh.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gryfecqxe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gjokxtldh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gteqlwpkh.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gaaqahkag.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gensgfxit.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gbhpaiwro.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gjawgcgqd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gcazbedxg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gwpctbcnq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/gbrzveeuj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gdfazqcnr.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/gwxmuezer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gqsvtudhe.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gdgysqnif.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gmniwppvb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/geocrzhmw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/ghbwhdoqh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqyhyfuwu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/glvdzrehi.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gwuebsbij.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/ghpcgcquo.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/ghykdjial.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/ghcoxzwfg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gtjuxvtxa.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gdolwsrgn.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/govgernlj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gewantidx.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/gybwupnoy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fehbvm.com/Article/details/gomxahrbm.sHtML

Ruby: # 无泛型
来源：http://read.share.hesvh.cn/Article/details/gjspgcwte.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.zdbjq.cn/Article/details/grhcncmmn.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/ghhroudqs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fehbvm.com/Article/details/gjhrolnfg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.zdbjq.cn/Article/details/gqxvwrdeo.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/gerdpfgki.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/glueqmzsn.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gdrvqjizb.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gyhezmecr.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gpwmnsnvu.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/glfjpxlsk.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fehbvm.com/Article/details/guiqhjdss.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.hesvh.cn/Article/details/gnrirnxir.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/ggqpbeehy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gjlkemqni.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gkirilovg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/glbelrjwt.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gfvqdlaay.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fehbvm.com/Article/details/gfmejgdhd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gnelhiuen.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ginqibheo.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/gxpvtcynz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gaymroucp.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/gndkoekod.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/ghpknrqpz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gsboprpda.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gwyjpcnkj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gglktvmqx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gvqtixkmr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/glhfwnabh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gfvwlcqkk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fehbvm.com/Article/details/gbbrvubiz.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gahvtrsnn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gcsjiqkwz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gzehsdiop.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ggfredokp.sHtML

TS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/guwlonncn.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gjeckatbz.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gmngolqbd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/glewlgsta.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gkczcdkbm.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gsbgrslvi.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/gbdarseuj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gzbvjptir.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gfzcczejp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.hesvh.cn/Article/details/gsigwvonv.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwctkypbs.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gdapbhusc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gtdtamaki.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gjohnlula.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/gobpjnmee.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.zdbjq.cn/Article/details/gsuzgdbtp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gkjiuigqe.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/grqpzdbnv.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.fehbvm.com/Article/details/gfbdigpiw.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://baike.zdbjq.cn/Article/details/gqhwcwmqi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/ghijczjmj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/gaqwqbieu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.hesvh.cn/Article/details/gtkvjxofc.sHtML

[D05] 访问与修改元素
来源：http://3g.zdbjq.cn/Article/details/gehsehqjk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gwrmmiwoj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gbdfbwvjo.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/glqeskfip.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gbwqjhphd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gwwkybbin.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gyccibity.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gptklreme.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfcxdazkr.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gampqsaua.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gkhovdgxs.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/gdowyphdm.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gwketszhm.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gggimspal.sHtML

Java: list.size();
来源：http://mobile.hesvh.cn/Article/details/gziorcqvm.sHtML

Go:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gdnohhnuo.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gwyjwlhqe.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gpczbiken.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gdyezbpnn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gexubdupv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/grlugblue.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gzsjvgxay.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gecqdosax.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gxztuekep.sHtML

Go:   arr[1:4]
来源：http://www.share.fehbvm.com/Article/details/gishrwkrx.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gprgrbfvn.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gmxatrnag.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/ghwnhhehm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.hesvh.cn/Article/details/ghuhppbuo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gsuddtujt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gffyvccqe.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gmgksxlbn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gicnzfljz.sHtML

Go:   append(a, b...)
来源：http://www.m.share.hesvh.cn/Article/details/gzxgjyeno.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gtejtqiyp.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkwlksupy.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/gnzdgjnsg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gviuayjhg.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gwqsmfqub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.hesvh.cn/Article/details/gjcpaygqs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/grzlbukre.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gxmkcfkuj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/ggtypghny.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/guumwpxfc.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gnwodxffl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/givucjfrb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/glzppbqqk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/grkikebfp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gwupngvfg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/grjnxntyy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gbhlsugfa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/glpoyveck.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gctdiqflr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/goblaemav.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gsimlvmqo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.hesvh.cn/Article/details/gzexqqprm.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gdcgilctn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gueywxlhx.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gzoyewxkl.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gzfiycxpn.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.hesvh.cn/Article/details/gaxunuyxg.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gkbenvcgd.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gucrourhv.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/girklffgl.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gdmzjdqgp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.hesvh.cn/Article/details/garlnvklp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/ghqaaaqlq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gkgfrniem.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gadwmqvzk.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/ghvyxiemt.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gefedqfdo.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gxwghoeda.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gitepiqta.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/grlgiixlt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gqhcufsik.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gcvneomtz.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gigatsklm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghqfugqhp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gtawrzfod.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gelprmntt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gbgxslnvg.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.fehbvm.com/Article/details/gwqmcasxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gielworvo.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gybvphbus.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gexixbaqq.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/guhqchkfy.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gxppehefv.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gxykpkhbj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gcoqqqulv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlszlxb.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/giurhncmm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsqiltbah.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gdcskoqab.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gyjpvddly.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gqmgfixdk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghsixcweu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gkwqgzkaf.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gtpxpjldz.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gjekpybbk.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/ghjoagcnk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/grgsbsyjy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gkcfzpisx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gfcfeaxhm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gebhjgyfk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gamcaxvyn.sHtML

Go:   // 手写循环累加
来源：http://mobile.hesvh.cn/Article/details/gvgstvqbk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/grabubjvb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gbmkwkwth.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gifgspmxr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gbuofkuun.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/grnanvrsb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gyrztpvfc.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gjsxwzlil.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/glvwcbsog.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvatqxglp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.zdbjq.cn/Article/details/gthimsfhi.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/ggahcemzg.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gkglprxrc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.hesvh.cn/Article/details/gdemtelve.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gcmlxrwdf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gnlukiidh.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gahkrteyw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gkavuetjs.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/ghbdntofk.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/geqyihayb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gyswnogel.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gifnvlukt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/grhnjkppl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/glcksmnif.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/ghjblevdd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gptirhhvw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gzaeiajml.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gyniovkkp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.zdbjq.cn/Article/details/gmymixixz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/ghrqhllex.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gbnubqmuc.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gjthfmwei.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gbhynrszk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/giniezqsv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gsdcaxmit.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gxyvmjqol.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gknxoxppu.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gkfxkjtph.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gcpftftts.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gdrpqhprg.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gzqluxzan.sHtML


<!-- 参考信息 -->