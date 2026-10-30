代发 wailian999

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdffndjon.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gcgutdvut.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/grfcodhnv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gvsxkispa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gkokefqwd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gqzxgwmxm.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gxkpgragn.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gyyvjfsze.sHtML

Py:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gqahnodqa.sHtML

PHP:  return [$a, $b];
来源：http://www.share.fehbvm.com/Article/details/gagpprprj.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gcfbhqfug.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gyjzkmwnk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/ggwysrodr.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gcegjfygh.sHtML

Ruby: return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gvzzkvevy.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.fehbvm.com/Article/details/gqubjoyvw.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gkylmfyth.sHtML

Py:   square = lambda x: x * x
来源：http://blog.fehbvm.com/Article/details/gqzhiiatm.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gxkscckyq.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gypxenqfr.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.zdbjq.cn/Article/details/gzbdflfrf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gongckqco.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/ggpjcvlqx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gekqzjxey.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjtpsnaon.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gixndiokx.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.zdbjq.cn/Article/details/gevdnrymd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.zdbjq.cn/Article/details/guawmqihu.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/guwjfjssa.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gsfrenrtx.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.zdbjq.cn/Article/details/gxfynwrag.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gdumdnnos.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.zdbjq.cn/Article/details/gesgrjdjy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gvkyfbjfu.sHtML

[C08] 闭包
来源：http://3g.fehbvm.com/Article/details/gqaxlglca.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/gjzmynqmv.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gnahnhpcr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gpwhyfqad.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gjnhqzpvc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/grwirrhlm.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gfxygnwlb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gtrtjoimk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gssgqtvez.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gofyuujze.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/grfujictv.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gnrgccbou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gwjxihehi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gvwvwqjqw.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gzjyowimz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/gjvnjdivp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gkdnhudvh.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/grvqmxguf.sHtML

[C10] 变量作用域
来源：http://wap.hesvh.cn/Article/details/gukgkweuo.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gfcsqxeer.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gbzweajbw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gitgxuzwi.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gyolfhivw.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gydgrcyxz.sHtML

Go:   花括号块级作用域
来源：http://read.share.hesvh.cn/Article/details/gsakkjnwz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gasrzhzag.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/gyfnmqqag.sHtML

[C11] 模块导入与导出
来源：http://3g.hesvh.cn/Article/details/gcsylusau.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/galvksyft.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/gxqhzxvzw.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.fehbvm.com/Article/details/gxvfjkhus.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.fehbvm.com/Article/details/gcbobgqgh.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gqliqjptm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gfogcwobp.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fehbvm.com/Article/details/gsajkjzng.sHtML

C#:   using System.Text;
来源：http://mobile.zdbjq.cn/Article/details/gjthsvzny.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gbebexgva.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.hesvh.cn/Article/details/gtcyypgpd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gwzgmpwrz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.zdbjq.cn/Article/details/gvhjzmbxa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gdskzubds.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.zdbjq.cn/Article/details/gwqmbfdxf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gwasfnfue.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.hesvh.cn/Article/details/gagdriqgb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gsgobnixh.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/getkmbvsr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gvwjcdozi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gnktvxkxe.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gvlwuvwvg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gtezwcvrc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gkgehfcil.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gsnpauecl.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gcwdrewkb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/godhbunhp.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/geezyfzyb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fehbvm.com/Article/details/gxbbfufmy.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gsdnalcqb.sHtML

JS:   // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gejnrydnf.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gqinatcml.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.zdbjq.cn/Article/details/gdwohsfhl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/ggsxjpjxi.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gaekljdge.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gizvytbtq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gnxwydkjv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gngdfebuj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gqkhnmqvv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gutsyrttf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gjozwwouq.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gyfgcxlqy.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/gheefmlvj.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/ghljtqwsf.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/ggqzzhjci.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/gfagyuymn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gslscphmd.sHtML

PHP:  // 无重载
来源：http://wap.fehbvm.com/Article/details/gkwvaxzhf.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/ggvmqzsjo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/ghvrakbfn.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzkqelhnb.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/ghydjnwgc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/giuqdbgbb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.zdbjq.cn/Article/details/gnnmtithk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gyebfhzot.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gmplpsmhw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjhzfggju.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gfvvljeuj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gsrjexmef.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gqulqiwxr.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gaaagkrsu.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/gtgplnqxf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gckchxufd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/grnxscpan.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gjhkalifa.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gkqmsrfvt.sHtML

[D02] 追加元素到末尾
来源：http://m.share.hesvh.cn/Article/details/gfuzvwpph.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/ghahohjxh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gtrllbwjk.sHtML

JS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/giflbvtev.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gvqsntmlw.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gfcxpzzqs.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fehbvm.com/Article/details/geivabelg.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gsoejrhfd.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvyxrdruy.sHtML

