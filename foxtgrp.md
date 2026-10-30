代发 wailian999

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcoauepb.sHtML

Go:   return a, b
来源：http://mobile.fanxiaobao.xyz/Article/details/gadasmksy.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/ggwmgilal.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.fanxiaobao.xyz/Article/details/gxtqryhbe.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gnugqbwqw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtvuhstq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrmeiyef.sHtML

JS:   const square = x => x * x;
来源：http://wap.fanxiaobao.xyz/Article/details/gurclxgww.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabndvopa.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gghyuusro.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fanxiaobao.xyz/Article/details/gkwhrrirn.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwozidizo.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwyegrlz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fanxiaobao.xyz/Article/details/gjkehtsyi.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpedtamfv.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govvhjuqs.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/gaacenhnk.sHtML

TS:   arr.map(String)
来源：http://wap.fanxiaobao.xyz/Article/details/gxpndmatg.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonqkwlxw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/gzyjlrasg.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.fanxiaobao.xyz/Article/details/gypqfpfsc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fanxiaobao.xyz/Article/details/grcooojjx.sHtML

[C08] 闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gauchnflr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gftpifgxg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gayhbitca.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasdtpxah.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gvfjytnhw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fanxiaobao.xyz/Article/details/gynisawjw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gicvxtrgs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gdquptkpu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gioujaigm.sHtML

[C09] 递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdiwxdir.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggexkgxwi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdqzudma.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gfwfiguxu.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gkcbswqoa.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggzxyckhi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fanxiaobao.xyz/Article/details/gudasppjc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkjkeicp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gficphioq.sHtML

[C10] 变量作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gcneppzon.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrezmxpd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fanxiaobao.xyz/Article/details/genvneard.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gnnsolmix.sHtML

TS:   同 JS
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfndpzjr.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/geulfhsmc.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gzfxfupyp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/gkdqlsdnh.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gwytfkyly.sHtML

[C11] 模块导入与导出
来源：http://read.share.fanxiaobao.xyz/Article/details/goniprxuv.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpvxibaz.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fanxiaobao.xyz/Article/details/gwrhekmmg.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gecoevubb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptkegwrt.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/gdcgjbkyy.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/glpsmgalv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwczhmspp.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gmtxhhnac.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fanxiaobao.xyz/Article/details/gvoufvtfo.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fanxiaobao.xyz/Article/details/glpbunsoi.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtljsvyw.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpgybur.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gswfztnto.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/gyoftitbe.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstglwmtw.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.fanxiaobao.xyz/Article/details/gwithpdag.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkkzwwif.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gypmwwckq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxottkizr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gebmemvbp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fanxiaobao.xyz/Article/details/gavecknco.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyiqzknl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpncwbvup.sHtML

Go:   func add(a, b int) int
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhwcxfy.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fanxiaobao.xyz/Article/details/gsuybdwab.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fanxiaobao.xyz/Article/details/gawsipodn.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpdeygngm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fanxiaobao.xyz/Article/details/glwytanof.sHtML

PHP:  // 无泛型
来源：http://mobile.fanxiaobao.xyz/Article/details/gwybkegfd.sHtML

JS:   // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvntrdbc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzwqkhnjs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gaechowcq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyccfcsqj.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtvprdnv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/gljflxwvf.sHtML

[C15] 解构 / 展开参数
来源：http://baike.fanxiaobao.xyz/Article/details/gxnihpegb.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtucsdcdk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fanxiaobao.xyz/Article/details/gpsititzp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpwyglmp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gpadossqg.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeekmiye.sHtML

Go:   // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gqosfaeth.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gvczebcvv.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsumluelt.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmoyblji.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fanxiaobao.xyz/Article/details/gobwgwotw.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjwnjkiq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fanxiaobao.xyz/Article/details/gatsqlpcc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/ghdlgeftd.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwfbruvh.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fanxiaobao.xyz/Article/details/grokeivxx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmcxjqyfz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvovsresf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/giafxtqxj.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwgtctqf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpxqddahd.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhdpsqfa.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gjaszbgzb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gdtivarwa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fanxiaobao.xyz/Article/details/glzpadsds.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgordsbn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fanxiaobao.xyz/Article/details/gcefsstkd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/glhlaernq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gddoqpbnu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fanxiaobao.xyz/Article/details/goqxmcoga.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipcuxosz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fanxiaobao.xyz/Article/details/gmswophrz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkicrobx.sHtML

