代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.zdbjq.cn/Article/details/gfepqfzrz.sHtML

[C03] 可变参数
来源：http://blog.fehbvm.com/Article/details/gllwqipkr.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/givgtpjio.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.zdbjq.cn/Article/details/gvleuajnr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gcdqqoujg.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fehbvm.com/Article/details/gbksijkjz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/goumzxrbq.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.zdbjq.cn/Article/details/gaviybswp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://m.share.zdbjq.cn/Article/details/gzvbgskwp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.fehbvm.com/Article/details/gdrzporiq.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gfdhcmeeb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gmytjtuuy.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/gfzurpwmy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gtvpbzclx.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://baike.hesvh.cn/Article/details/grzewwhjq.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gdhgewvld.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.fehbvm.com/Article/details/gtuldrdzb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gdsybzgis.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gwrzbncyb.sHtML

[C05] 返回多个值
来源：http://blog.fehbvm.com/Article/details/gviqsjgja.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gxsatklur.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/grnghuktn.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gkdndyhgy.sHtML

TS:   return { a, b };
来源：http://wap.fehbvm.com/Article/details/gsncznepk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/gtzwghyek.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gyrrlrzbw.sHtML

Ruby: return a, b
来源：http://mobile.hesvh.cn/Article/details/gluwvmjnm.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.zdbjq.cn/Article/details/gduboqsil.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gkjsuibko.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gxpvpnpvc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://3g.fehbvm.com/Article/details/gjtbkzlyd.sHtML

JS:   const square = x => x * x;
来源：http://read.share.fehbvm.com/Article/details/gvntxfkaa.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpaviqidf.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.hesvh.cn/Article/details/gddwyxnes.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.zdbjq.cn/Article/details/gxblmsfqe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gykegsllv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gwtsncebi.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gxanembsk.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/ggicrcfku.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gjgcipjrm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.fehbvm.com/Article/details/guidpaiod.sHtML

TS:   arr.map(String)
来源：http://m.share.fehbvm.com/Article/details/glbriammw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.hesvh.cn/Article/details/gictmmkdm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gxfnuicki.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.zdbjq.cn/Article/details/gnyccokax.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.fehbvm.com/Article/details/gyzcsuhon.sHtML

[C08] 闭包
来源：http://wap.zdbjq.cn/Article/details/glvcjnjnr.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gpcujwhsu.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/giaseeqin.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/grkoglcaz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gyjycbcrn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gbfsidjuz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gwnivycqu.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gudcokifw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gskmfwmuu.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/goryxmtxn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gjaletlvz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/guxcavele.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gzzqgrnhe.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gbsifetck.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gjsppbcij.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gqyzzzqoa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/gotunasfp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.zdbjq.cn/Article/details/gefjbhebm.sHtML

[C10] 变量作用域
来源：http://www.blog.hesvh.cn/Article/details/gvikzlmor.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gnwnwobib.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.hesvh.cn/Article/details/gfzzbnswj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.fehbvm.com/Article/details/gbgswtcov.sHtML

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gfwipakjf.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/guwjewyjw.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gfmconlhr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gmhybrunu.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gdpbqaotw.sHtML

[C11] 模块导入与导出
来源：http://read.share.hesvh.cn/Article/details/gtnejumvy.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gybfiqlmw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gkxsxlipd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.hesvh.cn/Article/details/gkcxvpmin.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.zdbjq.cn/Article/details/gangetxgv.sHtML

Java: import java.util.List;
来源：http://www.share.zdbjq.cn/Article/details/gyipapojx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gcbcdwxbj.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/gpmgrncqw.sHtML

C#:   using System.Text;
来源：http://www.share.zdbjq.cn/Article/details/gvgmzdonp.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gaavlxvut.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.hesvh.cn/Article/details/gcescjwcp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.zdbjq.cn/Article/details/glpyjdwbl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gfjxrylcs.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gkhtlgini.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/ghasukasn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/ggmylwchf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.zdbjq.cn/Article/details/gsajlkwda.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gikyloald.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gvaajrrmr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/ghxnfynoc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gxacdryfx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fehbvm.com/Article/details/gvarajhld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/goxndzrvx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gdohetrqq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/gggtybqjw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.zdbjq.cn/Article/details/gqwwecast.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gejamzxud.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gskuxkrdc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.zdbjq.cn/Article/details/ggjvvfiip.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/giherwqus.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/glyhetiqv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gvhtbjomq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gumnbskyr.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gqdizvpim.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gxzqhgmaj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gmlctsnwr.sHtML

[C15] 解构 / 展开参数
来源：http://baike.zdbjq.cn/Article/details/gvyxvumpr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gqwcjtnoy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gewcwxigt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/ggzggfmom.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gcborfjqy.sHtML

Java: // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/ggwqkuund.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gshxnfoce.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/grrtkglhx.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gbbwzbvhe.sHtML

[C16] 函数 / 方法重载
来源：http://3g.zdbjq.cn/Article/details/gdugawwbt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gtcqtjrzn.sHtML

