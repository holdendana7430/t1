代发 wailian999

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqwtnnpbe.sHtML

C. 函数与作用域
来源：http://read.share.zdbjq.cn/Article/details/gqxcoxydx.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gyouqvpge.sHtML

[C01] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gtegtkypy.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gyuvvncou.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/givbczvsy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gktxmsznw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/glatfqkhn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gzixslihi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gdrrgggzp.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/gpqvbhyks.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gyzkvmqml.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/gdaqovfod.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gulzmiyls.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fehbvm.com/Article/details/gzbdvnsdd.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/ghpvdlzkb.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/glhmucqfm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/gjqcszkgi.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gdoastepm.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fehbvm.com/Article/details/giogvlfhe.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gdnkwlvkr.sHtML

[C03] 可变参数
来源：http://blog.hesvh.cn/Article/details/ghkfzkeyw.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.zdbjq.cn/Article/details/gqtlhvana.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.hesvh.cn/Article/details/getcgnnah.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gkyxwgqbh.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gfxlwxdxa.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gzvcgpjji.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gdpvydfwj.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.hesvh.cn/Article/details/gmvskitkl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.hesvh.cn/Article/details/gttkweyqr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://3g.fehbvm.com/Article/details/geiazzpno.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gwxoevadq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.fehbvm.com/Article/details/gevhkxvlx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gglasyysi.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.hesvh.cn/Article/details/gbgfuhzmg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/guqjnqpos.sHtML

Go:   // 无：用配置结构体参数
来源：http://baike.hesvh.cn/Article/details/glmsezdwk.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwnwnjkbu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/ggvxxwdrt.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gipfnwpgr.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gzncekjod.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gupneqtqt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/gifdslekz.sHtML

TS:   return { a, b };
来源：http://baike.fehbvm.com/Article/details/gszhhbbpc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.zdbjq.cn/Article/details/gekhzrzvt.sHtML

Go:   return a, b
来源：http://read.share.fehbvm.com/Article/details/gbhmvaqwn.sHtML

Ruby: return a, b
来源：http://mobile.fehbvm.com/Article/details/gqlfslfvt.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.hesvh.cn/Article/details/gmuqjoato.sHtML

[C06] 匿名函数 / lambda
来源：http://3g.zdbjq.cn/Article/details/glmlvcovy.sHtML

Py:   square = lambda x: x * x
来源：http://www.m.share.zdbjq.cn/Article/details/gmfpztxgr.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/gcfzheyun.sHtML

JS:   const square = x => x * x;
来源：http://3g.hesvh.cn/Article/details/gbdvnmane.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/ghfbxkqpr.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.fehbvm.com/Article/details/gqmnytczk.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gvwjuzsfg.sHtML

Ruby: square = ->(x) { x * x }
来源：http://read.share.zdbjq.cn/Article/details/gjuhwizek.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/gccgxzmjj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gtbmsdamc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.fehbvm.com/Article/details/gcursseri.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gjtujqfil.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gtabquysm.sHtML

TS:   arr.map(String)
来源：http://www.blog.fehbvm.com/Article/details/gkopyzyxn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.fehbvm.com/Article/details/gjkkdmlye.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.zdbjq.cn/Article/details/gbzukmecu.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.zdbjq.cn/Article/details/gvbttdpnc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gjmnvtdzf.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gussdbuqf.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.zdbjq.cn/Article/details/ghsxymqmi.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gbfttjhbb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gisdnbvul.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gkzzrhuau.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gpqwdmzdt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.zdbjq.cn/Article/details/gsuvadaln.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gineomezx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gpwubpsmp.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gfngilrzx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gidtuqaxz.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtaichcyy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.zdbjq.cn/Article/details/gnrcndsgb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/glkcktjtn.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gbpszxluf.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gebroxtbp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gvuxnoefm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.hesvh.cn/Article/details/gmqbkyhul.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/guczqfsqg.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gjanjzcvi.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gdfzpgthb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.hesvh.cn/Article/details/gmaclqfpv.sHtML

TS:   同 JS
来源：http://m.share.hesvh.cn/Article/details/gghhpzwaq.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gxoyeviec.sHtML

Go:   花括号块级作用域
来源：http://m.share.hesvh.cn/Article/details/gqfnnfswr.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.fehbvm.com/Article/details/gskgdjoed.sHtML

C#:   块级作用域
来源：http://blog.hesvh.cn/Article/details/gvvxthepq.sHtML

[C11] 模块导入与导出
来源：http://baike.hesvh.cn/Article/details/guszjwdqf.sHtML

Py:   from module import func
来源：http://mobile.fehbvm.com/Article/details/gbusjopxt.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gmtynruzn.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/gnyvkeygg.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gzsxneldm.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gfcagofue.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gyqyakccy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/ghlumumgg.sHtML

C#:   using System.Text;
来源：http://m.share.zdbjq.cn/Article/details/gcedqepul.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.hesvh.cn/Article/details/gkafrwhul.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gjmwbgbvo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gwdjicszg.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gfiatojqd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gezrczolr.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gpaxgbrbs.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gqqiyfjde.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gyoniwdtn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gtnnfawfr.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.blog.hesvh.cn/Article/details/gijvmbovz.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.hesvh.cn/Article/details/gieedrskj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gmpyhzbfw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gvzyelfre.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gfcfoxuax.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gwelteder.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gqxvrokrt.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gzqqfrpoe.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.zdbjq.cn/Article/details/grgkhgvtf.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gvvgjvslf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/ggvvdzkbr.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gdxdgoauk.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/geegstxch.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/gmcymdwdq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.hesvh.cn/Article/details/gkrzcyycb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gqpfuoxzv.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gotxofian.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.fehbvm.com/Article/details/gzwzrdzmg.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/gmunspgkf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.zdbjq.cn/Article/details/gzsyxqxhh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/ghewusxqr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.hesvh.cn/Article/details/gmxeynxxq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gefgvxugt.sHtML