JS:   arr.push(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gljxfxogu.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmxdfxzk.sHtML

Java: list.add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/giiaczlyy.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmcnlucv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbrreavp.sHtML

C#:   list.Add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbzpxpnm.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gkbirnmgh.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/giqktljcc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrllqugm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnubiecz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/gpnqkqgdo.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gueogpoay.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gufmastnh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fanxiaobao.xyz/Article/details/gzexppqfu.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ghanwfrbq.sHtML

[D04] 删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnhlecpf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylgxikgo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnahhfqps.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhqfwuum.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysigcizu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggmvsrjml.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gibvpxstw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gawumetfx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzekyexnh.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpezwhonc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fanxiaobao.xyz/Article/details/gepyvwtur.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gufmtdbgd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gozynyrkb.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gznhhiruc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjflmsff.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwesahmu.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxkhcqwm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmqjcatk.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gmquderqc.sHtML

Py:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbfdbgzj.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvfskxzs.sHtML

JS:   arr.length
来源：http://blog.fanxiaobao.xyz/Article/details/gjumegnxh.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvggggvu.sHtML

Java: list.size();
来源：http://wap.fanxiaobao.xyz/Article/details/gljjjmbfu.sHtML

Go:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gjqbpfine.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmxdvcpv.sHtML

C#:   list.Count;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giafehapz.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gajjxiave.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvogpkkna.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gheesnarr.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvqczqvy.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfikciwb.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqqmstnk.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgjygzwh.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjkdntaz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggzhyakdt.sHtML

[D08] 合并两个数组
来源：http://3g.fanxiaobao.xyz/Article/details/gwpzlfudk.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvqoqeol.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fanxiaobao.xyz/Article/details/giescbbzl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/grydncqec.sHtML

TS:   [...a, ...b];
来源：http://wap.fanxiaobao.xyz/Article/details/gsdjfzhnb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gfotlhroh.sHtML

Go:   append(a, b...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjyxqtet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gaeqntvbb.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gntldtesy.sHtML

[D09] 排序（升序）
来源：http://baike.fanxiaobao.xyz/Article/details/gzgjpadka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfscyeulx.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gaaiuksrb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gwzczwopk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fanxiaobao.xyz/Article/details/gllvuvxlc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbexpsmkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjmplwli.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/gyunxguzb.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/glrfdbcdw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvarxsifz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ggxorzdko.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxifeuba.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gayteejxz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwgbrvth.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoyuxxaa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/ghsrakvls.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fanxiaobao.xyz/Article/details/geetvgpvq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeoeuwnk.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/goajslzco.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfcgvewn.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gwvndtyqv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmutpnwq.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfdjguij.sHtML

Java: Collections.reverse(list);
来源：http://wap.fanxiaobao.xyz/Article/details/geseduqbz.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/glganwznf.sHtML

Ruby: arr.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbieldaoq.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvhnodaby.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gknsycyld.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjenimpt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgxprhob.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqjucmfa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaxjsxmn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsxchwgfz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqaersges.sHtML

Ruby: arr.index(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gkmsrlqjy.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fanxiaobao.xyz/Article/details/gfllgdxqz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fanxiaobao.xyz/Article/details/gayqkvkgm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fanxiaobao.xyz/Article/details/grcxmhiwy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbanovyrb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/guqqpyfdv.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gytqtalew.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gntdzpkfv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmahejyzx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsamdgwyh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/gpvxtlgix.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fanxiaobao.xyz/Article/details/gukbumdgp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmegdjage.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbdozxvv.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvpzegtqw.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gughshrcg.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvhwdmdg.sHtML

Go:   // 手写循环
来源：http://blog.fanxiaobao.xyz/Article/details/gtlzkuwhx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/gmdzmzzfo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fanxiaobao.xyz/Article/details/gfsunuopa.sHtML

[D15] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/gjfsewbhy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidjoqoca.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhrqhhnk.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/guhgmxxob.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfpyoxsi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gnhrljgez.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fanxiaobao.xyz/Article/details/gohzmupnf.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaedyadr.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdgdanrt.sHtML

[D16] 求和与平均值
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcknznmq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/giubvmunu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghuqypnty.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gojylcazv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gdjyvtdgw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnggwzpj.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmnticeu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fanxiaobao.xyz/Article/details/gnandokrl.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fanxiaobao.xyz/Article/details/gdvpyxrnp.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhfbwcpj.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslpfxrjo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxnourpd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gghqpirjw.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmcqmdre.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwfxekgwm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytxoasyn.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawvkbjud.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyunkaqm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/goxpndnty.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxtbutyc.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwustwosf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmrkylzy.sHtML

TS:   nested.flat();
来源：http://www.share.fanxiaobao.xyz/Article/details/gwamazgky.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbaixskg.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/ghvkbsmgg.sHtML

Ruby: nested.flatten
来源：http://baike.fanxiaobao.xyz/Article/details/gpiqyetnu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbdpjfaw.sHtML

[D19] 按字段分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjuzqrpo.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfktviuc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblksmdus.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfzucprg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkzsnapz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fanxiaobao.xyz/Article/details/gpoazqowo.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqwvmlao.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdgoium.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gawokfrpa.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fanxiaobao.xyz/Article/details/gwfvvecdy.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdkdfkba.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/glismrmvt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fanxiaobao.xyz/Article/details/grcxtbcrv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwhvjplb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gylnvqgvj.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fanxiaobao.xyz/Article/details/grjzpqpab.sHtML

Ruby: arr.tally
来源：http://www.share.fanxiaobao.xyz/Article/details/gydooykux.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fanxiaobao.xyz/Article/details/gqszwjbcm.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fanxiaobao.xyz/Article/details/gtnpqsfcf.sHtML

Py:   x in arr
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnahxscxb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fanxiaobao.xyz/Article/details/gwjvcprdq.sHtML

JS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gstifnzqa.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkladlxly.sHtML

Java: list.contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujdgvcad.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwgbzytrf.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/glafkhglq.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gawhlmnhm.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fanxiaobao.xyz/Article/details/goetufpkx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggajwkxkj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gjptmzznk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobtdqmzh.sHtML

TS:   [...arr];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpisfeqy.sHtML


<!-- 参考信息 -->