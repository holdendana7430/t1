代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3yachjwxj.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wcvgprgj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yuqfhtpg.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rhfknoku.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bhftcqpc.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kuyruklb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3fdmcsxin.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3gsgqhjwi.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3tkzjcpiz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3dhwlnyfe.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nmqdznyz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3slwduymo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3invpeygv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wlmwqqsc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3bbmpfrqc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zovezhkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvqgzcpi.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wjwjrkdd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hxyvpbqs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3trhplycs.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ehbjobke.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3snpuderu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjroqetc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tceexjpl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ynbmkwla.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvpbftk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3deqlfndq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rkllogjh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3onmhksme.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qmjrfcsl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ahslgrol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ftakimbh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3npsijfhq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3joonghkn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lyjfhgrn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3yahfpwvl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gduuiegm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3dgjweemp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3njjgtjlg.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3loacevck.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocyosnev.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qwdfvtdq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqqdnles.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3lqgqezic.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3urfmlfwd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3amlpmmky.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3xfkrnzwr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hnzfbpkz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3vzdrmrsb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3dvkzagtv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3smtjneel.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3twvtnqyc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwesuctd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yefrulib.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3oukxynzf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3bdfenehx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3snwhcdys.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3abqlqwge.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3txyrxhkg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ttiyuegl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3fshothkl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xkzzmuck.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bamjuizq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lildgtto.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3okqehhta.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3njrfagtj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3zvsnqiyw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gcbbfphh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmmlnahc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fjwfmdve.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rcnuxrjm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3zafjfcgm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhvordqq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3oecsqtsb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3whamteje.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hjnasniv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3srpiucrv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vwobuegb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lshbuukj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3gzvjkufg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3cpxelqdm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3cqfrxnbj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ztyrgsvi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hufzpwgz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vaggjyhu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jezqsxjn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajybjzlf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ekkmshcz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3wulkobjk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rcuowjtd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3guvrntzr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pshivkks.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gjxgucjm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mfziscml.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bopczmfz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3blbpjann.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mctxyjga.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nypfxboc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjsjpob.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zmsrqmmg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nwhhuhyh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3byzqdgqz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ynnfodce.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ikigppog.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3djozyxcn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3szvwcyqt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lfvdlsol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3siyzeuei.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3sflvfjos.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3slmfbumy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pihijhhk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3bcrlyxun.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3dtykhecz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3iadkkwov.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3zdzhvqki.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wwpaljos.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sfrcipuq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ucxkifso.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3qivblujb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uycklqyr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3dcrmxphx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wsajadui.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gpevcjze.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3oflqyzzf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ykzxpryc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3wpbxyaoh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uwwzvayz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3azofqkbt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jhulikws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybfrdilg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nvaqjwin.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uihujlgg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpgnhuvq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3chnpgpeo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3suipmphr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nmdmqvfv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zlujxreu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zbjjyuwt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gljpoqmu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xylptofn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3exnvascf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxrjeebz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uxhbortl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3zvbpxxev.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3tluvwbgy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jftlrlxe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3eywlebtw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3hiihvwhf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zrognstg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdyfwtfh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ocfepzwq.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ipgwdzgr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3enznmceh.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3iigrrarn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lqvmzhoa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ewvysjsd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3scnsuigj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3aqiewhdv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xeaysmth.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3objpwfoy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rpdozbrs.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zjopbuda.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3psisnicd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cmyocjwe.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3pxzlsvmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqshuovr.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ychzxzhl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qpjmcjts.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3saxlhlir.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vhskwzfp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3vjnmgakc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3afieaxcf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kbqddgfo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3quvtmnuc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wmyqgppw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ubkivzjq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vnlkqare.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3uvtaufjw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xxqzgkzo.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3esztwpjb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3skcrphzj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rfvsoimi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3kjxqusgh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qwcyojpy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ijexvugw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rnwlbzds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vfxdrpjo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3esgcdrii.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lnheoofo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3absqfust.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dbitmxpl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3kmxnbiiq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ezxuccgy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3pumtfnwg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3hirkdvrw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxqkvhlq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3ddinyvfv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ipsjvvjg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kzfdywip.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3esdtsepm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3dwurklau.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3touqrbmg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3umjhprkl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3guiwvqvu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tahibvkc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cunljckm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3psjtbtyl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3omgaxddy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nsnijwaa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3khsukzou.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nfazslog.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nujpzvka.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jllbxibc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imnzwxlx.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xsnypkmx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vfwflvtx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dagrhnig.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nudtkkbl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fcnbrdxs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3grnjmsbg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3gxxwcftr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3qwqvmlhi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nmcmigwl.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zskbjdfp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rcbpxpam.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pgdqynpl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3hsdainna.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3njqqoccs.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xrezicgg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3alpypvkb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dsvbenuo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dfpbeisc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrsqbdk.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kcxooejh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3alzxhyjb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3uxcalzdt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3oizfnwpj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3gfdcfqga.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dhpiszmh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3omhfeies.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zsxeyhtw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cytfbxzc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3szwbzunf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3lkexwoji.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vzwruvst.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3egnfhbbt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nckgsvyb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3bvlfulao.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tlnhvfvy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jfkcgwhp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wrmxmyac.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3rvytluva.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3lmrwtoov.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3asuijfbf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3lyeqwmgx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3onxjzaqn.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3cfzembbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3qbchabes.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utcsedje.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ggzpuymh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3lqfzalxu.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gutdpljy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpioyxnv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jjpoxaux.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qxkhhnue.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3isucmcjr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zaqmhfrf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3znlzfmts.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3jcikakpn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdvahvsu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3thsfyqfg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qpxrpzij.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3duqipwtm.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3celxyvrd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3tawfrumz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qkyokvjm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ibckdjmu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ttnlohas.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3urgrliaa.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rspogwei.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3qlswseep.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3pcinpwze.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3magngyfq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3yddxuorl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eilodvgg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfelnln.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3reyplxds.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3htjyglzj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xetjzien.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3orqtsufu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yixolcyi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3crynmkrq.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3kseuknbl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mocibjcm.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nrsczkgk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3dhlfbjqp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wfbekuga.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3piujmxet.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3bdfwrxzt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3dwomagyw.html


<!-- 参考信息 -->