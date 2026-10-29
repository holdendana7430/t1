代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gzlcjrcma.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gyplcbeib.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gukkaclzi.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbrdqhns.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gawywbvnc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.hesvh.cn/Article/details/gyhjjelwh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://mobile.fehbvm.com/Article/details/gmwugssql.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gkkswheaj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gsemremjx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gnoebgudu.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.zdbjq.cn/Article/details/gpykoqlas.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gpxxavsbw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gmsujhnrn.sHtML

Ruby: f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/gotlazlmt.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gthchuybg.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/guncikpzd.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gkqnfeqzp.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gjvhkbgyu.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/guifllhph.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/ggdydopru.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.hesvh.cn/Article/details/giogrzqtg.sHtML

Go:   return a, b
来源：http://baike.zdbjq.cn/Article/details/ggcrrdhef.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gmkmbaexw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.hesvh.cn/Article/details/gvvguwjxb.sHtML

[C06] 匿名函数 / lambda
来源：http://www.blog.fehbvm.com/Article/details/gwlhabbso.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/gqbfwuvem.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gjaprjylx.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gowgvidvb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gzqozbhfv.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/glwwphxnn.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.zdbjq.cn/Article/details/gkpkotbyu.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gqdlknoec.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/geimjobjk.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gwphjvkhm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/gzvzbphnw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.zdbjq.cn/Article/details/gtxpvelmc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gmgiguome.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/glcxtfvwp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/giqhpelpf.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gwfwrtyab.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/govsleccm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gwlivzats.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gxuhtcwxr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.fehbvm.com/Article/details/gavedtioq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.hesvh.cn/Article/details/godqealpp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gepntfrqr.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gtatxwjzp.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.hesvh.cn/Article/details/gspcxkjsl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.zdbjq.cn/Article/details/gumqzlzab.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gpkyqekwf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gvczyibhd.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/ghnqrqazb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gohyheyhy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.zdbjq.cn/Article/details/ggikxzudu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gghngwppc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqghxgyrv.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.hesvh.cn/Article/details/guqgawqga.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.hesvh.cn/Article/details/gbasxshhs.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gpcrkuttq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/golywmirq.sHtML

[C10] 变量作用域
来源：http://3g.fehbvm.com/Article/details/ggwflsavg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gqaodcswr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gjywyqdet.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.hesvh.cn/Article/details/gzkrcezmf.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/gykxtkdan.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/grleoxduw.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gnnnxgkwn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gkyjwlcqb.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gqbcnzlsi.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/gwqstczbv.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gogjbzfek.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gojummkag.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/griaryink.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.zdbjq.cn/Article/details/gvjspqvoz.sHtML

Java: import java.util.List;
来源：http://blog.hesvh.cn/Article/details/givztbddc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gskegozjt.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.fehbvm.com/Article/details/gpsscveri.sHtML

C#:   using System.Text;
来源：http://wap.fehbvm.com/Article/details/giipiffhw.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gtofiedwe.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gnsdnoens.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fehbvm.com/Article/details/gnalcawxf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gkxctqtpa.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/glzkynpbo.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gbnjdfcts.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gupvtzzxp.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.zdbjq.cn/Article/details/growtiszy.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.hesvh.cn/Article/details/gujegcqcc.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gjvujarks.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.fehbvm.com/Article/details/grqbipwti.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/gveytnund.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.zdbjq.cn/Article/details/gjbfmkdst.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gjilrpahk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfulxezjg.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gggcynker.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gdsxipidh.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gnwxzmlml.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gyjrmvkkm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.fehbvm.com/Article/details/gnhbywnxi.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gtqmgdzyg.sHtML

JS:   // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gxckubtya.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/gumsdzsgv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fehbvm.com/Article/details/glizaxrkw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.zdbjq.cn/Article/details/gnfsrftnp.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gxblvwxhw.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gygmlyigc.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.zdbjq.cn/Article/details/gxmeygoov.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gljjlfprg.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gpbzvjjdj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gclwacqkf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gczixkjwk.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gbgavrood.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gpyjtmovr.sHtML

Ruby: a, b = pair
来源：http://wap.hesvh.cn/Article/details/gebwjdrvo.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gpidtepvj.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gxuuupenj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gpslcdpxn.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/guxynkryz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/ggdlemcry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.hesvh.cn/Article/details/gulrcpviw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gywjangbm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.zdbjq.cn/Article/details/gsotyhviv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gfhpjbbcc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.fehbvm.com/Article/details/galilmduo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gomeeytmg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.fehbvm.com/Article/details/gyatjcqnl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdgfpeqsd.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/gzpgxoedc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gwgmfuzca.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gishpmnio.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gfzckhyhi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/ghkhhiukq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/ggztcrhqo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gurquuovb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gtrtvuacy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gwmrfsiyu.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gjxtzcmkd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gyortwrzm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/glzsyvtzv.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gycssugkz.sHtML

TS:   arr.push(4);
来源：http://read.share.hesvh.cn/Article/details/gnkjofcfh.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/gowlxhpgg.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/gbupbpsxj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.fehbvm.com/Article/details/grcbqbhbu.sHtML

