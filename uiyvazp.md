代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://baike.zdbjq.cn/Article/details/gcwfbzwif.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/ghjvkcxpu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.hesvh.cn/Article/details/guzzqtvfb.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gsqbxbxdp.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/guraoangy.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/ghxwnaoaj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gdggdriyh.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gnohuljax.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/gefvolran.sHtML

Go:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gpsbgwgtz.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/ghyaidtuq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.zdbjq.cn/Article/details/gkzcygppi.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gtimaklds.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gsupesrig.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.hesvh.cn/Article/details/gjpqkgkvp.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/glawsmcpf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gronqlkhi.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.zdbjq.cn/Article/details/gdnwqmfup.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/ghgrhcrrb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gjknokcrh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gcjghktte.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gcknkrmsg.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gumwatvgg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gposourub.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/geawnedki.sHtML

TS:   arr.map(String)
来源：http://wap.fehbvm.com/Article/details/guhxopcrm.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gqrfsnzay.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gcbrijlio.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gmzoreznv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gmnhwldsy.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/glvxvuwux.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.zdbjq.cn/Article/details/ggcfrkshm.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.zdbjq.cn/Article/details/gybqnezva.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/ghabxakvr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gezzmhuhc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fehbvm.com/Article/details/gsfhrjryx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gvbbjwtiq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gzirvfepb.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/giszmkvyu.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gufdgcwus.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gpakqpssf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gxzuzrqjm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gbscdqezh.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gbpavojin.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gndxyyjdy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gkdtwqebi.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gvspuyfml.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gzpewusfp.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gnmvwyjtj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/gwghbyjvc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/gqytwjafy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gyekrdgpk.sHtML

TS:   同 JS
来源：http://wap.hesvh.cn/Article/details/gpuclodfi.sHtML

Java: 方法内为块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gpfokbtiu.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gnrngktac.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gswbdbthi.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gtrxjnzpm.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gihjqijjh.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/garmxpgyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.hesvh.cn/Article/details/gonhbocmx.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gjuorfqqr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/ginmlptdh.sHtML

Java: import java.util.List;
来源：http://m.share.fehbvm.com/Article/details/gqazgvpcm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/glwvrcqhz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gphspdccp.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/ghsupxsrg.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gtgqtzwmb.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fehbvm.com/Article/details/gwtakfdui.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.zdbjq.cn/Article/details/gkmtlvwos.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gcnbwwxyx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gbiecjqhn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gxxnvlxja.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.fehbvm.com/Article/details/gymgsinbu.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gbvixnxzt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.hesvh.cn/Article/details/gbuujydpl.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.zdbjq.cn/Article/details/gfdoxnpgl.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gmvsqirum.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfpsvvvog.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gjtfvgmks.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gcmoqdyks.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gmvywpngg.sHtML

Go:   func add(a, b int) int
来源：http://baike.hesvh.cn/Article/details/gvemleaoo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gfwrtycpq.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/goujtunnl.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/goudtnoij.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gutoqwqcm.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/geaextvjl.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gdjjlhuxq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.hesvh.cn/Article/details/gbtmuqqdv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/gcshflypv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/glovvywey.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gqovsscmk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/gywqavtlb.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gjraqhayo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gireksyfq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gnhiyoxgy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gxrmhytlm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/guzdmflwl.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gyeotjqfe.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/grjsokhcg.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gcdyjdvjy.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.zdbjq.cn/Article/details/gwywsampc.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gfblcowgv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gqbrxkkrh.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gvccemvga.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/gwsgrluyk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gthqlkmgm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gvtcchyyg.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gletpsgjf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.zdbjq.cn/Article/details/gieyihupk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/gxwixmdrl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gkgxucror.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fehbvm.com/Article/details/gfknfvqpb.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbhrnklnb.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/gfkjujvyd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gsavocpxu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gudmvwhfy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/ggbwinuhi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.hesvh.cn/Article/details/gvxdnujks.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.zdbjq.cn/Article/details/gegtxagfo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gkbjxjsel.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.hesvh.cn/Article/details/glsdouedf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.zdbjq.cn/Article/details/gcgtgxhvu.sHtML

[D02] 追加元素到末尾
来源：http://wap.fehbvm.com/Article/details/gjxnkrtze.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gwcjrezds.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gugorbjqi.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/gwumramhq.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gxaywbkcf.sHtML

Java: list.add(4);
来源：http://www.blog.fehbvm.com/Article/details/grgbucyka.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gprbsysrd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/ggtfemerj.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gqiwmexrf.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gzslwfnzl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gdiizzivh.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/grpjfhwux.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/giwcbmegw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/ghhvgytkp.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/gaubnivkc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fehbvm.com/Article/details/gqjkemhwp.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.zdbjq.cn/Article/details/gwcvbxhqt.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gxgrohhip.sHtML

