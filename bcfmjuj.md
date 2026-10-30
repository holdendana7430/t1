代发 wailian999

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gycocimhy.sHtML

PHP:  return [$a, $b];
来源：http://www.share.hesvh.cn/Article/details/gtfswgcvl.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gdgbylhzi.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gtlglaczl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/ghapietyl.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/gwgfzmusz.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gycuqngft.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gjdlkwqsg.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gcuafmzks.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.zdbjq.cn/Article/details/gubakbnom.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gzczgamsa.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gaxacjqhr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/gobixggpt.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.hesvh.cn/Article/details/ghrjvqbtr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.hesvh.cn/Article/details/gowfrvjvq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gfdqxlwiw.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gpixqmorz.sHtML

[C07] 把函数作为参数传入
来源：http://wap.zdbjq.cn/Article/details/gojhuuedf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gtekajbqs.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gzrhgjmff.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gjekpxvvr.sHtML

TS:   arr.map(String)
来源：http://wap.zdbjq.cn/Article/details/gbmwfjerz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gfaeplkoq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gfbqrmfcg.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/ggqxeargh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.hesvh.cn/Article/details/gpcmliqnd.sHtML

[C08] 闭包
来源：http://www.m.share.fehbvm.com/Article/details/ghrtohqnc.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gggyggbvd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gqtkxickg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gsuijrlli.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gztmkwypy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/ginvcnuok.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/ggcmfdbhu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gtlyruagr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gepocreov.sHtML

[C09] 递归
来源：http://wap.fehbvm.com/Article/details/gsqwkpsuo.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/grkwxxthg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gkmaowack.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/ggcakhwyn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/gebxiowyi.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfsvqdwgd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gqgezbkch.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/grzyycqdj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gyudptpwy.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/ghexlaqad.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gcyxqqcdt.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.zdbjq.cn/Article/details/gltreklrq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.zdbjq.cn/Article/details/geetjyvnt.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gdqisicoz.sHtML

Java: 方法内为块级作用域
来源：http://m.share.fehbvm.com/Article/details/gabjrlxdf.sHtML

Go:   花括号块级作用域
来源：http://baike.zdbjq.cn/Article/details/gxjdaocku.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gpjnigtkp.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gbkubdrhh.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gcsevsetj.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/gtavvtopg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gcurhyxro.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fehbvm.com/Article/details/gigwnpupq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gxgvaftmm.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/ghbkgfufj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/grqtmwiew.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gfivjbmpv.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gavsbqiah.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gkctokyhz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gbdhyttkf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fehbvm.com/Article/details/gptilbymh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/ghrhoszwf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gseyqdyvq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gobjsoxmn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gktxvoivy.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/gfniiqfhb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gihindzbt.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gryciixpi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gnpyznfse.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgexazxd.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/gihywlcdz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gcnthyoqs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqvbecjou.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gosbnqcux.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.blog.zdbjq.cn/Article/details/gdywuyjkt.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/gdtlsmkzq.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/gqbntkfez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gzamfaqxq.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gtfddjjjs.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/ggbawhauz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/ggwbqvhuc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gelclhvfr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.zdbjq.cn/Article/details/gcjahxytt.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gvsaqnxlk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.hesvh.cn/Article/details/gczfyrszh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gkjxbqjvx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.hesvh.cn/Article/details/gwymsqyju.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gfnuqpapv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gfsfivooo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.zdbjq.cn/Article/details/givvboruf.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gejmumoim.sHtML

Go:   // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gbyeygiqf.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gqcymtcqi.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gnoldppye.sHtML

[C16] 函数 / 方法重载
来源：http://baike.hesvh.cn/Article/details/gttocvgpi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gfrvkinyy.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ghltupgmr.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gppwusadt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.fehbvm.com/Article/details/gfswvthmy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gkolquaeu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gkrjlasfc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gigaskesc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gppldogyc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gftahkyeo.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gkdbndplb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gayftaxrm.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gkawccxdg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gctupzcjj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gyexjecze.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gtzpqjnvq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gftqxerrx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gqaxdaehp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/gqtwvuaht.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/giqteutsv.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fehbvm.com/Article/details/gatgnpowy.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gnndflups.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gnzzwiztb.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gmurwvsvj.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/ggdvexsww.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gtgjgziel.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gipfxtpqr.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/glczcfxyw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.hesvh.cn/Article/details/ghrietnyz.sHtML

C#:   list.Add(4);
来源：http://baike.fehbvm.com/Article/details/gwoesnrpt.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gwfwkiytz.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/gqdiomqgv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fehbvm.com/Article/details/gsrjvfpab.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gqlqjpqxu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gviyosivw.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/ghriznusu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.hesvh.cn/Article/details/gtayujtbf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gvdyrasix.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.hesvh.cn/Article/details/gvnwnovwm.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gxassjjff.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/ggfektipz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gqcsdfwth.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gadtpixkd.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gxixmdqun.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/garapkbqa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/gxnrjglee.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/glrjzkeoy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.fehbvm.com/Article/details/grfnbyhnj.sHtML