C#:   list.Add(4);
来源：http://3g.fehbvm.com/Article/details/gfnxczzno.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gozbfnbnt.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.fehbvm.com/Article/details/goncdgxrv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtyywdfaf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gusgmfmzt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gagjsoiqk.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/guulduooh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.fehbvm.com/Article/details/gzqecudqw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gjhysfium.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fehbvm.com/Article/details/gyszowcba.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gvajuwznk.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.fehbvm.com/Article/details/gihrfbunx.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ginrukgry.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/glegjynbh.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gnxriktnx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/ghfqldbab.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/guprhsnpq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.hesvh.cn/Article/details/glxeyziny.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gbxmgcefl.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/ggdcgnias.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/ghxuagnyu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gfpgsftpp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gzzczfilx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.fehbvm.com/Article/details/ggyomokyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/glvgdpmyc.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gabbtkuqx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gbzfkwqox.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gksckictr.sHtML

[D06] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gskffdqdx.sHtML

Py:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gadvmdwig.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/grunqczmp.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gubzwkyqi.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gjughvjlq.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gjxezcqfo.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gopseqszh.sHtML

Ruby: arr.length; arr.size
来源：http://3g.zdbjq.cn/Article/details/gmimfazls.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gajtxpaux.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gfbxeyvpg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.fehbvm.com/Article/details/gadetpisq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/gbziepzjc.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gufpyunuz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gxrbtdqao.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gqtcvygxi.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gjqapkiiy.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.fehbvm.com/Article/details/gsmohpgze.sHtML

C#:   list.GetRange(1, 3);
来源：http://read.share.fehbvm.com/Article/details/gqjryfeth.sHtML

[D08] 合并两个数组
来源：http://wap.hesvh.cn/Article/details/gqxxudetk.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gcfxutmth.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gabxugldq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/gthhfpbrf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gwdqddlei.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.zdbjq.cn/Article/details/gjkkykutx.sHtML

Go:   append(a, b...)
来源：http://blog.hesvh.cn/Article/details/gbiunxzdq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gpkbqaunc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fehbvm.com/Article/details/gdysoztrz.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gxejuqgpd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gesnfpniy.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gyafvluwf.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/gpzkvogow.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gcejpyhhr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.zdbjq.cn/Article/details/gheeivnnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.fehbvm.com/Article/details/gerxlwsjv.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gadopgxdz.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/grtouqxba.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/geowavibv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gdcgczmmk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.fehbvm.com/Article/details/gavtyamnq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gcvczjeky.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/giwatdnjh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gnnfwnnjb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fehbvm.com/Article/details/grtqqzkgq.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gfahykmvp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gmlxxzynk.sHtML

[D11] 反转数组
来源：http://blog.hesvh.cn/Article/details/gzdnfmeod.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gfqtosanm.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.hesvh.cn/Article/details/gvmeonwop.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gkcgqoanw.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/grcacvowu.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gffezsjvz.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gjgwwfjpv.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gtwkxbcac.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gscyqyhai.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gjzsuulhl.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gorroglec.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gwkiwssxo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gnheabwnk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gcbbbfhni.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/gcgqhvhdx.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/giepwewvj.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gjeadcgwd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gkuyyvdqk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gbzjsqwhx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/gefzgxzcg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.hesvh.cn/Article/details/gaofblkno.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/glxhqjjul.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/golwlqnsl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbivdkwrj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.hesvh.cn/Article/details/gzcpadzaa.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gznfaypeh.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gybkdhqsa.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gltjlenqs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gkzqmqolg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gebzukoxj.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gavlwcqjt.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/ggjwjubsm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gtyopqept.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gnzwpilvm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gmpovqsrb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/gsxzrcgeb.sHtML

[D15] 去重
来源：http://www.blog.hesvh.cn/Article/details/geiheojux.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gtanhypym.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gcnnkykpm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/guekiedlo.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gqtjfabop.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gotabkvzf.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.hesvh.cn/Article/details/gjpeuzlbi.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gwklzeznp.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxrfhxifz.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/grdbgpmja.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gbtssgkay.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gxchwtokc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gijigqewi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gtwbytoyk.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gzralaluw.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gjrlafmnk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gjhfrwqbc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/givrhqpqs.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/gplpxegvv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.zdbjq.cn/Article/details/goyidokjd.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.zdbjq.cn/Article/details/gotvprguf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gvnmuqbjn.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gdeoliivx.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.zdbjq.cn/Article/details/gtruvuvib.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gqneqxbnr.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gwfvuczxc.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gcvnysper.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.zdbjq.cn/Article/details/gzwynvsgb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.hesvh.cn/Article/details/gkedxsnkl.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.zdbjq.cn/Article/details/gcppkrgrc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.fehbvm.com/Article/details/gjwptehsq.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gqeyhnqxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gxwvuavmt.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gdlyexvzn.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gxlubzism.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/ghonlczws.sHtML

[D19] 按字段分组
来源：http://www.blog.fehbvm.com/Article/details/gwxvrkzir.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/geybltgcv.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/giniwkaas.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.fehbvm.com/Article/details/gsmifespb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gribthrpq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gpkzvgqhm.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gfhvxtxqn.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/gjabpleop.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/glywdgdmn.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzrmyvfcq.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/ggcuqrvqz.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gwtbvlday.sHtML


<!-- 参考信息 -->