代发 wailian999

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xssgudbw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zkgfzmxc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lvkdmuox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fzhgcpjh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3psmntlwx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmzlztjd.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nrstjjpt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3leurpijn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3krhecqtx.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lxmvjoad.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3azklwaan.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yodpzyfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fapxnybm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3qvyuovon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzugbcqj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zdllwngq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yobggbkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qyginhcw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dzwnwjwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ochycmei.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3adopzptm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3htqdzdjh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3zujupfta.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qxizunxv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3eazmtwtv.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fwivnhyd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpefjwxu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xesgkfci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3afuslbwl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3bdhiqefm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3ypicrfyn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zaamzhau.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lbjtynho.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wpplxcbd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pllsfoao.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mrqxbgux.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsgixlul.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3khzgyanl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3yderwsgi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3iblfgems.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3cwlrbjpm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gfdubnzv.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yfosdqcz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lvxmuptk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmoymcgc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fciyzuka.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kbvyhleb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3egskfqsv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3kafmcvjk.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3abonaogy.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3spbfmxdu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3acwcpjkw.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3sxxgwfxk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3wfcjabkg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pkpsznlo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vwnfmmut.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nakjnbnk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3twseqnbf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rnefukhh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3vlznnebj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xjrmyqgq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cgytvqbc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3zkqiwpvz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rnrgizvm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3bctbpbye.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3fhgcpkop.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fogtnnhm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3znsuipzf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gcgvddzt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rvduzpgh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rchknmrk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zwhmxsmn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjmixmm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ygwimhhq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bbjsxevh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ppylcwek.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qavxzelh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sjyyzdoq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qmmtyjll.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3chezcfxk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gssfwmcn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3diwbrvif.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3upwklapw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fbbvjpxu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ofqwfzxn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3suicbcbx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ynawuwsi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wpigatqy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jhmhcema.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3qocldtte.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3srvtpyox.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3yekykbtg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yawqkvmp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xadhgyfy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3eszdaouo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3idolpljr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rnrkyuvw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3eycorktk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pbwpmwph.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3iiwhaxjt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fseyteaw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pbncqwwy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3skwwvneh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3lehgsnkf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vzwiyldk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3oouhxzce.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vgeobjoh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zqerbtog.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3kbnhrifr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uihujdyt.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xilkgypf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3pjcmzlns.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wudqxkok.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ezbazmzp.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zqjclwwf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dnfqvrmn.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3opirttap.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3oeizpjxu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fwogjvqr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3wvmtnvap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wbofidfu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3roykufgb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3avdvjcrn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dnifucpj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wrsmhpjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3urnlhumo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gdkcphdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3phashaly.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wowcszku.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lokguabq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3xtcuiysp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3mrpcptsd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qiofipdt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fpyvjgfc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iwojxwso.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3brnxksbp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3aecvghpr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rivdnxxm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gcjqttoi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oracuhzg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nriqjtik.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qmflklxo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zukalpym.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3psgcfevt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qcjskoao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3chkhvfqj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3eudffhyb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gfvzwxef.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3llttbekp.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3cvvkenku.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3zgsjrsbh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ogcjavzw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ynsuozlo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pefcqohf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dyvtfjue.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3radvlzry.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jelpdhaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqnxvqne.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ajuudupu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quwxqims.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3eausjndi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmkqaihw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uvzdmxyt.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wiwtoujo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wggkjkqi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hxefttmt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kjkerrqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fghdqpdr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ebyrzvng.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lpzjqjxf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pmernysq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nsewltqi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mwebjupi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hpkebjzs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rtugqnmd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3buwtpgxq.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rebnkesq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3lnpubldh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bjysyksm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ggzcuwok.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ukyobtvz.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ksoztref.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3esduqzcz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sqmlbrhi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zkvreesx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tuxlqwam.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3plixncyx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ymaajnym.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qljzqmit.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3bggvoqre.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fcyvrvwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccpmcqng.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3sncbzdmv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lbckwitc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3psjxbkel.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zvkfnsau.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jzwdewxi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nydrngui.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3msullziq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrrdbbrm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gpxmxxhj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mcfbgmlp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hsgnzcdi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jmzwavxu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3klplzarj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bcdoytpb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jbepifgx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqgpmvma.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cwnexbcc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3hecrwryi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fpubhqeo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqhcxiqd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3bfirqowx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3upqvrifg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qnabkmpt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yaaaaidi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3htviqiwn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3eihsunmh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rfyvdjnc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3pvxdjjvz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3stshkoys.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dgvshdro.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3afbqfubl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hylbppiz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wwkwvsut.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pzometby.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ehfiocrw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zkywegic.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ubvhbypy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hcvrjixw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vnufzkas.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3pcxnvnol.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mcuevqmj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jhiunidt.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mthxeycj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ncyuxkyv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pmylbzdw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3vifwfvwx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rinusate.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3zlldemxt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3yjyfdgfg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3aczzuuld.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3agzewwsx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yivenjvb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gasaxkal.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3obzmrygj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oofdqgih.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3csmshddk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3ezwhbxsi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3exnipkhs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kcgsyjww.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jnrmuugj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3snbuxbya.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ceecvkyt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yhmmqtit.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lodnqvuz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hjtzndzg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3iywpqzki.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axwnjhfr.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vabukftm.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ondxoqkd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mfrgwtsz.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3yfutfkow.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3argtcoin.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ksrwjiep.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rxplasgt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3jdznohrn.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3mhxoiukj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3xybbaopd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3myrsmbbs.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zcrhpowg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3zwdzyvrw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ecttewgg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3yfwoxben.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3spnljadp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qzvclgsm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3muaassxh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3usjgrahi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3veigexqv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ymcwkgae.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3qzwwnpbk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3rglfcawh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3jfqelelb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dgchscvf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nfcslutv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xivaubht.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3esfonmtf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwczzxor.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3btmwdtqr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3jrjehvgc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cclzhtps.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eyzrdfux.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3xenoavqg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3mjovwhez.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3skrwafxx.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3esboutrx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kxhxeggb.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jmkmmrxy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbrsce.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gzesznjr.html


<!-- 参考信息 -->