[D05] 访问与修改元素
来源：http://m.share.fehbvm.com/Article/details/gddooepxf.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gadqxppab.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/giswidvij.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gilplwstt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/gmxerozgs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gvgawgfme.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gbvbjikhd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gkuppbvtr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gkdrtxouz.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/ghlvqsnje.sHtML

Py:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/grhelkklx.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gsgrnjbod.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/girwjqvda.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gzlnteani.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gppztrotx.sHtML

Go:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gsrwsjwoc.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gkcmesycd.sHtML

C#:   list.Count;
来源：http://baike.hesvh.cn/Article/details/gnejinxer.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.zdbjq.cn/Article/details/goaijnzqs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.zdbjq.cn/Article/details/gtaolteic.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gikvhhzwz.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/grdonyecy.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/geevftiep.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gunkiatyg.sHtML

Go:   arr[1:4]
来源：http://read.share.zdbjq.cn/Article/details/gbkaeppzv.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gpfzlbvht.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gfrrlywiw.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gshdufmbi.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/gstsutsdy.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gcmovivwf.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/gxvbvymsi.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/giddxpvsg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/gescieihv.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gcqpzbxgx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/guysqjwib.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/gizwnjaxl.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gjjljhhpa.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gbpuregxf.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gxdcfeapd.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gnpmqfwap.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.zdbjq.cn/Article/details/gmynvihki.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gjgnldvvn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gsrcnlzyx.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gwhyffgwh.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gsyoqkfxy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gnmjcdyik.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/glbyvhiib.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.hesvh.cn/Article/details/goccpeveq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/ghvwfjnti.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzrfeep.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.zdbjq.cn/Article/details/gypdqhnfj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gswvvfthq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gxnquiqat.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/glamtjdyu.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gffihbvnl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gmkbrrobw.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyuwdxowb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gyatzhhfm.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/guwrgobga.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gnhlewhfm.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.hesvh.cn/Article/details/gcszxwqri.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/giyujvawm.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gzfljfpjs.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/guzcywgiz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.zdbjq.cn/Article/details/gxdfcblvg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gqcebbbur.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/guwqncvaz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gnnrjkgus.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/gmtvfwynf.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grzwmxkvt.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gvgstommj.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/ggnovtfoo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/glrevrdeh.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gzqxdgqvl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.zdbjq.cn/Article/details/gablesqah.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gtxynrmae.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggnjhagkg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.hesvh.cn/Article/details/gqdfftorr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.zdbjq.cn/Article/details/gleurbpai.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gmfrpxbhb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gpjekbmza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gqhfosoej.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmsuztusl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gpxruinlv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/giurgwkwp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gbaingfpw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gmsiudnqh.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gxxwdljig.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gaacglene.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gcxunmaxd.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gloxlncub.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fehbvm.com/Article/details/gjqfatzph.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgxciqut.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gdswcjhce.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/ghobxhzcf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gqmemnqoe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gbfohbvzl.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gxmpkyxlc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gzgfqtybv.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gxwgzwplm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvabbugee.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gzypdeqhj.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gljglrdtm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gwgiyfctn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/guqfhffsb.sHtML

Go:   // 手写循环累加
来源：http://blog.zdbjq.cn/Article/details/gdfmjelhh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gafakrdog.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.hesvh.cn/Article/details/gtzblkaun.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gzdbyfrhl.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gvrovvmei.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/gkszaroub.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ggdtscfoh.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gmxirxqdc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/ghzcxbetj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/ghpkvkjzz.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.zdbjq.cn/Article/details/gguomusrs.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gupolynsd.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gdlslcacr.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.fehbvm.com/Article/details/gxcuogyaz.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gcbydrfuo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gwuimrbyn.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gtscyhgpi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gokhrtrij.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gxtqhbnub.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gpnkgdlqd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gxfmedtsg.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gxvciaoyk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gvmafmsbz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gwgfyyxbv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/guajzkuhm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gmbnwqvct.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gscvkcjwi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gfsdtqvmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/ggzzddtfc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/ggxdshsar.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gkpgtsnvn.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gftkpegmk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gtpsbxtyk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gorextzxz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gntjcewbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gbueqhxjk.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gmwhnxupn.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gbhuqgrng.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gbyvrznlg.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gxhtlfhmz.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gvsxjrwxt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gofwzrhpp.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/guviwmldk.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gjqxngrld.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/gzixdmvhu.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gcxoyaaob.sHtML

Ruby: arr.include?(x)
来源：http://wap.zdbjq.cn/Article/details/gtgagwqvi.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/ggqzyqsvr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gqclsimsq.sHtML


<!-- 参考信息 -->