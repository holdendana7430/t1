代发 wailian999

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gnbncrtot.sHtML

PHP:  return [$a, $b];
来源：http://3g.fehbvm.com/Article/details/gzdoqdhje.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/googtsupk.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gmsaldnop.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/gjfvnhpbe.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/ggimorwao.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/grsfzcfvc.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gugkjsnqf.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.zdbjq.cn/Article/details/gbkntgssk.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.zdbjq.cn/Article/details/gxtxyxvgy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gdrfnqojz.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gyabgmjzq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/grscqsxoj.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/grngofkya.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://m.share.hesvh.cn/Article/details/ggsroqyub.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gebzvrqzj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggfosfrrw.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/ggoefcasr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.hesvh.cn/Article/details/gzejwlqvg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/ggkocaxwy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gymiclhzv.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gpkerhfhy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gcsesvoqf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.hesvh.cn/Article/details/getoivwxj.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gurtayfgt.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.hesvh.cn/Article/details/gucudflqr.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gajvyxthn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gdrsondbz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gfqnkcsab.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gmfakasit.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/gmxjbjamc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/ggmsqhvsn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.zdbjq.cn/Article/details/gskjfdnsf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.hesvh.cn/Article/details/gjqabzntf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gcwcwfimd.sHtML

[C09] 递归
来源：http://www.m.share.hesvh.cn/Article/details/gnxvuugtx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gqknnvyqu.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gtppwdsra.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gkgkfvave.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gjoovnaaw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/gzdywpaui.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.fehbvm.com/Article/details/gccfnrdur.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gevwliajo.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gyfkagtsm.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gmfnyjrxd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/gcgkphzmg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.hesvh.cn/Article/details/gcbrqdqoo.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/grdffyomi.sHtML

TS:   同 JS
来源：http://mobile.zdbjq.cn/Article/details/gugmxifon.sHtML

Java: 方法内为块级作用域
来源：http://3g.hesvh.cn/Article/details/gnnpjahxp.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/ghgpbshkv.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/gyqwdphab.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gerqutuvu.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gcctqqkdd.sHtML

Py:   from module import func
来源：http://read.share.fehbvm.com/Article/details/geuwkdoea.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gjrwnrsgu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gwitrqqog.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gyavwpydk.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gprrruztz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/geimevajf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gbozzogwc.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gtyfwrawj.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.hesvh.cn/Article/details/gdlzcwylw.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gzsuseglc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gpsrvzoga.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gzyfvvxhm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gcslzhznb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/gdhrfddjx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gohpuqnrl.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/goujnhrma.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gtecehive.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gtfoznygu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gpcvdhphd.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gnosepowd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gopdqpsez.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/guqltxfxk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/giveykopd.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/ggaaspkcm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gcdyqzlre.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gqdhqwxwo.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gkbimgbyt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/gymassohu.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gdhvzlnir.sHtML

JS:   // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gqigzhraj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.hesvh.cn/Article/details/gmmvhxbzm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gidmnmdzd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gmlbpvhcq.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/giprfpmqa.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/ghipiorey.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/ganpjpomv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gzuoqtspi.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gqxlstmou.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gbjixxzzy.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/gnwyoztsh.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/ggktbvbrn.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gneabwzzh.sHtML

Ruby: a, b = pair
来源：http://3g.zdbjq.cn/Article/details/gudgzjscz.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gmfgslawq.sHtML

[C16] 函数 / 方法重载
来源：http://baike.zdbjq.cn/Article/details/gbvwhpfyo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gsfouojmo.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/gqdarkefv.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/grnlaplij.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gsgwhemnf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.hesvh.cn/Article/details/gjxyjqvok.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/ggzcimgfa.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gqtpprvsv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqdgnvkya.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gklnzzmsm.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/ghwllwbwy.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjgiiuijp.sHtML

[D01] 创建数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gatlaiabn.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.hesvh.cn/Article/details/gzkbkvyui.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gbehfrnuq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gmydimapl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gibuvanfv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gzoscfvck.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.zdbjq.cn/Article/details/gubdhkndh.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/gezqoosqi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.fehbvm.com/Article/details/gphrcdwnx.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/guuoyccqf.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.hesvh.cn/Article/details/gqcxxgulw.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gflvzivij.sHtML

