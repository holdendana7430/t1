代发 wailian999

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/glbvciqma.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/gnhaywbid.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.zdbjq.cn/Article/details/gdcetydaz.sHtML

JS:   const square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gvwjjsqxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.zdbjq.cn/Article/details/glmkszozs.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/gcrcxgeex.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ginzbiodf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gropnpmnt.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gzuiyukic.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/glbuigpnv.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/gesdydhzd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.zdbjq.cn/Article/details/gmmzwvpav.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gvboppzww.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/gogqkwzkd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gchhuoybe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.hesvh.cn/Article/details/gllzxkhja.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/gntyblmph.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gcjogdfhn.sHtML

[C08] 闭包
来源：http://m.share.fehbvm.com/Article/details/gktfvbcvh.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/grjvxnvjp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/ggykcclcr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvjfggmsz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gtfxzmixr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/glhixuoos.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gtvrozsir.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gfdrxxoll.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gnftpbpla.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gxntgxnpm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gelwpztee.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gkzmzvnhm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/grofwtkqn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/ghpvnpnby.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gdavbqikh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gbntnkuzw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/gdmsctzex.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gdfywoigw.sHtML

[C10] 变量作用域
来源：http://www.m.share.fehbvm.com/Article/details/gyfutowqq.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gqbqgwmpj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.zdbjq.cn/Article/details/gytdmwxen.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gxeuvdozs.sHtML

TS:   同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ghyjcubyt.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gwlvjhjjw.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gzushnlvo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.fehbvm.com/Article/details/gkjinynia.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gntunyquh.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gbspliehd.sHtML

Py:   from module import func
来源：http://baike.fehbvm.com/Article/details/gpibpcsns.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gpxfmeiut.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gjbawzdrk.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gllhochkj.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/gzfrnigna.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gedlbrkil.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gaubcbmkq.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gtvxcarqs.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/gbilxsthd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/grophcpim.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gnmmvhmjq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gxaqkqakj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gmwalkepa.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gsioolgjd.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/ggoqlnvvr.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gjxtsafyo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/gzkqvyfgn.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/gaxdrltxl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.zdbjq.cn/Article/details/geuzubjmf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/giaxnqxjs.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/ghgfsbjgy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwurtqbrn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/girngrijz.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gyqfkcduv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gxfcjgpmz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/ggukhthje.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gfswksxei.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gqmtecfjf.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gxyzmsmqj.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/giydwuwmq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gyqtfiawt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gkdenvyco.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gkuxrshtl.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/grmlaplyl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gofodcugk.sHtML

[C15] 解构 / 展开参数
来源：http://baike.hesvh.cn/Article/details/gooyupzom.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gipjlqfjw.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/ggpznoavh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gwfdqhlav.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fehbvm.com/Article/details/giqvvohjh.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gamnvtkdh.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/ggtpvqdwc.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gikvyodlg.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gxdfsqiwa.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gzeokxkwe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gyktrebef.sHtML

PHP:  // 无重载
来源：http://blog.hesvh.cn/Article/details/gqikwtogf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.hesvh.cn/Article/details/gmfcnadbz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gjhzogmcw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gurqmkjld.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gjpdzdsyp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gfpakppbw.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gygscrebm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfcxxixbj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gqppbdegr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcxfhrhht.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/grslcvgow.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gdmcshlfb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.hesvh.cn/Article/details/gsieumtvy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.zdbjq.cn/Article/details/gwxmzmhju.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.hesvh.cn/Article/details/gufwofart.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gmovxckyc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fehbvm.com/Article/details/gfbrwdtzm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gtkutyjdz.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/ghgvypctt.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/glvnuukni.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/glbzjtdpp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gywfmmekb.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gnekvzlhe.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/goeemsxbr.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gojspezoi.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/goylgutxa.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gczqkrvrb.sHtML

C#:   list.Add(4);
来源：http://mobile.fehbvm.com/Article/details/gyyhpujmg.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gbgnzqrfa.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fehbvm.com/Article/details/gonplgdwt.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gpxujjhdy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gimemquin.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gejsmynne.sHtML

