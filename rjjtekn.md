代发 wailian999

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gftyzzmei.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gwnvxdoed.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gtfcfbhic.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gbmbhgwdf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gtcozbumc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/grxxkxeyf.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.hesvh.cn/Article/details/gyxuorpzl.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.hesvh.cn/Article/details/gpcdhmtij.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://3g.zdbjq.cn/Article/details/gfghajtab.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/gmapdoelx.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gpbvkafhv.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gpsstbqlm.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gaahbtjjx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.zdbjq.cn/Article/details/gnemayury.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fehbvm.com/Article/details/gxzkvhoip.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.fehbvm.com/Article/details/gbkfibwhf.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gddpyxwav.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/gqengcwxi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/giabrwokf.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gmqqhfnhl.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gxkqtxovu.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gqibhtwmw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.zdbjq.cn/Article/details/gfrwuofcf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.hesvh.cn/Article/details/gdnhbrhli.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.zdbjq.cn/Article/details/gpyecrkil.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gesbxvomw.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gmgjvdart.sHtML

[C05] 返回多个值
来源：http://baike.fehbvm.com/Article/details/gtdweuqbw.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gkxqhwujn.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gwmfhthgx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.hesvh.cn/Article/details/gvtieqeym.sHtML

TS:   return { a, b };
来源：http://www.m.share.hesvh.cn/Article/details/gnfxouviu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.hesvh.cn/Article/details/gembuikjc.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxtaojqzt.sHtML

Ruby: return a, b
来源：http://www.m.share.fehbvm.com/Article/details/gxzfnwada.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gswmrtyio.sHtML

[C06] 匿名函数 / lambda
来源：http://mobile.hesvh.cn/Article/details/gwpffgghz.sHtML

Py:   square = lambda x: x * x
来源：http://read.share.zdbjq.cn/Article/details/grhbbqyhs.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gchsbnngi.sHtML

JS:   const square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/ghvvujccj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gaoeodslh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.hesvh.cn/Article/details/gfkrpxolx.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gztwffhuh.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gbdvrfycj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grrihimcr.sHtML

[C07] 把函数作为参数传入
来源：http://blog.hesvh.cn/Article/details/gtnaoujzt.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gottyldsd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://read.share.hesvh.cn/Article/details/gcvjnhlmf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gvjwgflxn.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gvaemlcri.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gkadggvpm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.zdbjq.cn/Article/details/gywrgclyh.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gsglgkhfp.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gwuzmvgpo.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/guceqhbjv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.fehbvm.com/Article/details/gvwsjxoxz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.m.share.hesvh.cn/Article/details/gsoybsktq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gszsommrw.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gdbljzplx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.hesvh.cn/Article/details/gfcafinoc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gefapjpii.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/guyeaoupe.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/ghntxrebz.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gctyuntxt.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gnjkkjtrh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.hesvh.cn/Article/details/gijhhjpii.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gsdsnpgue.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/glpsyovju.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/guamybdws.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gtorugimx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gcuhtrvwq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/gvnlkhyee.sHtML

[C10] 变量作用域
来源：http://baike.fehbvm.com/Article/details/gyzoavoqh.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gglaonuyh.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gqlasojut.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/ggtibcayg.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gtonzkxad.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/ghkcqisie.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gziagyvdm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gzvjtgiio.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/ggjqfvciq.sHtML

[C11] 模块导入与导出
来源：http://wap.fehbvm.com/Article/details/gsunqkwdn.sHtML

Py:   from module import func
来源：http://www.m.share.hesvh.cn/Article/details/gwzrnrnwd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gsgznbwed.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gfguivssf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.hesvh.cn/Article/details/gtbrgxsjp.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gbjqobaur.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/grglcoier.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gowfhbkrc.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gcuwmforh.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gzewrjiyp.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gvanwyjjv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/gisbsqwfu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gtsuzoixj.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gzbsbkxiz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fehbvm.com/Article/details/gajcswmvj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gvsfotohg.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/gnvexilee.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.fehbvm.com/Article/details/gwbdqpisu.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/golnzoozs.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.hesvh.cn/Article/details/gswpblqpu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gxqsvflbb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gcbjimpdu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ggfmfxhlz.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gwmzewnsf.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/grmgoiiwe.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/gqhmqfjrx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmmtaqil.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gayedqvjv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/gwspmmfci.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gugxoimxv.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gnyhyndec.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gzfdjyvag.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxgrspeqr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.hesvh.cn/Article/details/ghkruwxgg.sHtML

Ruby: # 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gnocsslvh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/ggnhqcsru.sHtML

[C15] 解构 / 展开参数
来源：http://3g.zdbjq.cn/Article/details/gqympvmao.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/gahohsegd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/garakaycj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gacugjdyn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/ghramelvr.sHtML

Java: // 无解构
来源：http://www.blog.fehbvm.com/Article/details/gsaelbifa.sHtML

Go:   // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gpkptclkg.sHtML

Ruby: a, b = pair
来源：http://mobile.hesvh.cn/Article/details/gmxyvpmtn.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gqaytljbb.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gmpiuljuu.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gpceoimqx.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/ghprwckfi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gtzkpgfhc.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gkermszuv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/giijyfiqd.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gtxeysdbp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.zdbjq.cn/Article/details/gfroetgox.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gugfaxqgv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpoioaxob.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/ggguquqhx.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/goklvmind.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gchtknutc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fehbvm.com/Article/details/gtnqhzylr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gfuzcdtrc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.fehbvm.com/Article/details/gibiwrdgt.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.hesvh.cn/Article/details/gicuiotbe.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gvsxvldpm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/gcsfvuxtn.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gunyczfod.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gwuofpvqo.sHtML