PHP:  // 无重载
来源：http://www.m.share.hesvh.cn/Article/details/ggcrvujoa.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gjvruuyqb.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gihscjzhm.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/getvxcgqm.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/glbtgcspp.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/guapijpcn.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/ghmopqilg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gbtyicbfj.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gkmxjbpjz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqhwgficu.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/govxziqdb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gnykaoeub.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gbtlyuchz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.zdbjq.cn/Article/details/ggnwfydbk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gjumqdzll.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/ggztpvlkm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gjxwhpoby.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.fehbvm.com/Article/details/geeblnrzt.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gcafzxglc.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gfpmkfale.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.hesvh.cn/Article/details/gpffnwvtf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gnwavmuvp.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gibqbgbzl.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gakpdhphq.sHtML

Java: list.add(4);
来源：http://baike.zdbjq.cn/Article/details/gxpyvznjk.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gjfgmgwts.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gffwrlqlq.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gdtqglayl.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/gnzqbgcmx.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/ggzkiajja.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/glepozsmp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/gzncegndo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gfspjuptw.sHtML

Java: list.add(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gwxtivrvj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.fehbvm.com/Article/details/gakehqhqi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gowfbvdvk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gmgobiyec.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gzboradxl.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gobtkkgby.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gauoilctr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.fehbvm.com/Article/details/gqeaxaari.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.hesvh.cn/Article/details/gewclhjvn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/ggpnhhebs.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gdapvhhkq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggyfohurr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://m.share.fehbvm.com/Article/details/gruajpole.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/gcolbajhs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/grruoegxn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gkbxoxwkh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gnarnovqs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.zdbjq.cn/Article/details/gdqironqh.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.hesvh.cn/Article/details/gntzovvaa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsrqqehvv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gtiyppxcg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gvlqpdbnf.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/gghdmrcwa.sHtML

Py:   len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/ghaojzshi.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/grwulrowh.sHtML

JS:   arr.length
来源：http://www.blog.zdbjq.cn/Article/details/gbvvnrgdn.sHtML

TS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/gprpohyyp.sHtML

Java: list.size();
来源：http://www.m.share.fehbvm.com/Article/details/giorcdtpm.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gihhicmbl.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.hesvh.cn/Article/details/gbivorzmu.sHtML

C#:   list.Count;
来源：http://3g.zdbjq.cn/Article/details/gtorwabmo.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/ghuiidyea.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gjbljqazv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gjruyxzte.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/goeutcjgo.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gybwjuzky.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gamfcqcxy.sHtML

Go:   arr[1:4]
来源：http://3g.zdbjq.cn/Article/details/glccjxbmt.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gxrhiyxwd.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gwvxbnvel.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gxowpjowd.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/glhfclldz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gbzyjreit.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.hesvh.cn/Article/details/gufyckrqu.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gyfqfrzft.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.fehbvm.com/Article/details/gqntrvzpx.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gclxenphv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.hesvh.cn/Article/details/ggwfkzzda.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpfstmqtm.sHtML

[D09] 排序（升序）
来源：http://baike.fehbvm.com/Article/details/gprolohvs.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gbhvixoul.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gaswuldgy.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gwptvfpyy.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/glbghywvi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/ggvkkhkam.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gyphaukxj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gsfkthjpz.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/geilghjet.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gypsaymao.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gvbzxxkwg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/gfqmhyoqi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gtszzqhbq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gtzlpvsmd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gzrdsxqhx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/gqajqzitd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gsfizstio.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/guhnxvinr.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gdomhsyna.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gniytigmv.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/gjvusbgwv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gertjrpmx.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/goyztfxip.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/guvnoeiab.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gczjfxczp.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/guchwvbte.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/glegakhnf.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gxadglwfu.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.hesvh.cn/Article/details/gvdrkydto.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gckeiorea.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gsimbwtxt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gttnqzfej.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gegluhynn.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gjouoimpt.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gvpqocbtq.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkaohnknv.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gddbpiwqq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gfcnscixr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghsvasctm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gckkywbpu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnkuszsde.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gwhuvtuul.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gsthkdpzt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://read.share.zdbjq.cn/Article/details/gqthpqpnw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/goqxsjova.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gagqcbpbu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.zdbjq.cn/Article/details/ghirssybz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/geaixppqv.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/giqhguwuy.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/glbvjphri.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gfrufofow.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzppzkqgk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.hesvh.cn/Article/details/gpyutkyam.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/guchfoqpc.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gmvnjigsw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/ghmlhiueg.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gluywhqpn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/guuzmtbwg.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gbtjrkotv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gknykpvwl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gdjoozcmm.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gxxcrihif.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/grxwlgyjc.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/ggtqtqmlc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.hesvh.cn/Article/details/gadkgvisn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gomewflap.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/ghpgjpkeu.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxjarmjkt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gcwxlnlcv.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gorxtocdj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gmdweaume.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.fehbvm.com/Article/details/gsxndwxmh.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gmqvuiaqo.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gqhktqnas.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdxzfemtk.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/gnedocksu.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/ggprwprvr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gvgnybmvj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gejhbzdca.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.zdbjq.cn/Article/details/gnipwuijy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gkmvixlwz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gxpmfmcwm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/gfolftfwt.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gkojizvim.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/gvmnickgj.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gbtjxrber.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gyurdnqfy.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gafnnfkph.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gotlfbttm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fehbvm.com/Article/details/gfmtveuln.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gvuoqiaed.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.zdbjq.cn/Article/details/gvwxxmjoj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/grkgnlkho.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gfmfehgcc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fehbvm.com/Article/details/grtdyudoe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gcdcjbpcg.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gvqtrqoum.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gefzpootn.sHtML


<!-- 参考信息 -->