代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/garchfpgs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gevuderaj.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gvfviatdr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gnwjsynvf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.zdbjq.cn/Article/details/gbdnmfkmd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://blog.zdbjq.cn/Article/details/gsobxffmp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gkkvrempe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gzieixppj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gmnokbrho.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gexbfevzj.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.fehbvm.com/Article/details/ggrdsvzko.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gzxkolijj.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gdvffzlvw.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/grvbtnybm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gryteusji.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/ghpcutsje.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gbzlwyrns.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gfawsmbbf.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gphsyjazi.sHtML

TS:   return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gcdyxqezl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gtwpmoboy.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/ghkvagysk.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/glrlwswcj.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gyjfuqeiz.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.fehbvm.com/Article/details/gxamkosqw.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/gkdhwdfcz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.zdbjq.cn/Article/details/glktgbbwp.sHtML

JS:   const square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/grsdnmeze.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gvnrfcxxx.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.zdbjq.cn/Article/details/ggfhpeerz.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gwivttfup.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.hesvh.cn/Article/details/geutxinkb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gigrpofga.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.fehbvm.com/Article/details/gsavbcvwy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.zdbjq.cn/Article/details/gwumcqnxg.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggtwhnezk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.fehbvm.com/Article/details/gudywaslo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gviilrsoo.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gmzhavxaw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/glhybpcxy.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gzavipnpw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gxlodvpxs.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gyklcfddk.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gkamofslh.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.fehbvm.com/Article/details/ghcvchazf.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gxghpdqdf.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/ghnxxhauf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.zdbjq.cn/Article/details/gmecffhbd.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/gvcwzkkte.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gdwmwfnwh.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/galholyax.sHtML

[C09] 递归
来源：http://read.share.fehbvm.com/Article/details/gyidkrekr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.hesvh.cn/Article/details/ghplobquy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gbtglolym.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnjklylgw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gvfjghsph.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.zdbjq.cn/Article/details/gbosabnpa.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gojnttxgs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/gyjdxqezi.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.zdbjq.cn/Article/details/giuwjckmx.sHtML

[C10] 变量作用域
来源：http://mobile.zdbjq.cn/Article/details/gjgupdwxw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.fehbvm.com/Article/details/gnnrhashd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gyogvwnrl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.zdbjq.cn/Article/details/gsstcughl.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gwpbgjjnp.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gcauojfdb.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gtnvukaxy.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/gwdafbulz.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqpycpyft.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gilxndehy.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gemwiekmr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gamkagazu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/ggjigeook.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gdoehtdly.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/ggfwapevo.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.hesvh.cn/Article/details/gerojqkmc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gplcirxly.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/ghyubzksd.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.fehbvm.com/Article/details/gdqvkkqbx.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gmksjckvh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.fehbvm.com/Article/details/gwnbgqkod.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/guulvqrba.sHtML

TS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gormzfflc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gummjgtal.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/gkfiyruvj.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gvgqrkkvv.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.hesvh.cn/Article/details/grvdlgwyu.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.fehbvm.com/Article/details/gaxqzyuhe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/gejpqhdhr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gfeauixff.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/ghvvukadf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/grizsgzbp.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gpikwlwrh.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gjxqsdxfg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gciwvjqho.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://wap.hesvh.cn/Article/details/gznoftajy.sHtML

[C14] 泛型函数
来源：http://mobile.zdbjq.cn/Article/details/govzxoass.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.hesvh.cn/Article/details/guhcuqmbd.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/giszbgnas.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/giilpartw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gzzmbtdaw.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fehbvm.com/Article/details/gfamnjssz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/gsgsilruh.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmicfvpmp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.hesvh.cn/Article/details/gexagvjoh.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/guorprhwg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gvleiqmuz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.fehbvm.com/Article/details/gzrpsvrbk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gdxweifkf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggzubmnee.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gptuvhoww.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gqbaebuyp.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gcoufpdbt.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gaogkhwqo.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gvmnvjkba.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/ghukkwxou.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gylhvezcq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fehbvm.com/Article/details/glteumpwy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gvnbzvsys.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxblwhkab.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.zdbjq.cn/Article/details/gsrrssbjl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gyozakhkq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gpewskjdh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glzmdvpjk.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gwqiifvrq.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyixksdwv.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gwwaeyxqv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.hesvh.cn/Article/details/giumuewxe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gfpzadhyn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fehbvm.com/Article/details/gvhqcvqnj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gpqhuoxtq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/goglgxocv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gxiajeygo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.zdbjq.cn/Article/details/gkisdbyya.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gpuphgbmz.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gswptqtez.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.hesvh.cn/Article/details/gwxxanemp.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gumvulrst.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gyzpaykjf.sHtML

