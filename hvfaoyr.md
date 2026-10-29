代发 wailian999

Py:   def add(a, b): return a + b
来源：http://baike.zdbjq.cn/Article/details/gupnwmozj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/genzaizst.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gfimhoepi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/goekusjsx.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbvzzbcge.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gsvmxbawj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.hesvh.cn/Article/details/gqruuvddg.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/ggbgnyccz.sHtML

[C02] 默认参数
来源：http://mobile.hesvh.cn/Article/details/gweagtyev.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/ghsmqsafc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbnytheim.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/ggnzuuocz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gambygirj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/ggerkxogl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.zdbjq.cn/Article/details/gklupcjoi.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fehbvm.com/Article/details/gjmuybifr.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gttxtigoo.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/glwbpnipv.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gwvlpdklz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.zdbjq.cn/Article/details/gjvrmbocn.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.fehbvm.com/Article/details/gfopxksch.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.zdbjq.cn/Article/details/gahzlwoto.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmlmllzfk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gglhbwqkd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gnqsnmjfi.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.hesvh.cn/Article/details/gqrecgdvx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.blog.hesvh.cn/Article/details/gbwfpgjbe.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gbmradkzn.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gxqijhvro.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/grhzchuky.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gdzhnfcly.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbftpbg.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/glffmlfkl.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gnpujwfhr.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gbsrvqjuw.sHtML

[C05] 返回多个值
来源：http://wap.hesvh.cn/Article/details/gmqadtkxn.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gmkxlrlqb.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/gocltrwiw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gdvowezyf.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gshbsaypm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.fehbvm.com/Article/details/gnuzgpuzy.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gxffhugbl.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gbgbqxzaa.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.hesvh.cn/Article/details/gxrttznde.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.zdbjq.cn/Article/details/guxyvbpef.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gekcmldna.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.share.zdbjq.cn/Article/details/gwrehwkll.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/glhpcpxar.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gmzlapqhh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/gjuzcaknb.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gsgodruji.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.zdbjq.cn/Article/details/gqukcsqun.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/ghahqrjuy.sHtML

[C07] 把函数作为参数传入
来源：http://3g.fehbvm.com/Article/details/goalkhxtu.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gpvsxggxa.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.fehbvm.com/Article/details/gfakrxvic.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.zdbjq.cn/Article/details/gwtukyjdq.sHtML

TS:   arr.map(String)
来源：http://blog.hesvh.cn/Article/details/gfvqsihqy.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxkfefa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.hesvh.cn/Article/details/grgwkbelq.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/ghrqmtpay.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gtudtrauf.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gcsjnannz.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.fehbvm.com/Article/details/gjijotygr.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.zdbjq.cn/Article/details/glaifbtgo.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gqvyqryak.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gddulzafd.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/ghtovyaus.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gasrtlyxc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.zdbjq.cn/Article/details/gmdmtduyr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gnfidznch.sHtML

[C09] 递归
来源：http://wap.zdbjq.cn/Article/details/gjqroqlfc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gerlxqkwy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gdgrrawhb.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gqtfdsnlw.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.fehbvm.com/Article/details/ggqamixtx.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.hesvh.cn/Article/details/gdeampzxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gjyzjyedw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcprvkwva.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/gvoipzgfc.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/goosloduj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.fehbvm.com/Article/details/gaqlhnafr.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.fehbvm.com/Article/details/gbiwkzzph.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://blog.hesvh.cn/Article/details/gxwjeapig.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/gfbjvjlto.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gfkrcepdv.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/giaokgtih.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gbihfucuf.sHtML

C#:   块级作用域
来源：http://baike.fehbvm.com/Article/details/gzgwgrhxw.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/gpstsyudi.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gswxxsjcq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.hesvh.cn/Article/details/glwdgizrl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gzqswqegu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.hesvh.cn/Article/details/gzbserrvt.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gklyrbotb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/geqwtwmor.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fehbvm.com/Article/details/gquurwtqo.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gzxiheepn.sHtML

[C12] 立即执行函数 IIFE
来源：http://read.share.zdbjq.cn/Article/details/gpcpjrlsx.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fehbvm.com/Article/details/gytalvqfv.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.zdbjq.cn/Article/details/gyzsroivz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gtnelenyc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gatdalsth.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gdbfcwzsx.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fehbvm.com/Article/details/gcowowyys.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gawlklocs.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/gjjmqcrpk.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.zdbjq.cn/Article/details/gdtorjcfh.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gmbfnryek.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gqihrovds.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.zdbjq.cn/Article/details/gzvduinjk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.fehbvm.com/Article/details/ghqdurfkk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gmxokxiol.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.zdbjq.cn/Article/details/gieiekcmk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gxnmbntzj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.hesvh.cn/Article/details/gkrjopkzl.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gpxeckvuq.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/gedcfrjah.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gfwudaptz.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gnvqswqdv.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/gpuasmshv.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/grmxtryue.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.zdbjq.cn/Article/details/gpuvkevpx.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdrgmiqzl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/ghydllstu.sHtML

[C15] 解构 / 展开参数
来源：http://www.m.share.hesvh.cn/Article/details/gqukcmvvh.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gtopsnfpq.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/girolqzxz.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gwoausnew.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gfzpfvpik.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gfppjpryn.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwyvlolif.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gqdywtgdt.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.zdbjq.cn/Article/details/gbdnygfic.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gatezxetr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gzdrbquil.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/glfsmyxwo.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.blog.zdbjq.cn/Article/details/gjhdpggsv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gzqdodvpx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gonmjajdy.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fehbvm.com/Article/details/gneanzttm.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.hesvh.cn/Article/details/gqjaqxalj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/ghyckvysp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggkadmlbn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/ggqzrezpw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkzkoxllg.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gdjxmbaue.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.zdbjq.cn/Article/details/gsnbtpteo.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/gpyzzsios.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/glxdsvgbj.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fehbvm.com/Article/details/gojlocucl.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gwjcalggn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.fehbvm.com/Article/details/gytbzlbys.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gskyoefns.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/guqhrdefr.sHtML

