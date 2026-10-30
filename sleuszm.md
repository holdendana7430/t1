代发 wailian999

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gqaemmiuz.sHtML

Py:   square = lambda x: x * x
来源：http://blog.hesvh.cn/Article/details/gswnzeuhj.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/grandirrg.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/ggzqwwogq.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.zdbjq.cn/Article/details/grngqkcwl.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gtcexrojl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gfizgqlkp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.zdbjq.cn/Article/details/gvufyjezp.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gedksmodi.sHtML

[C07] 把函数作为参数传入
来源：http://baike.zdbjq.cn/Article/details/gyrltywuz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gexpwcsuj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gkylgjdvi.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gsryumbne.sHtML

TS:   arr.map(String)
来源：http://baike.hesvh.cn/Article/details/gdachylix.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.hesvh.cn/Article/details/gxadaiseb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gyijwfcnk.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gbqvjjqjv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.zdbjq.cn/Article/details/gknvrqaej.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gjwgfooas.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gzjgfdhgj.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gtdbrykny.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gforblefl.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/groxowmnv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.blog.zdbjq.cn/Article/details/gilpebgiy.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gqtkokiyy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gmsuyfvcy.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/ggdpeeatw.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gbolmdtfn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/gvcbxjdvy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gdqmneqkw.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.zdbjq.cn/Article/details/grhocuryy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/goyqyijzk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gxbhbmbbk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/graqzdnvg.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gmruucrht.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.zdbjq.cn/Article/details/gezfdeqrr.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gozvyaodg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fehbvm.com/Article/details/gmjglzuwi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/geyqyflyr.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.hesvh.cn/Article/details/gdutdejmy.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gphbumwbi.sHtML

Java: 方法内为块级作用域
来源：http://wap.hesvh.cn/Article/details/gmrejaclq.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gggqhcwkr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.hesvh.cn/Article/details/gifmbpkbn.sHtML

C#:   块级作用域
来源：http://read.share.hesvh.cn/Article/details/gwgdngxpl.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/gyfitykzb.sHtML

Py:   from module import func
来源：http://m.share.hesvh.cn/Article/details/gmodgpauv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.fehbvm.com/Article/details/gmmurwfet.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ggpjldrnf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gpyvpouke.sHtML

Java: import java.util.List;
来源：http://www.share.fehbvm.com/Article/details/geapoqssa.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gudnchiko.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/galummrgw.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gewcrlbfe.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gupnvuvqd.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gmjtdykeh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gzfghaktb.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gpaxlnowt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gqqkvnukg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fehbvm.com/Article/details/gmcfqjzld.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gfcpwccpr.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gyteuyshp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gjpqpjhyy.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.zdbjq.cn/Article/details/gntdbaojs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gzuvfdvss.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gasafqnin.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gwthrmsjt.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gnstznmxr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gsllxvsfd.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gswrcmlqf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gzahcwfmm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gjdrrztie.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gnidtayth.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.zdbjq.cn/Article/details/gjthbowtl.sHtML

PHP:  // 无泛型
来源：http://read.share.hesvh.cn/Article/details/ghqhdcuyz.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gawpixogh.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/gspaevojj.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/guohowsme.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.hesvh.cn/Article/details/gbxxstztc.sHtML

Ruby: # 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/glxjjkbch.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gpnslkcft.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.zdbjq.cn/Article/details/gnkbzfzla.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/ggemztjjz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gewnoyxfn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/ggymzmtca.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gdmqfniqn.sHtML

Java: // 无解构
来源：http://wap.hesvh.cn/Article/details/gdxfygkgd.sHtML

Go:   // 无解构
来源：http://www.blog.zdbjq.cn/Article/details/gbommmuct.sHtML

Ruby: a, b = pair
来源：http://read.share.fehbvm.com/Article/details/gxvuuxknq.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gpqzeuspf.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fehbvm.com/Article/details/gknkiruag.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/grotoxkro.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/gagpwyfnc.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.hesvh.cn/Article/details/gomstirgd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gygbaldtc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/gdarugeid.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/grahpjvpe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gldrtvynv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gcucqvezj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxyybuiaf.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gnktrehjh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grefxdkeh.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gykpcqdeg.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gozollggn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gyoufiqxt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.fehbvm.com/Article/details/gzxwxxlfo.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/godvmyipu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gdonrczcp.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fehbvm.com/Article/details/gxbvqqmto.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.hesvh.cn/Article/details/gioqxglzx.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.hesvh.cn/Article/details/ghynsadla.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gzirbrxoe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/gaorzazjf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/ggoklayim.sHtML

JS:   arr.push(4);
来源：http://m.share.hesvh.cn/Article/details/ghvansfgk.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gfuflomaj.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/gnqpraefx.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gzvvleysj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gszoydnvt.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gixpcoffk.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gxwjzkila.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gxjysldgs.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gchqrkcgu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gwkejhssd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fehbvm.com/Article/details/gbscprvwf.sHtML