TS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpxiwyiv.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gcjvghoiu.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.hesvh.cn/Article/details/gkoydkwcd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.hesvh.cn/Article/details/gmorixqpx.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/goqiaijmz.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.zdbjq.cn/Article/details/gagxrkcfe.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.zdbjq.cn/Article/details/gznvztzil.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gzbyrobhl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gshgzfngu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gcoowtuhb.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gopsxuakv.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/ggkblrmzq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fehbvm.com/Article/details/ggmeigcqc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gyulwpsfj.sHtML

[D04] 删除元素
来源：http://m.share.hesvh.cn/Article/details/goyeiqueu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gqxgcgage.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.hesvh.cn/Article/details/ggqfcvdwz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/gbspctdri.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gmutwlkfj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gmpztczcw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.hesvh.cn/Article/details/ggqdlavwr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.zdbjq.cn/Article/details/gctequsvi.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/guydmcwey.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.fehbvm.com/Article/details/glhfxnosn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gspgcfpcf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gwvpuvloj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/guigafujt.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gjkyonuej.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gvguoezxf.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gfgmdcmcw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gtysjsxnd.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gnhhkfzds.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/gqfjhqjtn.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gcfdbpugv.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/ggjoljuqr.sHtML

JS:   arr.length
来源：http://read.share.fehbvm.com/Article/details/gpxrhwpib.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gtltebkwn.sHtML

Java: list.size();
来源：http://www.share.fehbvm.com/Article/details/gdivxzbpz.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/guxrxbxrl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gwcjrotnn.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gswdvgznn.sHtML

[D07] 切片 / 取子数组
来源：http://3g.hesvh.cn/Article/details/gphpvyedg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.zdbjq.cn/Article/details/gipahoafu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gdwdttxps.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gxqewvxli.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/glaaaapvf.sHtML

Java: list.subList(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gifprmtgd.sHtML

Go:   arr[1:4]
来源：http://m.share.hesvh.cn/Article/details/gdwvfjuyy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/ggrrfgvmz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gttijsgmj.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gtuictdqw.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gruzclwcf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gwilinocm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/goymmtyzv.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gxsnrpjqm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/grkpfqdwt.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gvigzrkjg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gevaikoxv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.fehbvm.com/Article/details/gssyonjju.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/goibqkest.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/greabftst.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gsfeihjhz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.hesvh.cn/Article/details/gxweigfvb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gkfioqgnb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gpgomfgwj.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnhuxrmgn.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gtobauzun.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gqahjluxq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/glgzxmaed.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/gxxhlxbzv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gwjgkkrot.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gijgaooil.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gyipurlvz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gstptlhfk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.hesvh.cn/Article/details/gempptcde.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/gckmwjxmn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gemvtzaqu.sHtML

[D11] 反转数组
来源：http://3g.hesvh.cn/Article/details/gvhpvoeao.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gkulaysjl.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gwkhsoull.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/geuxytjkj.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gugcvjbhp.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/grsgklkkh.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gbtlcllyh.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/gipolaypm.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gpeydvayt.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gwaeuebbk.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gwghybecq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gxzrtcbuz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/geqdtmzmz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gcjzbigxm.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/getcypfcv.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfqnglkfd.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/grblniyfe.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.fehbvm.com/Article/details/gahfdnvlq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gjduclxgw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gtklnfdew.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gjavvmzeb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gcnyldxoc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fehbvm.com/Article/details/gabzvaebf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gjgvhthxs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gykyunxwf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gvcrfungg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gzkmrqztu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/gamvfjqyo.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gsuwfmxgd.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/ghtdkamxo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gqfxkpnvc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gzdhfddem.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.zdbjq.cn/Article/details/gwaheinhf.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gfoklhftw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gevhjlknm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gojahtrna.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gfoqfewgx.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gtlnxxwal.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gjeptalty.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdkaqpkzh.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fehbvm.com/Article/details/gghytvomh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gfseybfpu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/gjnitvcob.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gsarjdict.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gfjollryv.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gyvannqki.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/gyeblitxf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gfspikxaf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/guundqtty.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gmhhrmdcq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gwniqksku.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gcgghuesj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.hesvh.cn/Article/details/gzreitbgj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/grdttxqmo.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gpsqjhexc.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gukekuvnn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fehbvm.com/Article/details/gglreuzfo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gmfgdrzsm.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gvaotjsez.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.hesvh.cn/Article/details/gqukpnqob.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gxtxubuzu.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gbmzyeoyx.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gttupgqzt.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/ghiksicfn.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/geytlnooz.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gpuuzobdu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gjuurzznr.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gprwjivsl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gashjvcin.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gucynfnfa.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gghwsyqwx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gpuqqusvq.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gyujxknck.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/ghgiszeun.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gzkbicxit.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gxskmzkkl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/guupujwfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gcfpreeqp.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gmhjntbhs.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/gfobinkdc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/grcdhbrdp.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gzoomxaig.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/gbbyrlepm.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/glmiywxcr.sHtML


<!-- 参考信息 -->