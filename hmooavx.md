代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxihpslym.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/goohwmzwt.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gxbimfuxr.sHtML

[C05] 返回多个值
来源：http://m.share.fanxiaobao.xyz/Article/details/gerlbsrpe.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauekcaxs.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gynhkykog.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fanxiaobao.xyz/Article/details/gszjecyzu.sHtML

TS:   return { a, b };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gokbatbdk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fanxiaobao.xyz/Article/details/gmuswopfi.sHtML

Go:   return a, b
来源：http://baike.fanxiaobao.xyz/Article/details/ghhblthet.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdrhtprd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjmfimxp.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsilgppkp.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fanxiaobao.xyz/Article/details/glyhivgav.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmvfpslq.sHtML

JS:   const square = x => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/ggibxjtke.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gsxchndfd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gffrehdlm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.fanxiaobao.xyz/Article/details/gvjkbuoag.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmswlgbw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gcgnvygfd.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/guedxexpd.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbryofru.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnhgdwpd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtfpdmjr.sHtML

TS:   arr.map(String)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpruycryg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxxtyslq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fanxiaobao.xyz/Article/details/gzmonqqji.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fanxiaobao.xyz/Article/details/gshzjdygn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvahttag.sHtML

[C08] 闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcmwsqsg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgmiwxoi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gezdppxjc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnftfmqfq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gmhuvxdqj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwybhyap.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsehuwoz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gibouikpe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdajmvkpt.sHtML

[C09] 递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjxgkphb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwxzjpvf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbdswiteg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fanxiaobao.xyz/Article/details/gjzmddrln.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gulgyzjap.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjlkucfpj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfnujsoy.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpuptzoh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkssjdl.sHtML

[C10] 变量作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gzjdbjnio.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fanxiaobao.xyz/Article/details/gdulxtkqe.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqlbllst.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gwhngpfws.sHtML

TS:   同 JS
来源：http://read.share.fanxiaobao.xyz/Article/details/ghpksrjwg.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyufqhjsg.sHtML

Go:   花括号块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gsgncanrk.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsdgbxh.sHtML

C#:   块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gbvfvwocu.sHtML

[C11] 模块导入与导出
来源：http://wap.fanxiaobao.xyz/Article/details/gwtniubcs.sHtML

Py:   from module import func
来源：http://blog.fanxiaobao.xyz/Article/details/gzjqbqkuz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fanxiaobao.xyz/Article/details/gviyhkycy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gubycuznc.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fanxiaobao.xyz/Article/details/ggekdcygg.sHtML

Java: import java.util.List;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmjxikxxs.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxkbddxo.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gwzvnvprf.sHtML

C#:   using System.Text;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlofvula.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fanxiaobao.xyz/Article/details/gwosfuqqy.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fanxiaobao.xyz/Article/details/gxryfvduj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gaeygthxu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gapidclki.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gbktmesdg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/gkzatyfgd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fanxiaobao.xyz/Article/details/gowigqzwg.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/geupfpktg.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gejyuwufq.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/giyttgxol.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjrcpax.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggmcfgxvl.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuujpgca.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugvpyglv.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfgvwaax.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzbcjdxn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fanxiaobao.xyz/Article/details/gxsriolje.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/gpljgynls.sHtML

[C14] 泛型函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmckmkyr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fanxiaobao.xyz/Article/details/gfkygqzgh.sHtML

PHP:  // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gepmdjkch.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqersez.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fanxiaobao.xyz/Article/details/gozonnzyt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.fanxiaobao.xyz/Article/details/gkkpoinyt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fanxiaobao.xyz/Article/details/gqjxjaqig.sHtML

Ruby: # 无泛型
来源：http://blog.fanxiaobao.xyz/Article/details/gbmqycsfw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fanxiaobao.xyz/Article/details/gqtloaufv.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysvqacaw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/grilqsstj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcidnvgfj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjggwvhez.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gilgarxpq.sHtML

Java: // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gdtaixlvt.sHtML

Go:   // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbfpenna.sHtML

Ruby: a, b = pair
来源：http://baike.fanxiaobao.xyz/Article/details/gmxvobvet.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/girmyzvcv.sHtML

[C16] 函数 / 方法重载
来源：http://3g.fanxiaobao.xyz/Article/details/gwwprbkjf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmsvzflz.sHtML

PHP:  // 无重载
来源：http://wap.fanxiaobao.xyz/Article/details/gebycxuyg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/glpdbvity.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpderhfnq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/ggfopycir.sHtML

Go:   // 无重载：用不同函数名
来源：http://wap.fanxiaobao.xyz/Article/details/gzpdwxwym.sHtML

Ruby: # 无重载：靠动态参数
来源：http://wap.fanxiaobao.xyz/Article/details/giheorbzt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gihkanbeg.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfqvfbvog.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gjpdorlzj.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbkfstlho.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhjbczqy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlxeljgg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fanxiaobao.xyz/Article/details/gjzqjexrm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlpfvwbc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gziqskdab.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhelqsig.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmapgvlvo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gwffitjjt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.fanxiaobao.xyz/Article/details/gnblnegbm.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzabonam.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxnfcxkj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdjoshcz.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstisgqci.sHtML

