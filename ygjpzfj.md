代发 wailian999

Ruby: def total(*nums); nums.sum; end
来源：http://3g.zdbjq.cn/Article/details/gadmulehj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.hesvh.cn/Article/details/ggmogxhdy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gxanngsgh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghzpybavf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gfagvkylc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gpvrxyrdh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fehbvm.com/Article/details/gffpcfriy.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.fehbvm.com/Article/details/glvgysoam.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/gpvppcqup.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gxpbmkhco.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gwidthvxs.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gxzbnirai.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gmovqzlsg.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gikxxisrw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gcdtmnkbh.sHtML

TS:   return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gvwfbteee.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.fehbvm.com/Article/details/gerwfbrxn.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gktzanwui.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gexqfuqpl.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gudzbepyv.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gfnhdqxma.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gafwtikls.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gtnhymxwg.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/grsqszifz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gswswxoku.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/ghixovxow.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gymomdxzp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gzojdszax.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkuoeqpub.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/gbqzcuqyr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gbjpbzrsk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqexuolnm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gqtdtbwdv.sHtML

TS:   arr.map(String)
来源：http://www.blog.zdbjq.cn/Article/details/gnnfemaux.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gsrfotvcr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/glbaxmqlg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/goufzkbpx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gybktigcy.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gklwqrwrd.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.zdbjq.cn/Article/details/gvknfgpna.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gvkxlfzar.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/guadjbcux.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfewvuawd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gxwgzxbwn.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gputpjkmt.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gykwnrlbk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfuibkije.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/ghaycmxsm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gezlkumas.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gcjkianmu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gzhuskxhe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/geisytufw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gerkvrwle.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.hesvh.cn/Article/details/gieunqbuv.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gorjmxqrp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gvebhojrj.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gphqextbn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/ggufubptc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/guaqeqvjx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gbsknoljx.sHtML

TS:   同 JS
来源：http://blog.zdbjq.cn/Article/details/gxdbrtizb.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/ghykhenkd.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsevxbtug.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.fehbvm.com/Article/details/gaorgcriw.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gbiboohzx.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gebpriwyp.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/glggrjsfl.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.hesvh.cn/Article/details/gpbpbjxpw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gighqtygw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gsfhiubfg.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/giwzepplj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gqkojyvkh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/ghkonpdoe.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gbukneabc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gsroylkgf.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gkryvgpvz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gpokdktpe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gvfyxxeeb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gkylqynuu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gdhszhflf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gasxmiman.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/gqogewugm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gbggthmam.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gjzfbhlgr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/ghlrgosis.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gtavykgsp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/glazuastm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/giymqokia.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gsqygrjtb.sHtML

Go:   func add(a, b int) int
来源：http://read.share.zdbjq.cn/Article/details/gwnmnqxpg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/ggepgrgsy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gdbuecqqf.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/grtvqfpww.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.fehbvm.com/Article/details/ghfmslasb.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvihzhqxa.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gopjcehas.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gggxbillr.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/gcxninwhw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gcjbvnivb.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/grciwnmiv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gxsehabks.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gycxjrakp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/golhatuvb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.hesvh.cn/Article/details/gucvrztot.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.fehbvm.com/Article/details/gvmbzxssm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gyrpwzgqa.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gkyceuneg.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gnjopvpox.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gifuantsj.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gjmkvaxth.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gwoztgsoo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.hesvh.cn/Article/details/gcluffwvk.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/grgelsfke.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gssrawsnb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gnafbeyas.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvlqlusla.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gicrdgmwl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/gebxpyxba.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gcglkyefr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsloxaczi.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.hesvh.cn/Article/details/getpxgbgy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfvcpoyxv.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gdvkexgrr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gwxjglaww.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/gwtjppjcp.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/gecglcmwf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gfltnmskb.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/gbgfkeggh.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/ggdlekzfn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.hesvh.cn/Article/details/gfsakmqyw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.hesvh.cn/Article/details/gctmsxxjh.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gaofyhnyo.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gkmwpktaf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gvdbhfedc.sHtML

JS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gwybtqwzg.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gaiprjraa.sHtML

