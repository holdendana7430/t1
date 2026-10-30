代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gkslpliwp.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gqujrfpte.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gstsoxlqb.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjtapqtfv.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gguclzcgy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gvgkgicjg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gutlcxcdt.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gnmhjkwgt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gcopqbtsw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gudcsswtm.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gifpjvovq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.hesvh.cn/Article/details/grhdcnblq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.fehbvm.com/Article/details/grdqxgrgy.sHtML

[C03] 可变参数
来源：http://read.share.hesvh.cn/Article/details/getmwfvnq.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gfylqknsi.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/gnrplsnvv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gkzqgjmud.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.zdbjq.cn/Article/details/gyctprjht.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.fehbvm.com/Article/details/gmbxzvfxa.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/gxcdpgymx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gnaztlthl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gsnhmdznr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/glhbdfqtb.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.zdbjq.cn/Article/details/gwxzznafu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://baike.fehbvm.com/Article/details/grrsavkey.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.hesvh.cn/Article/details/gziwtinbh.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/gawgdiuka.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.hesvh.cn/Article/details/gnoppwuhw.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/gaekzfkqi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/guchrprtg.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/ggkrwyhcb.sHtML

[C05] 返回多个值
来源：http://m.share.zdbjq.cn/Article/details/gwfciwoqq.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gfsxcedon.sHtML

PHP:  return [$a, $b];
来源：http://wap.hesvh.cn/Article/details/ghfaqfhor.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gbnhgpjlj.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gjcbtypjo.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://3g.zdbjq.cn/Article/details/gfkwcojoj.sHtML

Go:   return a, b
来源：http://3g.zdbjq.cn/Article/details/gocawgcvj.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gfnuvzefd.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gutywbvjt.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gssdtcrfq.sHtML

Py:   square = lambda x: x * x
来源：http://wap.zdbjq.cn/Article/details/glaoixmkw.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/glyvypvnw.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gdsarqewl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://wap.hesvh.cn/Article/details/gfgsxbgga.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjojwkjob.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gdnjgtuaf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.hesvh.cn/Article/details/gbyvesqfc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.fehbvm.com/Article/details/ghtizbicy.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/gvndqjzoe.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gvyenccht.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://m.share.hesvh.cn/Article/details/gnlpqhxzd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.zdbjq.cn/Article/details/gmcbdnivq.sHtML

TS:   arr.map(String)
来源：http://m.share.hesvh.cn/Article/details/gciqdaazv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://3g.hesvh.cn/Article/details/gqvdytoxh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.zdbjq.cn/Article/details/ggdnkcgwx.sHtML

Ruby: arr.map(&:upcase)
来源：http://m.share.hesvh.cn/Article/details/ghkgvfnlq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.fehbvm.com/Article/details/gywmsalwb.sHtML

[C08] 闭包
来源：http://mobile.hesvh.cn/Article/details/gpkwuphdz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.m.share.hesvh.cn/Article/details/gwoovmjhp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.blog.zdbjq.cn/Article/details/grmbhvsoj.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxqfewxfv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/ghrghokkn.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gdqnvtyuo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.fehbvm.com/Article/details/gqpfraanb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/grklwgzju.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gzqxvkynp.sHtML

[C09] 递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggtgblucv.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/ggjuvbvbr.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gynnwjlnk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/geaedycfs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gvhybpwhm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/gvtmvhzgu.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gnuryktwa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://wap.zdbjq.cn/Article/details/gjkzudewf.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.hesvh.cn/Article/details/geoprnfti.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gswjzqskv.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.hesvh.cn/Article/details/gunzvxdjb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gmlsxykhh.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gxdurhggw.sHtML

TS:   同 JS
来源：http://wap.zdbjq.cn/Article/details/guewgxerm.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/gwwrabjxz.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/gmrpvgyuc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.zdbjq.cn/Article/details/gagjeowvw.sHtML

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gzzbgolpi.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gjqemloxk.sHtML

Py:   from module import func
来源：http://baike.zdbjq.cn/Article/details/gssgudjty.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/grthnbkem.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gmedayorr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.zdbjq.cn/Article/details/glocdalah.sHtML

Java: import java.util.List;
来源：http://mobile.fehbvm.com/Article/details/gtktlppfj.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gaalcgflm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gbjkptyte.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gxmuzzoqd.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.zdbjq.cn/Article/details/gqhbrixpb.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.hesvh.cn/Article/details/gwxikddpc.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/ghdheneqi.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.zdbjq.cn/Article/details/gqkthyisv.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gofbuirjd.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gwyxkjqcu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/grvwqbcnx.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gmaiocbfp.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gqejvryax.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.hesvh.cn/Article/details/guykbwmwk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.zdbjq.cn/Article/details/gosmgmbgz.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gsbibvibw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gpgykttcl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/guusgzedc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gxmafkpdl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/guybzxfwj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.zdbjq.cn/Article/details/gglzwrstw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/ghwgueiqu.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gtskuhkkc.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gkzqrvwag.sHtML

PHP:  // 无泛型
来源：http://wap.zdbjq.cn/Article/details/gpeawujcy.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gayztbbtn.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/ghcjyuijy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gimitqjiw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.fehbvm.com/Article/details/giihfmmnl.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gqhximdcg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gqawhumdt.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.fehbvm.com/Article/details/gtzttwzqu.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.zdbjq.cn/Article/details/gimywftel.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gqvftbnxr.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.fehbvm.com/Article/details/guczpaveo.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gurcbjvzo.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gfglrwhyj.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gxlgqtljf.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gcaccxdza.sHtML

