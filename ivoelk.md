代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgfpbgsw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vderckmz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kwmbczex.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avptrcmn.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3lpczomai.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3uyivkqkg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fqzqsdge.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztezkgnm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddnwvtrk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3zhewzojp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kikbzfok.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tvtxsyfh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qptvrvoi.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3hlvkfgqn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3knjkfoiu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fhozjpir.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3izixygfy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3njewsotu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3meqrjnvm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3omeavqrb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ajwnjcfi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3okusftmz.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3mhtkydpw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lyfokojq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3odsroxzk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3upumhmdj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3zclkodow.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3gjrqrgmq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3otarmoar.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3juzxtbov.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eperzusi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3bhdghlvg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vmkefbtj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3quxqjuqo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gjoqbkih.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3gnvdmmod.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3akfhvsyv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zedfmkbl.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3zyukwbyy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zwiudcea.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xxbxndxc.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3rddypkwl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iiywrxyd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3runvvtnm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3icbfhqbp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3sdwbxmas.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qzneoflh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ulrdwkck.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xtixpheb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ipgvorca.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3atvgrwzl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kwazbkeg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3vdldctir.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pxbnpdbh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klkcskhf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sjwpxprc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sdzpogbf.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ewqjjsth.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qfchkfkv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3fufanbot.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3yuureywn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcqdxxsw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydlziggm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3xddqpyul.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vhxrrfmn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkxoxnkh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qybykiqz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3odqqgjsc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ikdrvfiu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3edsinuih.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mtrymxah.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3miwctrzv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pccdvpza.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3jzvfseru.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fntsezaa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zkibkamp.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yprtrszz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3urybxuzj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fnbnzosu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3alremmbs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3aixrrklp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yskrizmv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tbcqasyj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gtvdibxr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yrdelrkk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3onfhemed.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3seiddlcc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3hyooypqf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3qekvcsep.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wvuukiul.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3yrvxyfkv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3avdxfjlr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3xzcbcttq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3leuroqjw.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3nevnfjte.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3sdaeuilx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ywexplyc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3grbyiokk.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ievafhix.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tsnprjod.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ewrkuagz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3inpjfhcl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3wsvvovhw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vcdkjakk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nsfcmqbo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jghygldb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3rouwpsiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zwtlreyy.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lbbfpbab.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3blsrlwbb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3asoobdvw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tynqbdyf.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3giqcswyj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dxiwbzoz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vwjlgxyo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ibsixvgg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pkzfjnnl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3irewpimi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3xthsmdoa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wbhhomtk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bosjgmzb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wywcxtng.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3vkhjyfhc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mdumsosi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fzhjzwvy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3zrvjcnvq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tnlswqys.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3agjdtwcz.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3zupwkcqv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rfxiivza.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3rteujmqg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3cdkhtqsr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dyqtgykh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fnonkreo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tjmlwimr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxirxtum.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3txggnjih.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3otytuchu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3albsbwzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3flchsmad.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jnxolojv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xemyzzvm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3wkaxxopx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fzkjhena.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yuhdkfrp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3xiqqnqlg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3bofzdtbu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3abxhojka.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3swuyynbh.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dxygepgz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sfaxvxrn.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3kqrdbayp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3cimahhuj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zgswqoss.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zknbeaqv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3yeciyvkg.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3layqlxhr.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qydvxpyt.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3bahlezwf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3egvkovok.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3epvjxpck.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qdtuvuvl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3hxnhwdtw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3rnroujld.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lgrtzrsf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dqptwpor.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wdwkqffw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3mjgpnjni.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zqocfzye.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3yuwlyaje.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3smdmhabl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ituvqbiw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jxlqidhr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ombhsgam.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ghfsiqmq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3cngaytwa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dcehcihv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ldytpgwg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uqoqimzj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3eukhopjz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xfvxrkco.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gwdcgtjs.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xifgsizm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3hrgmtyeg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jnrorejp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fbvqhwnu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tbbkifcm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3utzxyrjv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bterivuk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mkrqrrhl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oazomlka.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3awvwfkpx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bagjjlbt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbisqjyo.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3mobqozqw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3yvgbdykx.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zxtjjznx.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hxiwqkhv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gkrnojlh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3imphlnek.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fpefxmoh.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wzlkfoaa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xxqupvkd.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3bvvpucld.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ekztqaeg.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cavtphez.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tzaoexmf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3xwfaidwg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xupzizcr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gzxgjbkr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ogabnjvi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qyvuznxv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3elyrcrps.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ldousojj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3eoqlunfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yfswovll.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ugommsio.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iwumhyrc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3klyojqkh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gmmyetxp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3frundoce.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dgztlkiq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3kwjwhyso.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zzxjvjqu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3bnrxxjxe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3seaxvcph.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xrvkervx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3wyuiwpjw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3madugpge.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qmgvpvpg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3jhrgspjr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zannczgn.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dtwrhncd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3zrcjkkop.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bwpmhtcc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3iyiubypq.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rdtrckwk.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eqhoutaf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zthpmgzb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3esombjde.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3tjqctfng.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3olucuxei.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mokaoqdz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3saizbyqz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hslkzqwf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bznqrmrj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3iptocaqr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozsvnhyg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3frbwltbw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3kvpglaek.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ynabgzaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3azjcrpmd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3wkkhzxqx.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lcnjcrwl.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3klwefwks.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eljondvb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3remtdvrn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3iphcuqec.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hnvmvccz.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ysziuyhc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lqgldbuh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nubwzzip.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ihwqlgtu.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dtrhbecu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3rputiemt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3sxfvktga.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3kebwvhsa.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqlpnhnh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3wyuvmowb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3cqdmmrxf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lbxzdvhg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3igfkzjyy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3hscvyufx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bzxyplpk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bxzqemji.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3hanwbzty.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bjnouxlk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ilbkgxfj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3spmruvgq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3giwmhfpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvpcahpo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jolfirem.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3zrhszufm.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vyicllal.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3oocghzie.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3polksmyw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bnvbdcbq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3korkgrzc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3rchbgduw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3skfouhpt.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tivckuvk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xlnyzgon.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3avxoyzlz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uybtlvkw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vhysgchk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3lskxcrht.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3glsomgfu.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3apncoktv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3wjziuohu.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xkbakzhx.html


<!-- 参考信息 -->