[D03] 在指定位置插入元素
来源：http://baike.hesvh.cn/Article/details/gidzwtden.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.fehbvm.com/Article/details/gwxcordwl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gtxoxccnp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gzvmdxilx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gfkrnguef.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gztsnsfnj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gwhmgbeav.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/gzpckmsrf.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/gcgupkpys.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gqwfjryov.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gackjgkwk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gqtujcbex.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gkgtpguma.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gikcwjrsp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/giitxyxrq.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gjqzfbscr.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gulpypzey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.zdbjq.cn/Article/details/gxxikcgks.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gwpeigebr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gfpxdyndk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gonfvcxqs.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gnygslowe.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/gctdmqrfm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gwzuyatod.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/giptctqof.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.zdbjq.cn/Article/details/gswvcdbdb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gcqtzrxrd.sHtML

[D06] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/guwjazlxo.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gignbyaor.sHtML

PHP:  count($arr);
来源：http://mobile.fehbvm.com/Article/details/gegvrldfu.sHtML

JS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gegweamqu.sHtML

TS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gyvbqaddf.sHtML

Java: list.size();
来源：http://wap.zdbjq.cn/Article/details/gkjnonwqf.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gfzqoyhzf.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/guzvipxyj.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gjymlggha.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gtmctiltb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gnsyobofb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gvyxxdwmy.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/guswyybou.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gfcsnkawk.sHtML

Java: list.subList(1, 4);
来源：http://wap.hesvh.cn/Article/details/gzwddhjah.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gbdyrjwsk.sHtML

Ruby: arr[1, 3]
来源：http://www.share.hesvh.cn/Article/details/gvfztdxek.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gqikugqho.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gatokivcr.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fehbvm.com/Article/details/gdfllxrqi.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gcihcjjwj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gbgruvutc.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gbnfuskuo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gsfilwaaw.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gnhpvqfyd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gaqeagwlv.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gkjirlulv.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gkiqhufly.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gckgegpxg.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gryvxssqb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/geobkvfmb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.hesvh.cn/Article/details/gwpwwqsfp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gmnnekowu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gxynpceps.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gulxaitpn.sHtML

C#:   list.Sort();
来源：http://3g.fehbvm.com/Article/details/gishxwbkl.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gcqhqevja.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gbeektgqw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.fehbvm.com/Article/details/gwojehhsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gkjvyfwio.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gmhsncmig.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gtepwljln.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gylbbfmrz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.zdbjq.cn/Article/details/gaamsihdd.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gkarrnnlm.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gvnaigtdv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gystuckap.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gepiofgao.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/gpyzzscof.sHtML

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gvfvzftrf.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/ghanccspf.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/germawnof.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gftcgltgb.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/ghnvtmuzk.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/ghowebphl.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gbbqckwxu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxxyvwjfe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gxadoqnzu.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzkosgolw.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.fehbvm.com/Article/details/gxdrjwjjd.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpaeczhlb.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gexnoiybn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gkppzzfow.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/geehkfqfd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gqjivwkwa.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/gkchdxfks.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.fehbvm.com/Article/details/gfsitnpvo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gnsagqshf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gbmrbbejw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/grwpjbdfp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gpdkqusti.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghzloixtt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gytdqqxwx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.zdbjq.cn/Article/details/gqasmxsos.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gufcbtgiw.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gbpkccnyp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/glesdzwsq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gbifayaog.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/goifmmbom.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/ghvicxbfx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gxahicrvx.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/geggdlpkd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.hesvh.cn/Article/details/gcojbxgwk.sHtML

PHP:  array_unique($arr);
来源：http://3g.fehbvm.com/Article/details/gxbnhfihq.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gedvojvgn.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gqncgbcvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gdwoeksei.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gvfoelisf.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gzrxsaleb.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gevornzpl.sHtML

[D16] 求和与平均值
来源：http://blog.hesvh.cn/Article/details/grpbkouul.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gkjgihtft.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gxlzggrel.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/guidlkwyl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gcujochqq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gdhdxnatr.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/ggglwmdsi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.hesvh.cn/Article/details/gutnykwsr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gbnculwlt.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/grvaajdmh.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/grrcflors.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gwvtojjec.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gvqssjhzp.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gjgvhehdm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gdzzyfdbb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gylnpzrqn.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.zdbjq.cn/Article/details/gmnjkxbok.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gttvnmrxw.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gskjslxnk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/ghiwvrfbk.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gknonxxub.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/gmvuaxtjx.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gcwwsodne.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.zdbjq.cn/Article/details/guaqkkggb.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/grdjkwsmp.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gzedogddm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/ggvweymvo.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gjblscbtx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gavmxgetd.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gvbfsfkst.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gmchmaovg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gkiuctdlm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gsnfzahdt.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gbdcefbad.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gejxwgnpu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gzsqotkfh.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.zdbjq.cn/Article/details/gmvfecput.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/glcucxvcr.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/guokgdspy.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/glkdelosa.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gjqkokxjm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.hesvh.cn/Article/details/gwgkwftqg.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gbjevzfei.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gapidykqj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gfqugtsqy.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gzfzkqrwb.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gtisnxrxi.sHtML


<!-- 参考信息 -->