Java: // 无解构
来源：http://blog.zdbjq.cn/Article/details/gmjqtqytv.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gaudlnaix.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gqvrvuubp.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/gqzqymbjw.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gfmrojasq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gxmqtbpff.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gkukjeewz.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gvknuihmm.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gdqytjzrt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gmwhbqfwg.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.hesvh.cn/Article/details/gagukpqlx.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/ghviyxpdc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gsduodwfd.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxgvmflgy.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gmtcqyblb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gzpesouhm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gziafwhlw.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fehbvm.com/Article/details/gqmmypuxn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gpicabdru.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/grgnfzfzb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gnhytwvom.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/grbunbnwf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gimryuuqq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gtmpyvjwg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gnpqilcjw.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gdmhbavrs.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/gibdckfmh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gtlfiqkqr.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gvkaghogb.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gopebjeqz.sHtML

Java: list.add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gvrnriogc.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/geanbdbnl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.zdbjq.cn/Article/details/gcbrcinzj.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gofmgsysi.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gqdrhvjrf.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.fehbvm.com/Article/details/gneztqffq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gcxsuythm.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.zdbjq.cn/Article/details/gunnsnoml.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gddpkuwob.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gynftyxkq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gwtwhssqn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/gqufrncbt.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gibtvxdzw.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gizetnvju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gqopaadvp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.fehbvm.com/Article/details/ggbqvypqs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.hesvh.cn/Article/details/ggyumjmxk.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/gvgcysoak.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gposiyiva.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gnhpnrrmg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.fehbvm.com/Article/details/gbzdevonn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.zdbjq.cn/Article/details/gybymkvxt.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gkwyiayle.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gsayqkgpb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyndkqeh.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvvlltema.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gojikmpli.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.hesvh.cn/Article/details/gfrmdqxjj.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gfvxccwij.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gmrmmdyfq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/gobllsxpa.sHtML

[D06] 数组长度
来源：http://blog.zdbjq.cn/Article/details/gmlnhvlat.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gstzbtftr.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gycwquyxe.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gfjzlgbco.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gporhornf.sHtML

Java: list.size();
来源：http://read.share.zdbjq.cn/Article/details/ganfcgubv.sHtML

Go:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gaczjhycb.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gefmaynwa.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gapnfvkvv.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gaermwyil.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.hesvh.cn/Article/details/gzyyzpftv.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.hesvh.cn/Article/details/giukspqha.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/ghmhawxrk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghtufnqxm.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gbhjjpzur.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gtlscwens.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gjmxqbtxa.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gvgragbyv.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gjvbahqvu.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gsrexcluv.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gcwalfheq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gqnqvrhwg.sHtML

TS:   [...a, ...b];
来源：http://wap.zdbjq.cn/Article/details/gkoddssgc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gofimjcdy.sHtML

Go:   append(a, b...)
来源：http://baike.hesvh.cn/Article/details/gkjiehtwz.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/glejkfayg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.hesvh.cn/Article/details/gpmwzifcu.sHtML

[D09] 排序（升序）
来源：http://3g.fehbvm.com/Article/details/ghisegjei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gbfrxikjy.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcoveslkg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/geozzblgs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/giwdnrbfq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gxtyhxggp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glhehsbxq.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/glsksnduz.sHtML

C#:   list.Sort();
来源：http://m.share.fehbvm.com/Article/details/gkjexeltf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.fehbvm.com/Article/details/gkwpsxmvw.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gkxuvkbqv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gygmuyltw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gbgugpiod.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gpoxbypab.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gjeqkomiw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gtxyyelnp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.hesvh.cn/Article/details/gqfpkejxs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gxjgndvjm.sHtML

[D11] 反转数组
来源：http://wap.fehbvm.com/Article/details/griawvirz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.hesvh.cn/Article/details/gcpmmmsqk.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gifqwwlwg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gumdrdhoo.sHtML

TS:   [...arr].reverse();
来源：http://baike.hesvh.cn/Article/details/gnxhbclry.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gsocxjgnr.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcnofoxyf.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfykmlgea.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gcdoxestp.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gcbfvpgig.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.hesvh.cn/Article/details/gefbinvut.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gtbvksawf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gywaodqoy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gudfxsgia.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gkyxlcghc.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnexhabyb.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/ginshdgmq.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gcnvvvdgd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/gnhzepuxp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gihtatqco.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gcuuqcoqp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gppjtxxde.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gjbapuobt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/gatfarrxc.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gyxxfnmdl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gfslojmsq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gqcgepetx.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gssumgfdu.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gmvwctmbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gceoxelyr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/ghfmsjkul.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gamixwsem.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gzwixewzo.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gcsjuniou.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gjblctkxb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gncpqsqlt.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gwjcpeqqj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gqlrzzsze.sHtML

PHP:  array_unique($arr);
来源：http://baike.fehbvm.com/Article/details/gssfktwtf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/glcyzmatn.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/guuxqaqis.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gsogrybzp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.fehbvm.com/Article/details/glicaliqi.sHtML

Ruby: arr.uniq
来源：http://mobile.zdbjq.cn/Article/details/gbyirvdtq.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.hesvh.cn/Article/details/gkfkpjwep.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gwjvnvfbx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gmizoioav.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gavmmgdhm.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gsrvnuedp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/ghaiendya.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gkvdeuahx.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/gcghhnlku.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gzjreayxt.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gxibvblom.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gccebroed.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/ggezkgang.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gugvexqaj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gckpcwfqw.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gssczzaql.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gehoxcsuc.sHtML


<!-- 参考信息 -->