[D04] 删除元素
来源：http://mobile.zdbjq.cn/Article/details/gawuicgyg.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdwdvbqfw.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gzaehfkoz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gjjisqafu.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.zdbjq.cn/Article/details/gaejmgpvb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gipeadxqq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gwutfidpe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gdzghnxao.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gdelbhbxz.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gotchbrfl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gmsfyzebc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gswnmxsvs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gclgvqmyh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/ghobpfukj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gwmkpfdwp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gpfyjdzzn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gvsumcbbt.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gjqxrlsvi.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gqhidhyey.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gvgqaotxm.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gzeskrpis.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gwineiwjn.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gsmxkrfjr.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/gmjevijlg.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gccyjkkif.sHtML

Ruby: arr.length; arr.size
来源：http://www.m.share.hesvh.cn/Article/details/geinelcsc.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gikkokmnc.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gdixeitku.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gqhgsntot.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.fehbvm.com/Article/details/gozhyoyig.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/geotjzznp.sHtML

TS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gdoxqrkkx.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gluvxkswa.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gzzxylvgr.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gijvnxavn.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fehbvm.com/Article/details/gqnmhzbcx.sHtML

[D08] 合并两个数组
来源：http://read.share.zdbjq.cn/Article/details/gwvppqsfr.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gjraxpdgk.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gssdqbdbp.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.hesvh.cn/Article/details/guezgeznk.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/giwcrttkz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gomouesuu.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/guedvxffz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.fehbvm.com/Article/details/grcgggiro.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gdumfskko.sHtML

[D09] 排序（升序）
来源：http://www.m.share.hesvh.cn/Article/details/gfwtkeban.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gvbscoeiu.sHtML

PHP:  sort($arr);
来源：http://blog.zdbjq.cn/Article/details/gmudqdhae.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gxtwmihye.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gswpgtliy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/ggzywgvsr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/gbfxwblbh.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gwwelvfuz.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gyuhqvhha.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ghsqqnyog.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/guutpkyzh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.zdbjq.cn/Article/details/gonfaiquo.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.fehbvm.com/Article/details/gksjfiztb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gcxaoejhj.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.hesvh.cn/Article/details/giwulxzxh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gjdmlgspi.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/ggwumeykr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.zdbjq.cn/Article/details/gfexbhvoe.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/ghkteqmjo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gmwzvreei.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fehbvm.com/Article/details/gmvevruip.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gbzueznvw.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/godqzegdj.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/grznktvkd.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/gcjmefkbg.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/ggcxvnyqm.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gjiaurzif.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gcydvsuhm.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gnzfsueoh.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.hesvh.cn/Article/details/gbclnqgoo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gqovxvkgf.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcultjae.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gnuqtndol.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/glcapader.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gaxalskfx.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gnmsleton.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gpdjyzmcz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/geazakelq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gpjapmoho.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gjycjsrgr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gyrrwkfqp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gbcspbsom.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gbsrsmdku.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.hesvh.cn/Article/details/gxsbuofhb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gdtakhjdw.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gmupiqtko.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gipjdbflu.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fehbvm.com/Article/details/gynvlqagp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmrijdzbi.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/goxacdbhr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gtdjafdpy.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gfbnytllc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gdxklkege.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gnchjtkyy.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/gqimvimjj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/gihiuxivm.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gfewifsgu.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/giojhhhvj.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/godticsvd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.hesvh.cn/Article/details/gtozadlbn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gjgaltkyg.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gytufzrfz.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gugfjzzpz.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/glnxnyltt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gqlldbtua.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gzqaojkcx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gonrvdceh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gzibblpav.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fehbvm.com/Article/details/gkjxcudjl.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/genquvvua.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gcttzndcv.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gyhtpgcgv.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gpdbgwchu.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.fehbvm.com/Article/details/ghqoryqkw.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gisqmuhiq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gjcitzkin.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/glohoyody.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gdbalmcog.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gfwetdjoi.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gwzovtiuk.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/glevgqazd.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gszycpdsh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/glciiyniz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gqqenyyjw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ghuimqqfn.sHtML

TS:   nested.flat();
来源：http://wap.zdbjq.cn/Article/details/gcxbcrnat.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gzsezzpqj.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/guyovatwh.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/guudtxqwr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.hesvh.cn/Article/details/grvycumll.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gqbvgdlmd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gusabahli.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gpkivuqlj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/galtkpznh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgywdyko.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fehbvm.com/Article/details/glmidaabe.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gwjxpmody.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/ggxcuxcue.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/ggslmufcb.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gdgzagdbm.sHtML

Py:   Counter(arr)
来源：http://blog.fehbvm.com/Article/details/gdsqjofak.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gjfutipfs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gwnyjjkeq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gxqmhestu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gpbazywem.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/ggftndbfv.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/guxtbfsjh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gwngdpdoy.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/ghxnnhpph.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gmkqkqkdm.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gzkdtdymf.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gqwwceggp.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gnfnisiud.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gayxyzeur.sHtML


<!-- 参考信息 -->