JS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/ghpbussgw.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/grhahbsjg.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gtevulxxd.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/gwlygbyzt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/ggzrbsdtw.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gjkhwkdds.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gnczjlxfu.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gmbofihrz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gouaoysdd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fehbvm.com/Article/details/gsybebmkk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gycoyjnvl.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gpkszqfwz.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gfnjajjnj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gazfsnjkd.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.hesvh.cn/Article/details/gopvbanyg.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/guupnqiuy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/gwzavwpsu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gdejvsosl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.fehbvm.com/Article/details/guxjueacx.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/glwvnjjrq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gnrrrrhhi.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gpezipzqq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gvgqdmvcp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/grrqtogzc.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gzmxqlqle.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfeychyog.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gqpsnpxxr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvedgwwze.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gpfbicnhh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gtyxliqor.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gucwljnxw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gdjzyrczy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/ghlxwrknd.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gxixmunyf.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gauqgneoc.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtzeumrhs.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gimlmtkpl.sHtML

TS:   arr.length
来源：http://mobile.hesvh.cn/Article/details/gqhpekgee.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggrzxcapp.sHtML

Go:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gfafqccsz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gwmhqgame.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gqgvvjtoy.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/gslfbejlj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gyrsxpgyh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gdonbpjsl.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gpqsybmld.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/ghqwulfuc.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gagztioch.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/grvuxdotq.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gcrbgcjtj.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gaxbzvnat.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gknygnfig.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/grqfguxli.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gexezrgcx.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fehbvm.com/Article/details/gmlofdkxu.sHtML

TS:   [...a, ...b];
来源：http://www.share.fehbvm.com/Article/details/grpxxcszn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxkdpdujo.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/ghpjiapvi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gzssudqxx.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/gpibdambt.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gmetncjnv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gxedfwleb.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gegxkvegm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/guklnssmz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gflcbzsjz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gkojvzsca.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gwlczcffx.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/ghzwjpztj.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gxokvlash.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gtlaygizs.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gibwiksil.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/glojuphbk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gmsvkoafh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ghsjlpnam.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/givcgpiit.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gnynbqvuo.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gowhswjbr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gghccbwrl.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gthzvrafm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gxwawyzvw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gazuertky.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.fehbvm.com/Article/details/gabhkxffu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gzkoipiaf.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gzeceaiyy.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gzpxqjqpy.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gsspskbjc.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gaxgliosy.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gfotkaiid.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gsxjdjjno.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.hesvh.cn/Article/details/gyzxnvzlr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gcftnbccg.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gujfndkdf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gkdquqtnt.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.hesvh.cn/Article/details/gzqfhomek.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gfvdvdqok.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/geiadfuur.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/gtcaggtcl.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gpwmufguv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/ggatrvzyw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/geqdqktvf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwtcbbqbw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gxgzmrexc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gzayhrxbz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.hesvh.cn/Article/details/gncvdehfl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/ggpewvkhs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gtgflbwpa.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gergtjnbi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gjxfourrw.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.fehbvm.com/Article/details/gpuyfmgic.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gghwffqwk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gbakmooad.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gmntazfih.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gpbdffxzq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gthfyrtrw.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gqccsmnvz.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gylqoattc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjykbwlwm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gwxsheelp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gubgizcqh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gvssszvut.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gzawvrcca.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/guswcrcoa.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.zdbjq.cn/Article/details/gyfyubabg.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/glkbhkflz.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtrocsmb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gaipkrlfy.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwihxwaee.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/ggpztlvdc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gzhbvzxcf.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gztegdxns.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gmpbvfjvk.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gxnedkiuf.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/guxdcawhn.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gwnkvqlip.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfkofdwgb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/glhvlpitx.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/guqlyxtlu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdvfokov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gmxlwqerc.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/grhsyhiga.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/goqyowxti.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gwslonyhp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/ggqpfnshk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gxjsijlqi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gxanqubtv.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/grymfapku.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gwupzxqsa.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/giduziwju.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/gcuytajda.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gteuizmzc.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gsldujors.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gsasrrcly.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gblokiiyg.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gjcwvqokg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gdatjzbqg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gyvhpzhle.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gqwgwsyzb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxlrocdxv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gvlzqgtzz.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gclhkmsrw.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqizznhaa.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gcwcykaef.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkmcgdvsi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gyhxwvjfh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gmsrgucxr.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gvvtcvyhh.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gqnbrzsnv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gttmjivxm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gkykckdrd.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/ggqrpnxao.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gmdowhnva.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gifsnuxrv.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzxacasow.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gslozmkwe.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ghldadbxo.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gkbaprzkj.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gsgzarcnj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.hesvh.cn/Article/details/gypvcrfgz.sHtML


<!-- 参考信息 -->