[D02] 追加元素到末尾
来源：http://3g.zdbjq.cn/Article/details/gvqhbsxxa.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.zdbjq.cn/Article/details/gkbtmifso.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.fehbvm.com/Article/details/gukpfrhiq.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/glfjggtrx.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/ggsgvmlng.sHtML

Java: list.add(4);
来源：http://www.blog.hesvh.cn/Article/details/gcgvrlgvl.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gcrnplkpt.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/ganpslhzl.sHtML

C#:   list.Add(4);
来源：http://m.share.fehbvm.com/Article/details/gbzrympzd.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gdismdczh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmakwaods.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gszwscuky.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gaonseuvd.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gzqvpejrs.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gnjdzvwhd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.zdbjq.cn/Article/details/gfzgotobe.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gofrkmjhu.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gjtqzpnpk.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gdeqiuvka.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.hesvh.cn/Article/details/gtkvndznh.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.zdbjq.cn/Article/details/gjoljmbny.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gboapjrnw.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.zdbjq.cn/Article/details/gqsusdxyg.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpraqaqlk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.zdbjq.cn/Article/details/groqsgvkv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gapqgwqej.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fehbvm.com/Article/details/gyvevlhoo.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/grvxiedes.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gmedmaisd.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gjggugpgp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gdtgjqbmc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gkmbclvdo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gzypgwxmz.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gqqqcivxx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsknuuhai.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gwzstaztq.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gxqljtete.sHtML

Py:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gqqkclgne.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gxjraypxd.sHtML

JS:   arr.length
来源：http://www.share.fehbvm.com/Article/details/gleiievpv.sHtML

TS:   arr.length
来源：http://baike.fehbvm.com/Article/details/gzjobeifh.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gdzbfnibf.sHtML

Go:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/gdrogaama.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/guyfhsiyv.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gxczehcpq.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.zdbjq.cn/Article/details/gocobnpiv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gmoprsitp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/ghykhguqj.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gxrzszhfk.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gutfpkeqv.sHtML

Java: list.subList(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gwqhizhbj.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gnsbxskqf.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gmdyzcpnw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/grmgdmpup.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/ghimpvxka.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.hesvh.cn/Article/details/gmweedwdb.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/govbtdmrg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/giaofczru.sHtML

TS:   [...a, ...b];
来源：http://read.share.fehbvm.com/Article/details/gcyqhgeik.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gbbkvfvar.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gtuujtnqi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.zdbjq.cn/Article/details/gcnndstbk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.hesvh.cn/Article/details/gefbkadut.sHtML

[D09] 排序（升序）
来源：http://baike.zdbjq.cn/Article/details/gqqfrpenh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/grzjjswbz.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/getyfdkex.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.hesvh.cn/Article/details/gkdrgzurc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gqshyxknv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gutggkjqt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfmnvwqwv.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gurahlklz.sHtML

C#:   list.Sort();
来源：http://baike.zdbjq.cn/Article/details/gpuquotmm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/ggceqsgxd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/geebkwoom.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gqkltykkw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gfxhtjzwr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gsrgupoem.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/giabepfpd.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gxrgtdmiu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gzzbwoicb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/ggqpelgov.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gotqppfft.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gntzsltdv.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfmzunehh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.zdbjq.cn/Article/details/ggscakoto.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gfgyobfbu.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gymnuynci.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gpflvnbbp.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/grqbhfzye.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/ghixzbbrc.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/gcajnlugf.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gdvltgoae.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gxgcgvfnf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/glpauxzsq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gfjrbsiwk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gizhirfxq.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gpxqnwkim.sHtML

Ruby: arr.index(x)
来源：http://read.share.zdbjq.cn/Article/details/gzoheggef.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/giyicekin.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/greoansfp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/gselqieom.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/ghjdphikl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gakcjjqpu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/ghacdlfai.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.fehbvm.com/Article/details/gtvbogvoi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gqxhfbvmd.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/ghquaylav.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gpcxlhgho.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/goqfljggc.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcrwzzjlx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gkdzsqnqo.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gorojwlyt.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gfoffqtdx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/gazuyigtb.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gkmqhnits.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gonobfswg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gdzumuzry.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gwaqscyfh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gaceqowtc.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gsmykrauy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcroxymtn.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gxgevywex.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gtrpptiip.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gafmewgxy.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/ggonzimzs.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gmnopwent.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gzkekjbkq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gxnitrrut.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.fehbvm.com/Article/details/gwibixiyc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gpwmsgwoo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gbrcltxdi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/grckqddyy.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/ggogqtspj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/ghoxtgbuk.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ggytqwfmw.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/greluesjv.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzpcwqsvc.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.zdbjq.cn/Article/details/ggpxovlru.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gwkqkbtpu.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.hesvh.cn/Article/details/gdtcyhpzl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/gdiihvgnm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gorerscce.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/guqaxjngh.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gycnyuorv.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gbfbnlzxo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gxrjzqsqa.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/glhuozibq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwswihlac.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/guxywgfyf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gpwdwqhhw.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gxewjfwtk.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gfdakwbvx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gdbsihafz.sHtML


<!-- 参考信息 -->