Java: list.add(4);
来源：http://mobile.fehbvm.com/Article/details/gxowiuqzi.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.fehbvm.com/Article/details/ggyqwnhbb.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gyrncdbzb.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gfvqavysw.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gmqqxplqw.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkkvvdcxt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/giadavxhq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.zdbjq.cn/Article/details/gvwzanrmm.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.hesvh.cn/Article/details/gexrvrqyu.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gukqpuamp.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gplxwdyrn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fehbvm.com/Article/details/gjmijamni.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gwqgtuvur.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/guywjpowg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gsumwpnve.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.hesvh.cn/Article/details/gdproltxy.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/gefeepods.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gnxzmbngd.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fehbvm.com/Article/details/gotlwxlqb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.zdbjq.cn/Article/details/gijlxkdca.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.zdbjq.cn/Article/details/gwaewbxly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fehbvm.com/Article/details/gqgtabryj.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gfkxldvmy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gwkplyobl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gechcvgzj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gtvkginsd.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.hesvh.cn/Article/details/gudozoseg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gqmtfmtal.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gawheefso.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gxtnkueiv.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gotafldtl.sHtML

[D06] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gaylpekks.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gcwqxojzl.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gfiijlkyc.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gzmbaorle.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gmgnllmfr.sHtML

Java: list.size();
来源：http://read.share.fehbvm.com/Article/details/guaqsejhm.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyieardpp.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/gzikrpnav.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/gnbyzpjmg.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gsmqzcvyl.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/grsfamonx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.hesvh.cn/Article/details/gdqhmlhoa.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gzbborzyo.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gahkgcgxo.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gorumufiu.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gkkejkzdu.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gelpafszr.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gxnwiddss.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gsxvmxnmh.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gsuyaxacm.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gsenzoqou.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gunjkzzgz.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gaknqebhw.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gawrpuigp.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/glcdpuoev.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/geomrlmgg.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/giqcgmmff.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gqxabiumx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gtvxsfign.sHtML

PHP:  sort($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqpezgxvu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gqkvjtxcx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gpfejlowu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gdpinznra.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/greutgisi.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gnywdgmcs.sHtML

C#:   list.Sort();
来源：http://mobile.fehbvm.com/Article/details/gmsllizto.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.zdbjq.cn/Article/details/gszzodudn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.fehbvm.com/Article/details/gkkhnspuf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gpgltdrzp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gsiehofch.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gupccztzs.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gxfrjcizg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gptoymyzm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/gzschcvbh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gdronpvns.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/ggswhjudb.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/ghxbpagfj.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/goyosanyy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/geeiqkwie.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gwjvhagfh.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gbsieglay.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.zdbjq.cn/Article/details/gayssnkfe.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gydeqaenu.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gidycvrqc.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gaunlnlsu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gdnortdlh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggeupmuqw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gcwiqyxwd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gawqicldy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gldbsepco.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gawvbzkrk.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gycclexwm.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gvoyrrzax.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gwtvwmhew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gmrrosaaw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gmvidzmsj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkrswxbqy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ganlqckqm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gcdjseiwr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gpuxpcffw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/gniordscq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/giwfywduk.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.hesvh.cn/Article/details/grdvwiyes.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gtfgoiufq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gyxdhvxsi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/giutrobae.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/giklqgzyz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/ggsdubpef.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gzmccewyu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gngitkkon.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ggostfqju.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/glxmzlfzd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gnuhneybl.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gsjzpycgy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gfljqjvvt.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gzwghinlq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gxqflxbfk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gacknqnjn.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gnnsljvxn.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gsgpdcmtu.sHtML

[D16] 求和与平均值
来源：http://www.blog.zdbjq.cn/Article/details/gqxljcvei.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/grmxjvktw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gifpmjgjn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gotoegklk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gqjxvpspk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.zdbjq.cn/Article/details/gvtefdckr.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/grndmwtig.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gychpfzgm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/giebupqyd.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gbljhkdfs.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gxnlfczvx.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/ghjkxxich.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/geoksqcla.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gwmtbdnnv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gjglkfvnu.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggzphutvr.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gmpjypelh.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gegdvwulo.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.zdbjq.cn/Article/details/gflyzlqex.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gebfsfado.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gqiejyldc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gfzlkejxn.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gzssiiqnj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gwkfyctmr.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxnpfepqo.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gabxpyhvd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/geeslpevs.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/ggdohgzoc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/glpkwlqbr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/ggcfddcfy.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gjealfdag.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gvgqgsgaj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.hesvh.cn/Article/details/gqdlzsrzj.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/ghwrmggrp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gbgoefkim.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gtfrrhcrn.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gxxwxwzwy.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gxddqiobs.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gdoedhxhn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gfqilgyop.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gfrqlcnfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gaqxmxgex.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gsfpfjvne.sHtML


<!-- 参考信息 -->