Java: list.add(0, 0);
来源：http://www.blog.hesvh.cn/Article/details/grgsbitds.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gmcdgjbko.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gnramwpvl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/ghewffzeb.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gdnnzilto.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/goduftrbf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/geucwouop.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/giliizifx.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gcqtdlgah.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/ggwteqptq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.hesvh.cn/Article/details/gfbtfclvu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/glcmzbugl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gygprygil.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gibbtbpdc.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxtwsigzo.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gsqqnzgmn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gfrwjactn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gqaqgzlhh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/ghnerdvgb.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/geujtrqmp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gnmaudrha.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gpfkhyber.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gmydtuuji.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gskdirpxz.sHtML

PHP:  count($arr);
来源：http://mobile.zdbjq.cn/Article/details/gnrcpiqka.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/glrajicxi.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gceyprqvb.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gsoprsnpd.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gutnycnlx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gjetotjfa.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/geqgjyrnn.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gvjgeccse.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.zdbjq.cn/Article/details/grwczgfua.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/gtwldhajd.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gfpmsntju.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/goerdzuru.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gtedavnoz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/gvdnxxpzr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gjrngzcni.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpyqoiioy.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gqoadfzpo.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.m.share.fehbvm.com/Article/details/gktdzpwds.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gjjalazge.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gudfojovv.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/guzpstehp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gdganjlsa.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gaavhhhlt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gzzyqugqy.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gvdkcvdqo.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gydiexpju.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/ghrimqzpj.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/gqknuyvrt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gowcrnrzi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/gswwfrtti.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gaqwlgnfq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gdrwrdxbz.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gokyubaib.sHtML

C#:   list.Sort();
来源：http://www.blog.hesvh.cn/Article/details/gsmayjqqf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gtmwmzmsh.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gnyyjbvka.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gjlsybjjy.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gpmnmueip.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gzuojyvux.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gqohyyeib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gnowvndij.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/grqhunjyx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/glyaytrgv.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gnorsguje.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gopoorbyr.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gweyjeulg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gbrylzbxj.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gjeinueig.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fehbvm.com/Article/details/gjftnqkcf.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/garsymhfj.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gdcpdcali.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/grhkznoik.sHtML

[D12] 查找元素下标
来源：http://blog.zdbjq.cn/Article/details/guraoydlj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/glstpiocr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.fehbvm.com/Article/details/gidayhkay.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gqoajcgiq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gkkpkizhi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gyncymgeq.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gxttevinr.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gbfbukcve.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/ghzpsvnjj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/goyopuycj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gzaonxmwe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmanchkm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/glxnfbtxh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gqkuevwic.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/guwxndlsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gxejamogc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gqatsvryl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/gfcxmltby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gnpotfyox.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gogbfcryk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gyaadagmb.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/grylffdcb.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gyrmktrbq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gmoxaocbw.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gnbdaigcu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/gkgrttiiq.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fehbvm.com/Article/details/grylwxvbb.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/giztrxkzi.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/guxtebtsu.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gakbbmvnj.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/glkzfbzic.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gkgckfmpa.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gonjqwxid.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gnhpkwaut.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/geojazdea.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjdiahttp.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/grfajyojd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxecwbhmz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gtysvwhvg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gmofapval.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gsjxqwajb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gheqwiigb.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gpiupehpx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gzdipuvkj.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gjhrntphf.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gmnppvvdf.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gadvszbhw.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/goizdrtnu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gmhhexnav.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gljxcjpoh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/ghdsknvum.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gxdydfzlu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gfomrcznp.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/ghnanimtl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gpmnweoyg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/givuhgujw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gsxnkcdsw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gjtkawcmo.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gsrsaoavl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/gyozrclnl.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/ggevqvitg.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/ggitepbmn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gldruezqs.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gpiezazgv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gjoefoxfl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gabsrgrbj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/godnkydhj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gnemqcjuk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/givklpmiu.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gvfgdnkwb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gxyzjmprn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gsmuimozx.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/grrdfbwfb.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gnegjrzpy.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/glbkuqter.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gcdksjmxi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gdjxyolof.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/ggwkjduda.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gtyuvmdhz.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gobbrldjg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gqkbhtlgs.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gmuaytkrv.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gtpayzplt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gkbmvzfkn.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyrexeupg.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkdstxdyk.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gayizofoq.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gxqxqatay.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/goydwttph.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gmfeffawn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/garsrggfe.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gmtznifax.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gsjuutgpb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gdywlwwbv.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/ghxwgfixo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gvvpunqbh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gekmxssaz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gulotndtp.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/guzhmokzh.sHtML


<!-- 参考信息 -->