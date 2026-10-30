代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fehbvm.com/Article/details/gbvjrmvxo.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/ghatvjewq.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.fehbvm.com/Article/details/gpawdghab.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gxvtryfns.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gzlxdlqiy.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gpqyhkzyx.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.hesvh.cn/Article/details/gcqvezmnh.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.zdbjq.cn/Article/details/gdtpurinf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gywqmhdae.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/gpdnwcnpu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gpquhefvt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gjtvzvegz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.hesvh.cn/Article/details/gtohgxzkb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/glynycwbv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.zdbjq.cn/Article/details/gjjvlqkly.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://blog.hesvh.cn/Article/details/gwqkyohac.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/ggnxvzqdg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.fehbvm.com/Article/details/gxghwfksb.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gncuazwqq.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/glllzmfwr.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/ggtelsngu.sHtML

PHP:  return [$a, $b];
来源：http://m.share.fehbvm.com/Article/details/gvnhxkzgp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gxepcwtvw.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gcuplwpda.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/guwofhclh.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gjpaieedf.sHtML

Ruby: return a, b
来源：http://baike.fehbvm.com/Article/details/gthddsjvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gkhxzrdyv.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/grbufcfsx.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.hesvh.cn/Article/details/ghyiyftiv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://mobile.fehbvm.com/Article/details/gtmwgxjze.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gkyuqopao.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.hesvh.cn/Article/details/grtkxvvgn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gcmomhhst.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/geutdifip.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gezkcehtd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/ghyffsbgk.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gkxbqmhed.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/ghnjrtjti.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gtdbhaiyo.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gjgaouuoc.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/geglzmmea.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gjdwxoaho.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/geezjbblz.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.hesvh.cn/Article/details/gbtnhrdwn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fehbvm.com/Article/details/gtdpalfav.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gkyarntez.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.fehbvm.com/Article/details/gzjpycjte.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gdmplercu.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gltevkvlg.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/grluswqgy.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.hesvh.cn/Article/details/giukqorph.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gtyqdpklw.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.hesvh.cn/Article/details/gadlmnroq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/guesrxpxh.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gcrhtrqnu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gjxbnluso.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gouvqsdlc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gnqdotngl.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gwlrxawdo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gmfkjtirc.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.zdbjq.cn/Article/details/gvysmuxaw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gvpluswis.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/gburhcesf.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gqvqmgajh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.fehbvm.com/Article/details/gtolyyoyw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.fehbvm.com/Article/details/gbhwoymee.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gpvstfmel.sHtML

TS:   同 JS
来源：http://wap.fehbvm.com/Article/details/giihalssz.sHtML

Java: 方法内为块级作用域
来源：http://baike.fehbvm.com/Article/details/gxfsymchd.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwksbbhmu.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gqkydozrh.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gnckpjhqi.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gjxenfxmn.sHtML

Py:   from module import func
来源：http://blog.hesvh.cn/Article/details/gsobhbahg.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/ghlpxqxoe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gdkoopzrw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gvxhftvph.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gmqlpkyzw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.hesvh.cn/Article/details/gikkpmaoe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.zdbjq.cn/Article/details/gaapvtjuj.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/gsysucqdt.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gpwxpmiza.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gtgfpckay.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/gwzqbvvcd.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gzxaobzrp.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gcuuyovbu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fehbvm.com/Article/details/ggictfhae.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gkssiyzjh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gwtxgfjrx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/ggehspqks.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gjahjmlmz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.fehbvm.com/Article/details/gbbsbzdjj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gkeaplclg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gbmqbgtqo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gpfrztqgu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gzjwmcnvb.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/goovydagg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gqdgtrrhe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.zdbjq.cn/Article/details/gibsydfpk.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/guzyisisx.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gxsltlqxj.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gfgqdpmcv.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gayifhyjs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gthtmjwmb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gudponwfz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gtfrihiai.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gshenswti.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/grfempeku.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gdlivhawf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fehbvm.com/Article/details/gjricdjqo.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/geqgoohxf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gbbxfcmvr.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.zdbjq.cn/Article/details/gcjgfycus.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwhlvkamd.sHtML

Go:   // 无解构
来源：http://wap.hesvh.cn/Article/details/gptncohgy.sHtML

Ruby: a, b = pair
来源：http://blog.hesvh.cn/Article/details/gkzevmyfm.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gwufjqucg.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.hesvh.cn/Article/details/gstbfefyx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.hesvh.cn/Article/details/gdbdttuho.sHtML