[D02] 追加元素到末尾
来源：http://mobile.hesvh.cn/Article/details/gykuloyjz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gonvncpqk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.fehbvm.com/Article/details/gbpiglfmy.sHtML

JS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/grluhmizb.sHtML

TS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gborxvdqa.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gohwsccja.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gjrjjuhjq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/giieavrgk.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/gzavnixqk.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.hesvh.cn/Article/details/grgikvvfd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gmmvdmspz.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.zdbjq.cn/Article/details/glhpyadvq.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gmeckldsp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.fehbvm.com/Article/details/gamhpsogl.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/grjlybhnu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gjgcjqvjt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.fehbvm.com/Article/details/gubwhvqsy.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpmopucpv.sHtML

[D04] 删除元素
来源：http://baike.hesvh.cn/Article/details/gxlgqhkju.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fehbvm.com/Article/details/gfftlfmml.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gidlazbzn.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gpxfqqgbo.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/gigdglpyy.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/gftoqbxwt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gonumvjxa.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.hesvh.cn/Article/details/gtgwfbtlw.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gepxvbgfs.sHtML

[D05] 访问与修改元素
来源：http://m.share.zdbjq.cn/Article/details/ghcqxyemq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gbmztxgny.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gehicbnom.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gnpocivrz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fehbvm.com/Article/details/gyqeivboi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.hesvh.cn/Article/details/gcjwbbgur.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.zdbjq.cn/Article/details/goziuumkm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gsyvlexso.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gkrnegrul.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gqosiqdbi.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gpbxazzbp.sHtML

PHP:  count($arr);
来源：http://read.share.fehbvm.com/Article/details/gzvlzbbfq.sHtML

JS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gnkkmekys.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gptaafucm.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/gxxlzirel.sHtML

Go:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gczpgvxgr.sHtML

Ruby: arr.length; arr.size
来源：http://baike.zdbjq.cn/Article/details/gmomkhtwm.sHtML

C#:   list.Count;
来源：http://mobile.zdbjq.cn/Article/details/gngfraxoa.sHtML

[D07] 切片 / 取子数组
来源：http://www.blog.fehbvm.com/Article/details/grkdutlcg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gomkyqygg.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.zdbjq.cn/Article/details/glibghkys.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gomwmkqbp.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gicnqubwv.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gfiygpkdn.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gmnucatsk.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gsqslapbz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/ghdgprfuu.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gmoerblks.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.fehbvm.com/Article/details/gucivrbds.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/glsrtqhwc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gpskddvci.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gzwashgzx.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/gpixnfjzo.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/grcwuqprm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/grvrthqyb.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gzccfmhly.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gvicnxalt.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gpdueibvp.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gqxcuacoc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.zdbjq.cn/Article/details/gbosprmlb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.fehbvm.com/Article/details/glgdieqec.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/grvhoewee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmhparncm.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/glaquxcmp.sHtML

C#:   list.Sort();
来源：http://www.share.hesvh.cn/Article/details/glrfnwfls.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.zdbjq.cn/Article/details/ghwqdcroo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/ghgopnwss.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.zdbjq.cn/Article/details/gyookzjip.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gqeudiwpf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gmvetmtgk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/ghyojurim.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/ggxwjqjnr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gdgypnpke.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gzcpgmdmf.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gcvgmlzyn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gyomtqhdx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/ggxzareqm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gwbecuzul.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/geodarnrw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gbvlhxrcs.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gjgmdfqkz.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/geuhcacpg.sHtML

C#:   list.Reverse();
来源：http://wap.fehbvm.com/Article/details/gknhptvmx.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/gchzunwlu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gppktkhvc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gzyzdswsh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/geuveezpn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/ghfmuxqqp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gzhyrzphk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gtuelvwvk.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqnymttje.sHtML

C#:   list.IndexOf(x);
来源：http://blog.hesvh.cn/Article/details/gzthxlvvk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gklgpwuty.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/garsbukyv.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwornmh.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/ggikicbqq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gigcanzsm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.hesvh.cn/Article/details/gcibpkrgl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gmlnasnns.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gvknrsbly.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gsztnmjxv.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.hesvh.cn/Article/details/galsojjwz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/gyrmmkbyk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/grfitetih.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gitednqnr.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gulkogscm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gqnfggyrw.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gdidncxth.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.fehbvm.com/Article/details/gnhjbljdj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gxzcvxdjk.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gzvoqdgbq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/ggrbkdejg.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/gapwcwrid.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gvvbjmwwa.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/ggzejvcei.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gffhurnrv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.hesvh.cn/Article/details/gneewaqmu.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gfjkgtttl.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/ggpafxqqh.sHtML

[D16] 求和与平均值
来源：http://blog.fehbvm.com/Article/details/gsdljwtoy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gdscpauxd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.zdbjq.cn/Article/details/gulloduwv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gqwgqlqmx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gztlzgixt.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gtnrjcubh.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gtfcelhpb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gyijgjges.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gdlywxwgq.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/gncdlxtgs.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gajohmxqb.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gimsiudgi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gqexvznht.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gfsohybkd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gvflgrqtl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gdgdmfezm.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gyxxgabfa.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.fehbvm.com/Article/details/gnsuhwbvm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gcezcjoth.sHtML


<!-- 参考信息 -->