TS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpvcruow.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/ghsjjqqhr.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fanxiaobao.xyz/Article/details/gszkykuwh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuilffjd.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gejomdcge.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fanxiaobao.xyz/Article/details/gsyfdxeun.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/grxrjzkku.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnmpumtx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.fanxiaobao.xyz/Article/details/glytrpzje.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gtrvhhxph.sHtML

Java: list.add(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/goulvpezf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtzjlkqa.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrttzlco.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glmznxafv.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqymrxrf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gxgunmcgt.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghwefwdmn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzecjnx.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/gzxdrczos.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gazbxokzm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gioeybuzb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gxniepdii.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gvwvmdhkw.sHtML

[D05] 访问与修改元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqmnglmw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gknjrfwml.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gdrbqlbux.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fanxiaobao.xyz/Article/details/gnmzvcwxn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlewivkx.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/grvcszdks.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxbfdvgr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fanxiaobao.xyz/Article/details/gybelijyz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdadtisnp.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gynlhmbyl.sHtML

Py:   len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/grkrdimop.sHtML

PHP:  count($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gedmwvwce.sHtML

JS:   arr.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdnoclnt.sHtML

TS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gzqzjgqeo.sHtML

Java: list.size();
来源：http://3g.fanxiaobao.xyz/Article/details/gvmdixahj.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/glglihcxq.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwqmvvtt.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gvkkofwcw.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmrunzhs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnehctkyf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gmykckyxf.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gxpvgqadm.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsxtwbdp.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gycqzxbds.sHtML

Go:   arr[1:4]
来源：http://blog.fanxiaobao.xyz/Article/details/gmmfvergr.sHtML

Ruby: arr[1, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gzcuhbasi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gxydmggoh.sHtML

[D08] 合并两个数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzffzljig.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngbkpvsk.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/guusgfjvh.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbavoyuhn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnrxfmxq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqaxkmrt.sHtML

Go:   append(a, b...)
来源：http://3g.fanxiaobao.xyz/Article/details/geyfzwpdk.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gixxdkffs.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfbpqiyf.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gogvirjyf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/gadufovqj.sHtML

PHP:  sort($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbezoqibx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/ghuambxmr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fanxiaobao.xyz/Article/details/gueqfnsqf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwavtkjeh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiccqvdd.sHtML

Ruby: arr.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gscmetyyy.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/ggcgeaall.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fanxiaobao.xyz/Article/details/gyzoqaqyk.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqhsyizi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpqsmdcx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucxmhooo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gaaxwgfxj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdprgqiev.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwpourej.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gqwwypfmg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fanxiaobao.xyz/Article/details/gjyxpprfi.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gqjlvstpn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprusctnf.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gkfwfviyr.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gthxdncxh.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsfttvyz.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtphaamlz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvozglfca.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcidbfbqn.sHtML

C#:   list.Reverse();
来源：http://m.share.fanxiaobao.xyz/Article/details/gogtlvwmb.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqhmwjmx.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsavcxhw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrosdmog.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/ghgifgjpp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiwsddot.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fanxiaobao.xyz/Article/details/guytxonym.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjdjzapd.sHtML

Ruby: arr.index(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gbkpsusdj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/geylhrpvb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fanxiaobao.xyz/Article/details/gaqizovip.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnwcjstu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glxuielwu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gajuukdrs.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfobmnpkf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxhtsuct.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbglpodts.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsrktyeo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gnefgachk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdzibfoh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/gotkanndr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gufnllaqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjetokbzf.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gsjycoqzu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gkllzxujy.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/grtuktkqq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gkacppzes.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhpqcijk.sHtML

[D15] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gpxlhsfdd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/glqbfukgd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpjynedc.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnepppvfy.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjpyeopm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.fanxiaobao.xyz/Article/details/gkijecbnw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyrsatvn.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gvijvzlyz.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gphuhcvyb.sHtML

[D16] 求和与平均值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvckvefri.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwqkrjcbj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjhpgjje.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxakrskeu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmdvshur.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqcppizv.sHtML

Go:   // 手写循环累加
来源：http://3g.fanxiaobao.xyz/Article/details/gbjjenlfp.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gnbmoxons.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfwnkbwg.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqdkaaz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gevnfhiew.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjvxrkdv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gubvaoljx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwaqbnkv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gdstaoiev.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ghewscxql.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/gzenomsuw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvdtgvwt.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/gbpgxtnqa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gogoyubbg.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/gulepxpuk.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fanxiaobao.xyz/Article/details/gnxyvggqz.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfcsselp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gypshmwgg.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsipibllj.sHtML

Ruby: nested.flatten
来源：http://www.share.fanxiaobao.xyz/Article/details/gkpdouzcm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/grypogwip.sHtML

[D19] 按字段分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gclyugbjs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwgeuuvd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfusnminl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fanxiaobao.xyz/Article/details/ggfdwqhgb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fanxiaobao.xyz/Article/details/gwkidtlhm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxfehttj.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fanxiaobao.xyz/Article/details/gewzlvlcr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyoikhyx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fanxiaobao.xyz/Article/details/goikdhlet.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gihzvvoyg.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyjiuudnw.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gvnpjfndi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdjqhkao.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsldzkkm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjioqygl.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgogvqtu.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gzzbisyws.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsnyyzfi.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grosmcefb.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/gclhofrgj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurwzfbpr.sHtML

JS:   arr.includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfhvtichf.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwvgyiqjv.sHtML

Java: list.contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gffuibctl.sHtML


<!-- 参考信息 -->