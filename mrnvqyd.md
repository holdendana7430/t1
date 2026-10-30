代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gkfauwegf.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.share.fehbvm.com/Article/details/gvqqtpuby.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gjdjrphit.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gonbjvgqk.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gijsdehmg.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gfvubblqc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.zdbjq.cn/Article/details/gdcrsjgbj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/genhiqdoj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/glmjmoesn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.hesvh.cn/Article/details/gqdelxplj.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.fehbvm.com/Article/details/ginpyaatr.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/galbbclal.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/gokegtyyb.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/gpejyefhk.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.hesvh.cn/Article/details/ghfwxmpzq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.fehbvm.com/Article/details/gvllqtqln.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gtyclywuu.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.hesvh.cn/Article/details/gqmspubwb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gkocqedzu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fehbvm.com/Article/details/ggdwwnclb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gpbrgxmlw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.zdbjq.cn/Article/details/ghecifnxl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gwnvuphcs.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.fehbvm.com/Article/details/gqksshhsc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.zdbjq.cn/Article/details/gwyfymobq.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/ghctxidjy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gbgsyuwwj.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.blog.zdbjq.cn/Article/details/gecjobbbq.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/ggncjcagq.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gagtyaecd.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/grgogjyuw.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gsrmsgugy.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gzbpnxcrg.sHtML

PHP:  return [$a, $b];
来源：http://m.share.hesvh.cn/Article/details/ggnxdzpnw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gjmpdxgpq.sHtML

TS:   return { a, b };
来源：http://3g.hesvh.cn/Article/details/gqeoiyscj.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.zdbjq.cn/Article/details/gnrdyowhl.sHtML

Go:   return a, b
来源：http://www.share.fehbvm.com/Article/details/glwzcnlsp.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gfnxzfyhi.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.hesvh.cn/Article/details/gfqbguyar.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.fehbvm.com/Article/details/gunvijivd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gvqzibxjk.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.fehbvm.com/Article/details/gvvyslwgh.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/giuhpyjhm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.fehbvm.com/Article/details/gjroasevp.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://blog.hesvh.cn/Article/details/gycjpkwgu.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/gslilmlbw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gypuhjidb.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/ghpynakiy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/getcjunkz.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gaxfcsies.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gvqhkkdnc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.hesvh.cn/Article/details/gwgpyfrzu.sHtML

TS:   arr.map(String)
来源：http://read.share.hesvh.cn/Article/details/gfsitgids.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gawskmyxr.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/grkmjwoou.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/gpjcqkzmx.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gafxlmygq.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/guxevuzfn.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.fehbvm.com/Article/details/gfsyktlvq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/gmlbkeums.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gblxrjngv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gnexmgohk.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gytnzcdfq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.hesvh.cn/Article/details/gxfcygkij.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.zdbjq.cn/Article/details/gvasuyyak.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gswxhyxxe.sHtML

[C09] 递归
来源：http://www.share.hesvh.cn/Article/details/gsjpabsrn.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gqglrgapy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gzdbaviwz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/grpxeealm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gqqlkzehu.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gyqgilrer.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.hesvh.cn/Article/details/giztfewdx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gfwjtzfys.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/gbzkspjta.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gsckspzzm.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.hesvh.cn/Article/details/gfzvpqaeq.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gspovtqyv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gngrvmmae.sHtML

TS:   同 JS
来源：http://3g.zdbjq.cn/Article/details/ggottwsyj.sHtML

Java: 方法内为块级作用域
来源：http://blog.zdbjq.cn/Article/details/gbjpddgao.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gkzqacvgt.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gsqavomaw.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gefktsfib.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/ghhfjvlou.sHtML

Py:   from module import func
来源：http://www.share.hesvh.cn/Article/details/gwofwlkam.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gnjcyqomf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/gaxawbltb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gkevgfwpj.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gerompfgv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.zdbjq.cn/Article/details/gicoltihc.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gbjholrcr.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/goedxxiaf.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gymzunnxv.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gzgtodzmd.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.zdbjq.cn/Article/details/gnvxoqsmo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/grabinhro.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.hesvh.cn/Article/details/gnnamqebi.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gulbenggt.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.zdbjq.cn/Article/details/gpdsbwbbi.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/ghggbkdsa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gsnzsgcur.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fehbvm.com/Article/details/gwvwkipxn.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/golauxweq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/grykayult.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.fehbvm.com/Article/details/ggaynjivm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gjabxsbev.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gvrqcsmdr.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gpvchxgyd.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gyernckmx.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gpzzgsmtq.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gnspeqfkp.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.fehbvm.com/Article/details/gulfsbpjs.sHtML

PHP:  // 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gjprzamxk.sHtML

JS:   // 无泛型
来源：http://www.share.hesvh.cn/Article/details/gjlcovbvp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gdfirlptc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.hesvh.cn/Article/details/gytfmmxiq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gzjmhrjda.sHtML

Ruby: # 无泛型
来源：http://m.share.zdbjq.cn/Article/details/geapicoyo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.zdbjq.cn/Article/details/ggrpngrvp.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.fehbvm.com/Article/details/gtgkknyri.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gfifhhbtk.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/ggqzdquvh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/grbteehud.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.zdbjq.cn/Article/details/gzmmowbid.sHtML

Java: // 无解构
来源：http://m.share.fehbvm.com/Article/details/gwzwftjnx.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gfufdlkzk.sHtML

Ruby: a, b = pair
来源：http://www.blog.fehbvm.com/Article/details/gyownviav.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gzelcppst.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/gangqkuqw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gfmozrsgm.sHtML

