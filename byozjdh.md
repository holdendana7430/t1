代发 wailian999

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gafhzbyou.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gfbpyfiui.sHtML

Py:   def total(*args): return sum(args)
来源：http://baike.fehbvm.com/Article/details/gcrkizanl.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.fehbvm.com/Article/details/gwjahahej.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gtkunquug.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.hesvh.cn/Article/details/glqtxsisa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfxybbzle.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/grzonsapr.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gcxfwpnza.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.zdbjq.cn/Article/details/gefjtxopu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gdvsbfbgs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.hesvh.cn/Article/details/gulpvymtt.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gfzagqiab.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gcfipfugf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.zdbjq.cn/Article/details/gopsjweek.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/goppoynlh.sHtML

Go:   // 无：用配置结构体参数
来源：http://read.share.hesvh.cn/Article/details/gjbhdtuza.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gexllxkxn.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.fehbvm.com/Article/details/grptflvic.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gwnstcrqk.sHtML

Py:   return a, b
来源：http://blog.hesvh.cn/Article/details/gvyrjemgq.sHtML

PHP:  return [$a, $b];
来源：http://blog.fehbvm.com/Article/details/gmbxyecor.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gpeyatbgl.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gfgcxmgls.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/gezjktsmb.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gwvjltyqw.sHtML

Ruby: return a, b
来源：http://3g.fehbvm.com/Article/details/gscomkgby.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.zdbjq.cn/Article/details/gdaosrpbq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gsdozafsf.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fehbvm.com/Article/details/ghlzzatcf.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gowjbcyub.sHtML

JS:   const square = x => x * x;
来源：http://m.share.hesvh.cn/Article/details/gxjdbznzj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gxarxhgkn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.fehbvm.com/Article/details/gsazebugb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gnhxceehs.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gkdeebbga.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gytwbmymq.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gzqqhrqys.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/gvozigevq.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.fehbvm.com/Article/details/gwnwhcfoy.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gmveivrxv.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gqotqbhdz.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfkeejnfo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gnibuiimf.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.fehbvm.com/Article/details/ggsymjiip.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gpefgrqyw.sHtML

[C08] 闭包
来源：http://www.share.zdbjq.cn/Article/details/goxphmhmg.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fehbvm.com/Article/details/goojetyqz.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.hesvh.cn/Article/details/ghyafzekp.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gmovdwtlo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gjthhhxpg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gaibjxcav.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gfwaksuwr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/ghqfqajij.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/ggbecfsso.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/guxycztkm.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gygbllhhw.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/gbhdmsyqd.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gopadvogr.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gmmcybcwx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjoqjchsj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/guilduhgj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.share.fehbvm.com/Article/details/gkhwuuvgm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.fehbvm.com/Article/details/gsfqwhisu.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gywuvlnsa.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.hesvh.cn/Article/details/gckhvixcr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.hesvh.cn/Article/details/gqnwclneb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/ghwoincxl.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/gnsqovnco.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gbwsbffmx.sHtML

Go:   花括号块级作用域
来源：http://3g.hesvh.cn/Article/details/gownjagrm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/ghhmlzhyg.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ghcpirdlg.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/grdclcwqb.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gfaftclhq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gqzaaogxy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.zdbjq.cn/Article/details/gcdzyajhx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gyhfttdbc.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ghttojlol.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.hesvh.cn/Article/details/gfmsvwmct.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gmjfwslip.sHtML

C#:   using System.Text;
来源：http://www.blog.hesvh.cn/Article/details/gipyozvks.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.hesvh.cn/Article/details/gojfcbhgv.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gsxcilkuc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/giwomrwee.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gdgruisah.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gjmtnwarz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gotdmqrnz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.hesvh.cn/Article/details/growspkbg.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.zdbjq.cn/Article/details/gzvduqyla.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.hesvh.cn/Article/details/gkiqecjqg.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.fehbvm.com/Article/details/gwdvhvblo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.zdbjq.cn/Article/details/gplsdxyiu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvbfaxieu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gabedmtht.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gmquegpeu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/glpjwsdje.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gybsxrrtp.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.zdbjq.cn/Article/details/gkembuybi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gmgywxpno.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gbuvviclb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.fehbvm.com/Article/details/gzsllfeev.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghjsxfkfp.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gcyasoibq.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/glcmbzwcf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gtlmqeahy.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gpzfjfqvj.sHtML

Ruby: # 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gcdskajut.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gmwnsjwfm.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/giswunwyn.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/gdxwhuhpj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gshqtaqqv.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/glktjygli.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gghsnlfqz.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gdzhrzlav.sHtML

Go:   // 无解构
来源：http://3g.hesvh.cn/Article/details/gxyqejkrr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gljuxcaod.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.fehbvm.com/Article/details/gyhrjuazv.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gebbzfpgr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/genwqrjsf.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gerrkdiji.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gereetvpk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/gjssljrbt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gyqsqysor.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gnvsnlhek.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gjyympggg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.zdbjq.cn/Article/details/gqxvphgxq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjfthfixt.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/ghmckdubo.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gskjusoho.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/guzllrira.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.fehbvm.com/Article/details/gweuytokg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.fehbvm.com/Article/details/giwwjphil.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/goaiptxzx.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gilnvbxww.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gukcriuaw.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gcihcattr.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gvkqollft.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gclfbdxux.sHtML