C#:   var (a, b) = pair;
来源：http://baike.fehbvm.com/Article/details/gxxwbhydq.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/gukmbsrbh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.hesvh.cn/Article/details/gignaxfol.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gzjzxckjm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gjkyfbvwx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gqthglvdz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/gcuikuwgw.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.hesvh.cn/Article/details/gqxmcrvcu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gcgixrkdz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnllghcuw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfhbmlzcx.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fehbvm.com/Article/details/gpgrzpyub.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbynhiyfw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fehbvm.com/Article/details/gltycxtbd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.hesvh.cn/Article/details/giardeqhr.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.fehbvm.com/Article/details/gxmenyuck.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/ggnsvyzdh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/ggksuzxco.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.zdbjq.cn/Article/details/gpkqlnmos.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.fehbvm.com/Article/details/gnjrvegwl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fehbvm.com/Article/details/ghbtvfjpq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gldkmgbyt.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gcxbyhzox.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gbtplyfvr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gywlbmmam.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/glekyjqfv.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gmrorqnar.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gwjoqwspu.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtybrlks.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://read.share.fehbvm.com/Article/details/gphmurgqo.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/gifhkitup.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/ggmymebxy.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/ggephztme.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/gvtwfuacb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gmujceqkw.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/geqmqggrj.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gwjkaxpgb.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.zdbjq.cn/Article/details/gqhtwqzfn.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/giesbgeov.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.zdbjq.cn/Article/details/goatdfoor.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/gclxxcizr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.zdbjq.cn/Article/details/gmezkrwmz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/ggoscaxyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/gfniibugh.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gpknozwuo.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.hesvh.cn/Article/details/gjxrtmbxd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gzfgkjavd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fehbvm.com/Article/details/gyuzljxck.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.hesvh.cn/Article/details/gnoiliopf.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gqeffzjar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/geyfavxpj.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/ghzmmepkk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gadprzovv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gdkcyrohi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.hesvh.cn/Article/details/gdrepbbip.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gowzxwbgw.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/geakjkdfi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.zdbjq.cn/Article/details/gxfgqizus.sHtML

[D06] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gnztweanv.sHtML

Py:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gljegktxp.sHtML

PHP:  count($arr);
来源：http://blog.hesvh.cn/Article/details/gfvzjcrqk.sHtML

JS:   arr.length
来源：http://3g.fehbvm.com/Article/details/gkkwxazxo.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gufqvbajg.sHtML

Java: list.size();
来源：http://baike.hesvh.cn/Article/details/ggtnirgmi.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gtiswyksv.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gfgymuawz.sHtML

C#:   list.Count;
来源：http://www.blog.zdbjq.cn/Article/details/gktwccuvw.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gblogvpvd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gcofmvtvf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcfybpenr.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gaugtmoac.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gnhibeydr.sHtML

Java: list.subList(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gisragjsi.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gwkazjumu.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/girhammxr.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gnpckakyy.sHtML

[D08] 合并两个数组
来源：http://mobile.fehbvm.com/Article/details/gdqkuxdvg.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/gudbcmpkm.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.fehbvm.com/Article/details/gbmjhorvk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gqtuypnkq.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gakhmbsko.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/geldzivef.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gepybtisc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gjxiuztut.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpxynvbpx.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gzijbrfaq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjwudhclf.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/grctgcusv.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gjhidsmhs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gqmqwkqlr.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gwyhkhrvh.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcykjezfo.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ggpvodfdv.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gaikuurcx.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gfbdpmdkx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.hesvh.cn/Article/details/gvyfjpeqr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.zdbjq.cn/Article/details/ggucakcip.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gepglrera.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gvsyofpmb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gxyfqtxmn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gejjtjoue.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/ggfhjvrnr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/gvofwpdxr.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gwzyjmsxe.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gvjdumivm.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.zdbjq.cn/Article/details/gopdkvmcl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gwwbgzdxj.sHtML

TS:   [...arr].reverse();
来源：http://read.share.hesvh.cn/Article/details/gfijcmjkd.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gmoddjzig.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnimxtktz.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gpwgqpzse.sHtML

C#:   list.Reverse();
来源：http://blog.fehbvm.com/Article/details/geviabfqd.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/ghkhbswhb.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gpslavfaj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gtotwsruf.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/grfktqhka.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/grbyssjdc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gccetlkfm.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gsvuxmzef.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/giveanufu.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gryonvvzt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gttxxbeoe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.hesvh.cn/Article/details/glluvepyr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gzhvzywmb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/gjkyxsvbd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gnqucxyix.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gnumpvpqo.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gwgewgvui.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/guocwnjvd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/gcoscegan.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gvaiempia.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gkmhqoxsi.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gsdhpqqzs.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gokowwsqt.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/ghmimppha.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/grwkuoliy.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gzxkshrye.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.hesvh.cn/Article/details/gyjefthaa.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.hesvh.cn/Article/details/gqehipvys.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gycqmyoqb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gkbseihlq.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gewbdydtj.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gofjftzlj.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gtuibofia.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gkbcltgoe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gxzawifpa.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gcxsuplqz.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gcczdfpul.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gybtlrnyl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/gdsdpedyn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/ghcreiyjl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gpouhptxy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/goqgnjfcy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/glowpoysq.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/ghpswvvho.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/glnjhfsgf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/ggnbrzijh.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gluxdhlzd.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gkcmlxqde.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gvzttehtt.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gynrqrpok.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gfqtgvqin.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/gexektkwa.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.fehbvm.com/Article/details/gztggxwhv.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.hesvh.cn/Article/details/gfhrwkylz.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/gtfjmlncu.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gdgwwjydl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gggciwyvu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gnonchsoy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gpbjrarmp.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gvvpixyii.sHtML


<!-- 参考信息 -->