PHP:  // 无重载
来源：http://wap.hesvh.cn/Article/details/gpqygiqmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gejfprnbv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.zdbjq.cn/Article/details/gueapmjqf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.zdbjq.cn/Article/details/ggsnubifl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gdzrwjsdd.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/ghrqowmck.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gptceyfls.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gewxptzqn.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.zdbjq.cn/Article/details/gfuitjjoh.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpndakttc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/grnrijihl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/goykzsotx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gegpobieh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gnfbymrrp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/guylcdzae.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gvnlaudom.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.hesvh.cn/Article/details/gldevppuq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gokkfcisk.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/guknkhdjl.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gjsdlgfjh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/gibwkmqyz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/ghoemtlrc.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gwriexafy.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gqfyyfhog.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gyjovyyfc.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gkkgcqjav.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.hesvh.cn/Article/details/gvkdgpzit.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gvvxrsffv.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/gvommmldq.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gbxgnvdnm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.fehbvm.com/Article/details/gjynvllwk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gfpvhkvtj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ggrtnytue.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gnxcpoayb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gbmgqazzc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/groyitdtu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gsqjmiflt.sHtML

[D04] 删除元素
来源：http://read.share.zdbjq.cn/Article/details/gzwbxwjnc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/ghpmgeteh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gwhewepjl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.zdbjq.cn/Article/details/gtrlocrcn.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/goiknpfkc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghgbdkbvp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gdcsxofwn.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gabvvsiar.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gyrjakpav.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gpfybejnx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/glqyqjnyf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/galargais.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gukbwfqwf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.hesvh.cn/Article/details/guniakhxw.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/ghhlstute.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gorhalmsr.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnmvbwnws.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gupiasajc.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gfhdufypj.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsbadbztw.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gvpmqxepf.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gxvvljpdl.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gjrjqulbl.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/gggpiamim.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gvsdkwbzz.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gsgozhnga.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gfznprutq.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/ghgmjdekq.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/glqatlelr.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gybqgvmbz.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/ginxtjucp.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/goaxrseqh.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gmtrsmrxq.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gnugfhzan.sHtML

Ruby: arr[1, 3]
来源：http://mobile.hesvh.cn/Article/details/gjdfswjrh.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gjjyzulhs.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gmmzsvwsl.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gbabarxor.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjhfsqiey.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gzhaxvbzt.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gbqnylmjn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghlaeydwn.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gyeuvddqq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gnatmkoch.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/gsgmzfjjw.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gzltiszfp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gmucczzru.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/goqhwdazj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/ghwbeguqb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gzfjnukod.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gqhdbpfos.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gtdnmrnjy.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/ggqlkrhig.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/ghtrbjctp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/guxwfsbei.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gdncetkza.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gqilizwul.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gxjaqdqky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gucoqxgjh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gjwfogbhd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gbtgnfhyp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.fehbvm.com/Article/details/gyexkjiwd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gukcxyslo.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gzeiwwlsl.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gkemqhkhz.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gglwkznrv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gufjhnpxb.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gqoijciom.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gloibobyp.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.fehbvm.com/Article/details/gtjptusdp.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gllpfxocw.sHtML

C#:   list.Reverse();
来源：http://blog.zdbjq.cn/Article/details/glyzkegro.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gfnsacdwj.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/goedqsmcn.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gayndllxg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gfyktktsx.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnsoftehh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.zdbjq.cn/Article/details/gefhodlnx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gbinsjvma.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gyquchybu.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gvkavvugs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.zdbjq.cn/Article/details/gfrxpxgew.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gvqstlnsj.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gijiyetoy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/girnszfzq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwwuzpbcr.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gemevyile.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gwoinbadt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fehbvm.com/Article/details/gdaokouga.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.fehbvm.com/Article/details/golushqid.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gplzdzyri.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gqhfbunxz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/glynsqsre.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/ghnnfpbwz.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gscoyfxmp.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gielyldig.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gwagquwel.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gaqmdsjlf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbnhemads.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gbefubktf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gegwvnifa.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gwypoqvyp.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbgxiireb.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gbqqjrwsz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gtysdgbup.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gchohaopz.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gzegurhbg.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.fehbvm.com/Article/details/gzvawklao.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gjdgsgpbu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gducthzub.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gmhqszwrg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gglpfyhzx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gpumvtskb.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/geslqxwiw.sHtML

Go:   // 手写循环累加
来源：http://www.blog.fehbvm.com/Article/details/gfwdedlex.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gahgdgmij.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/ghixyakjq.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gwcrnmjxm.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gozdqbugf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/ghmbelyzr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.hesvh.cn/Article/details/gnsyywksn.sHtML

TS:   Math.max(...arr);
来源：http://mobile.zdbjq.cn/Article/details/gpypixzgn.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gxvgqbtku.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjbjezmuf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/grqquiaad.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/goggkoyqe.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gfwnxqyga.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gwtrfihek.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.zdbjq.cn/Article/details/gpnvmwqkd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gkpmmfefh.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gylyhkyxw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gttjgwsbx.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gbbjttcbm.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gvwouklmd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzdubsyym.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/geuazwmxs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gjyhjequk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gucmewoxt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.zdbjq.cn/Article/details/gjwvyxuaa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gpheoalwm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gyeqmuptn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gwptzurmp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gmmikuaed.sHtML


<!-- 参考信息 -->