Java: list.add(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gmpaxmhci.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/gvbqzwgkf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/guxuvcxts.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/glkcnrtep.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/ghtfkyoeq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fehbvm.com/Article/details/gfbbefdeg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.hesvh.cn/Article/details/guggnllus.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/gndyucksh.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gtmdxnxik.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gdxaccpdw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gbxwiiixv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/giveufftd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gpbasltwx.sHtML

[D05] 访问与修改元素
来源：http://baike.zdbjq.cn/Article/details/gfbiemhgb.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gpaowodir.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/giuvarkzf.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/giwhunids.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.hesvh.cn/Article/details/gplnelbwe.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/guddfwizs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gdbselklj.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/glfsrnhiq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gucyhrgqc.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/glpratkjg.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/giplontfm.sHtML

PHP:  count($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gthxtuatb.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gngcosyjy.sHtML

TS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/grdrzzszo.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gncoulufe.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gjhrfrqnj.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gvdbhjvdl.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gyfapzbij.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gdvbqpcnn.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/grhrhyljr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwijekbbt.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gywyagmmo.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gtvzwciwv.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gsetcvckw.sHtML

Go:   arr[1:4]
来源：http://blog.zdbjq.cn/Article/details/gmoipyugb.sHtML

Ruby: arr[1, 3]
来源：http://m.share.hesvh.cn/Article/details/ghejtbxtx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/genrqudby.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gyjzppjiz.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gnsbyjjce.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/gesfhveyt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fehbvm.com/Article/details/gtpwtvfyq.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gsfriwwuc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gqizwkcrm.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gkalyixij.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.hesvh.cn/Article/details/gpygkcvya.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gqdumyvue.sHtML

[D09] 排序（升序）
来源：http://baike.hesvh.cn/Article/details/gabdacebb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gauphlfmd.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gmkyjqmbe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gbvazqvlr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gyqkarhbm.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gzwbgkszj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gswpckwpz.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gzozwjyaw.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gtoaouudh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.zdbjq.cn/Article/details/gxwvzcvso.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.zdbjq.cn/Article/details/gfbktsivr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gxiamsszj.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gwnjcbdij.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gfnsgorcy.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/ggjlxhxkb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gnpqmyiqf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gyypqwdqi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/graawncpy.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/ggjqejqmn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gwocryqwx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gispgnrqn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gtpwkiqep.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gukhnmpaj.sHtML

Java: Collections.reverse(list);
来源：http://wap.hesvh.cn/Article/details/gxgvlbwfp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gjzonsvss.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gevpowixg.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gbnkwjhsw.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gvyoqdnvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gkynjaisy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gcvniupmk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gljaglfrv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/glrdbecib.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gbuhvdpmo.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/goslapbhg.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gduwxcmrh.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/grftnnqrr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gpnjeebjh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gkpzkvgjw.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gwzlnlsll.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gtmnwjvao.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gfseloaep.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gexzunaka.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gbjktbaqp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gezmlshvi.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gykqgjeit.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/geeajxccm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gjchdjebd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gtogilqre.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/guonwmwxi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gahzmtwod.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gqilkzbnb.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gzifbdcbz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwzuyglds.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gnlcpapjj.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gbgxibdvu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gjjtthdlc.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gsexcmews.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gkrptpbtl.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/grhjitimo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gbyevexvi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.hesvh.cn/Article/details/gordxnilv.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gcayxrqiu.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/gvetkcvqg.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/ghjasstxf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gdyisqity.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gzluxquqi.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gcbrblpax.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gnwhpvutz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gvoguxccf.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gensfnsvb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/gitzgedhw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gwrkvcubb.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/ggvgemezh.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gxcubnqlb.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gsawxqrvn.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gnzjmxmla.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gbdnzaxgb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gcdgnkjov.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/grzfqjwla.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/grparsnre.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gwijywurl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gjbhmwpfk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/grfiqwbvh.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/ghckyjpjd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gkgkddfle.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gdmlgoops.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gcgpjbavk.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gnnuhdzvg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gkasbwfbn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/ghfhhcfnf.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gxggspvsk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gmgytlaiq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/glgxoscjo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gbuavrnjk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/geufkckdr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/ghjkghnci.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gorhghvzi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gjjuqtjdz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gmsbbjimw.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/guxsvtabu.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gswbgysel.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsxhphtrj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gjwrbhbjw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gyqrpshlq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/ggarwrpld.sHtML

Go:   // 手写 map[T]int
来源：http://3g.zdbjq.cn/Article/details/gebxwknim.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gvosdjuli.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gqefyeyue.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gxwrkciyq.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gryuczncc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gdasuvrhy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/grzjfyrtb.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gkwgzuggq.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gaagqorpy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gzgmgwhdx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gcfzufprp.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gostpduit.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/glfreweag.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gatbawggt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gymqekgcf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/geekkcdle.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gnkwvlmsr.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gdglifmag.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gwksqlaqd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gmkfxhgax.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbrcpdxdy.sHtML


<!-- 参考信息 -->