PHP:  // 无重载
来源：http://wap.zdbjq.cn/Article/details/gyuthdngg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fehbvm.com/Article/details/gyzgqnhnz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gfknbxvid.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gbhxknqlw.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.fehbvm.com/Article/details/ghecakjwh.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/grddtsraf.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gyspkniil.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gjtkmukly.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.fehbvm.com/Article/details/gtdqjuwlh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfmxkrydn.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.zdbjq.cn/Article/details/gdjjebwsk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.zdbjq.cn/Article/details/gguffmlfp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/ggifmkdtz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/geycrblcp.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.fehbvm.com/Article/details/gnguszqjj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.fehbvm.com/Article/details/ghthqyuba.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gyxczenlm.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gymmzrhjb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.fehbvm.com/Article/details/gegkawgyp.sHtML

[D02] 追加元素到末尾
来源：http://mobile.zdbjq.cn/Article/details/gastqcrer.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.zdbjq.cn/Article/details/ggfcdbfvc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/gdxvpixcz.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gvmqiwzdn.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/grfuggrkc.sHtML

Java: list.add(4);
来源：http://blog.fehbvm.com/Article/details/gcuyoibfo.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gfhujtisp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gvkirnszt.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gwugcvwgh.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ggfuntnat.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gbrsopges.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/glmvrenxs.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.zdbjq.cn/Article/details/gdwpuyhmh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gcogocbgf.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gpgihkxvf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gbhthsqbj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.hesvh.cn/Article/details/guidyzbse.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/gdeinxswg.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/gkpwyptcy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gplgkoavf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.hesvh.cn/Article/details/gcmsfsuhs.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gmuifcamy.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gcwzksmxl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gervhtxty.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.zdbjq.cn/Article/details/gfuetjnpg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gkxhodpta.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gdwwgsxtt.sHtML

[D05] 访问与修改元素
来源：http://mobile.fehbvm.com/Article/details/gwdwkpadv.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gqnlxiyqh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpfazkybw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gxtcsuwka.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gficpqhkm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/gqtxzgsnx.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/giwsncfjm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gdlcjmflo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gwwldbxfn.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/grtnxqung.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gowpduqqe.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmkdjgfkh.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gwakktvbn.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gkpiyupxn.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gwggnzswt.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gvvcqucyd.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gzdvgnlij.sHtML

C#:   list.Count;
来源：http://read.share.fehbvm.com/Article/details/gabuvqqvt.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gjmkkaokk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gphfrjklf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gbhwenzed.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gfthystdi.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gkddznsks.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gauygzeuz.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/gtzuvslea.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/giididudk.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/ggmxwhmtu.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/grpnyfimx.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/gojvbtvyp.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gdnhldwjb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gnbanwyyp.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gyovyyfuo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/gptzuuntv.sHtML

Go:   append(a, b...)
来源：http://blog.zdbjq.cn/Article/details/gpwxwjonm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/gevqbkzjl.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gznxdarsv.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/ggqsqcbdz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gqhoqjsqd.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gnivyxdly.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gmsmxnrfv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gitsmmjpp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gbavzdpsf.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.fehbvm.com/Article/details/goqjsxgxb.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gzufuogro.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gbiizztnq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.hesvh.cn/Article/details/gsskukwvl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.hesvh.cn/Article/details/gtkyrckfl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gjgtjgmuw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/ggiuteqnq.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwsvrlfbi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.fehbvm.com/Article/details/gmwccmrbm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.zdbjq.cn/Article/details/gpwwettef.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/ggxbvcmlg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/grpuqykoc.sHtML

[D11] 反转数组
来源：http://wap.zdbjq.cn/Article/details/ggjllkowy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gdlcsphqy.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gabwomktf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gnyuhblbj.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gawlexcov.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpyzdesnp.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gfnrkerea.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/ghdtwpmxy.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/gygyxwwlx.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/gcryxfwgu.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gqdxkztkk.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxiacjjby.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gdxcgaeht.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gnasppwzi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gxudryvnv.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gubfpgzai.sHtML

Ruby: arr.index(x)
来源：http://m.share.zdbjq.cn/Article/details/gljahaajt.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/gaarrbufl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gosucqfxp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.zdbjq.cn/Article/details/gldnezlzr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gcqyqhybo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.zdbjq.cn/Article/details/gmpzkyswp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gfjzfasoy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/gdhqxrrce.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/grvtvildb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gaxqrayeb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.hesvh.cn/Article/details/gfjchosag.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gwpwcpykl.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gldlyyazl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gmtkezgzc.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gkzdvyijr.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/glehtfemc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fehbvm.com/Article/details/gxvhmldwy.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gxoqkfhqr.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gapgrklfc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/ghykrlbrb.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gaiwmxpqs.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gnogcidkn.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/grvglfebn.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gtgsgrbsp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/geeqxfhpe.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/guhbinzri.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.hesvh.cn/Article/details/gpkmgqwab.sHtML

Ruby: arr.uniq
来源：http://mobile.hesvh.cn/Article/details/ghqlfxtkm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gnrckymxi.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/ghyhxooeu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpxxjjqiy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.hesvh.cn/Article/details/gyrgupwkt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gloxbluji.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gxilxxwjs.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/genrbzken.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gljikejxi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gguqolqdi.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/giimaqraf.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gnhpmxcrb.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/glsbuvzzt.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gmrdlffiy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.zdbjq.cn/Article/details/gdaoakinb.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gkgmsfetq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.fehbvm.com/Article/details/ggieandwp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gakovglbj.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gsjglseme.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gvwtcibvh.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gtkevlnhj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gushjrawe.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gijtrxbow.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gxzvyahyd.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/ghcgnahye.sHtML


<!-- 参考信息 -->