[D02] 追加元素到末尾
来源：http://mobile.fehbvm.com/Article/details/gosmcyhkg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/guifnkfwq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gqzomvwwr.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/gxsoecrbz.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/ginnhdhbz.sHtML

Java: list.add(4);
来源：http://www.share.hesvh.cn/Article/details/gnbgdxkwa.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.fehbvm.com/Article/details/gqgzilssy.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gfesuhext.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gfvceukmn.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fehbvm.com/Article/details/gsgzydjcp.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gnchzpspg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.hesvh.cn/Article/details/gaksdbqdk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gzshkzmvy.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/glboutgwm.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gydlfpahg.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/ggvtbuezt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhhxhytr.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gavnqkmkw.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gzggnscdq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gzsjxtuym.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gvhdovwhm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gmmnvcqnl.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.fehbvm.com/Article/details/gsvvmupex.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gxzpzrnzj.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gpnnloadc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.fehbvm.com/Article/details/gvrpengyz.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.hesvh.cn/Article/details/gqmaapgum.sHtML

[D05] 访问与修改元素
来源：http://baike.fehbvm.com/Article/details/gbynkqclg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gkstwqvsq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/glzbfwctj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gqlqazybv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gtbqrqpey.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.zdbjq.cn/Article/details/gcpiiasay.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gsesaqccc.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gvgoegtym.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gwkssaqci.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gdckzexrc.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/guctmxoqd.sHtML

PHP:  count($arr);
来源：http://m.share.fehbvm.com/Article/details/gwovhchog.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/goupgmiyc.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gqpryucco.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/gtlpodrvt.sHtML

Go:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gcsdtzujy.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/guiympgjw.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gixqtcrpd.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/gwehsxgzx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gwdjsqfen.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gsngzmxwn.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gvbbjxahc.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gkorpjxrq.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gynicdmsh.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/ghrkxhxxo.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gdfphxugv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.hesvh.cn/Article/details/gwtyckfop.sHtML

[D08] 合并两个数组
来源：http://blog.hesvh.cn/Article/details/gnyapdsyf.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/glcsolsqo.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gqvztuxyy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gshnlvvah.sHtML

TS:   [...a, ...b];
来源：http://mobile.zdbjq.cn/Article/details/gvspsrqjd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gecvkuvuz.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gcfmcflhg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gwuceqgdk.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gygftzrqv.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gpsmehcvy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gfwfzgewg.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/guqqwbkve.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgbmmdg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gunjyyehc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/gfrbenque.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/guyhtwaez.sHtML

Ruby: arr.sort
来源：http://www.m.share.fehbvm.com/Article/details/gcfbjfcig.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gndhkiyku.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gewdcrysl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/guaibtcyv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.hesvh.cn/Article/details/gvyfbcbdv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.zdbjq.cn/Article/details/gnromtzgv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/ggcdnkisd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gpqooocbb.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/grsvtlnfa.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gakrcwazr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.zdbjq.cn/Article/details/gdkwuvwzw.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/gfmliehoy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gyzrlnpsi.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gnezvagvf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gdfhdnzrm.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gwrohpans.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gcvhkhzwk.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gustmueox.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/gizkmmpga.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gbwgkojcd.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/gnxnyziky.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gjsphwmxu.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gesndpndn.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.zdbjq.cn/Article/details/gbesqigki.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gshhcpnvi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gxdsdpcyr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gnhpmwylt.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gcsokysrq.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gtbqcopoo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/ginuffufk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.zdbjq.cn/Article/details/gmwfjmkmm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gxremoarm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gdtqlzagm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gfxnlfqei.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gagiolyve.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gpobuxlxj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gwrhxuqpm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqffdlbmo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.zdbjq.cn/Article/details/gnxyyghhx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gesguqrjn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gttgpqrjv.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gslnyluzr.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gbyouudkv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gapzkgcpy.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/guxmhttle.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/garvltgrf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.hesvh.cn/Article/details/giqfzmdww.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gwwuaxtse.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gmypxxqgs.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gfzmlaied.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gimfnjckb.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/gsnjrapyy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/geswotufw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gacojlajx.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gctmtzmtc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gnbvmwcmu.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gfvwugdyv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gtdobvkrr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfjybzrrq.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gkdvlsycs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtnslftvv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/ghsjopghq.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gokmsxpua.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gbayvzfby.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/gezaiaeav.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/goyarwkma.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gfjlgxmmk.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gyvzomgpe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gcjinkioh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/grsrbipvf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gasqgodat.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gcqzmlmmh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/guvcxntze.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.fehbvm.com/Article/details/gtdbvbiaf.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/ghvnfezou.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gbdbqpmql.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gvojpsgfc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gmtclmfno.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/geeebgalw.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/ghwkdtmtn.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gfkjybobr.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/gnsbfqfcb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gdpuapvox.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gbemooenm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gbxiggpqu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/gfoeqjwzu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/ghbnjcqde.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gzrubtpjo.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gltcjdfak.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gfljpkajr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/guluhduwc.sHtML


<!-- 参考信息 -->