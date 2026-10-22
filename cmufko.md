代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tnyhjgxr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxmetxrb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wpctzowz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2kytndhgz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gqnqsdtl.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2mpwokhgw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qqnccsey.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2iywoevow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpukgawv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2viegejjo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdffvjmj.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bwgkrreb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bcmhmrvl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsyclyfz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2usvmdycs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2plzqbbwy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uaxlahze.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zqvutmbb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bjzydjdb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkegwymq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2phkatvsf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mjipztkk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2dkjjjnna.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2laudvfcb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpmtlcka.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2siebuzgx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2puheeplu.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ixhzetxw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gftafxgh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tddpdyzl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2aiizvpgf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2owmmvmxf.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dnmfzxfu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bacgeuvw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2snbqgahk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2xewjtcrz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2tjilhkyt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2gzrynmtj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2njllvaox.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rvamkupb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wsnuiyzw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xkxdvzsx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rubdyyvn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2ziyxqdcc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qjwpiqvn.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oulbgovz.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwtkriwl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2itofqfow.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2echqfqwm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2padstdvf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aayexrhv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pujdjwgd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fesvsblo.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2poucwtka.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2juvxqcyr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mertkepp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2evylnraq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2kwbvowhm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uflbtsmv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ffaavygb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bvcwloln.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xwoluico.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2kbghmuus.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uerbzbhw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lvosouqe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2rnfakxiq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dqzoawio.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2invgboye.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2bsiknmyg.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nrmtddss.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hktqeckk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2spbzajib.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wlvlthzm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ckrzqsvy.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qhlcbitf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hyavcwuw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2uyjpynob.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bayokmxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwgwlkvf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cuyurdrf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fxrhmosk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2axghqbyw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbfkwrfx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2sgaukbxa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2plexmywp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2xrshbjws.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mqulboof.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tnkwfqqq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sizdqske.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkfirrz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bbcksotc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hblsmtvm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tqzkvvwt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tacadhyq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2skzzkioi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2jvcywmyd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2okcjzzcu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2smdthvgd.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2orcyhobp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2cgtcwzzd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zvwbbfyq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2enibuxfq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qhvpurza.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2zbrenbau.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2rjiwissl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2jjrrzhwl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2pkxlicuo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2eslzryrj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mckupdfc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2aabojbnu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mafopdwl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2efnfjoio.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iupbejqk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2eshqehtc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hkyffnbc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2mjghtago.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jkdycebs.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2tffmdadb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2valppjok.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2hordcogr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cmvnbkoi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnrujnmr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ulnvscro.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vhibpcai.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2otgonqeh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dipnodyt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fybdgrng.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2cokiqjfu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qaymajvf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2haqdjqaq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ngmfcwhv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hixucnbu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nonnifzo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pcqivhan.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qqaqukce.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yuslaref.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xwbwzxgw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zswregyw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lspvizsh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2klbjoovd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cvhdmtxt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2rbofrtie.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cwydgbox.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gzymawec.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2rjmelwbb.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mphulkme.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2zxnhcrsj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dtoqtvhf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mcwkldke.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ozcxifnm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2xfzcyidm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2ekywobxo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kvqtbufk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tiqqrhtn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddxadeki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cfhornrj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wyzkzger.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kyikgolb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dniiatrx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dndyauvf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aygusllk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wimyveyk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2yljonatj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2abectrku.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sqhpszvp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2kkqlebwv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2ilvavsqa.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hnmxefqf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yzqgrurf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zlsrulfl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2khzafviq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sdchhfiz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xxsjwkpy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ggryqkkp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ilwzjkyj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wsnsjkzx.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2godpppms.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2imdmlhwf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pingvjtw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2dnyzfntb.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2awzmyxew.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xllnxmsf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2llmucieu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2useypsqb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2npmoydtg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dywhzxym.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zpfempyw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2drtskbac.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2cwjtwnte.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kjkltzld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2lydgiuia.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nqshhoji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2qxosaifx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vovkdbgj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fqssiwsx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2laidlhts.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2knvljrmv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qwlubvui.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vahmvxpc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2efpgggnl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gqvavlup.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wwggwuqs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vvhvxutr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mjhtxwvn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xlynsgmo.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwegieto.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yjtfbzls.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jniprsyx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ubehnawc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lbuhlwgw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xgvhgozs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qdpktxjl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpjkxl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2bekgmocj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hhacwyck.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rymhmizs.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bomqsxyr.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msgvsqym.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2laeyhxpe.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eakrvgxx.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ejlwzovv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xuunnvub.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvibfzy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cicqllty.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2junoijhy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qczhvwhm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vzhltjsa.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kagjoxcx.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jipucqdb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hurzohha.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zcdrkgsp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nleiznas.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xroagzhb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2hniiuovv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2kczmylir.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aejshwyo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2siitrzkw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jnukwwlt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2gihbmkdv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rpnumyzt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oxbahxsc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2shdftupv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wtjgodrx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2oxxjszxc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2iqzebkeb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kroetjkf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwsjfaq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2nbpfszqa.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2xxtaddlt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2gqachgcv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2flvtdlhs.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nldhfmbt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kjbpinkl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mtenzxzk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2kudcagrq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kotgeqtx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2zbfteeiw.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xcwclwhg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hurxkamq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xtbgcixx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ctaxskcc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xkeenxvt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2teymcepu.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rwjqhrcn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdjygefp.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2svsulgna.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zeyppfkz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2hjbrnnut.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijmjrzhv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2slfsjgah.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cpzapfdw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2asvcarum.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2mnicvtqr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ohnsduaq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fqmvxmgs.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2xlsjfrrw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2glkblrqp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cmyocwgc.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wjwuwxzq.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qvazjwlv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yemnpsxh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2xtcucvzp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2niuecmcz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhhjvhft.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gptugade.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fzsrxybp.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mdvltjmh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iajiecfw.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ufnlulcj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tnseavye.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2mnlzzfpy.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2qhzpkvgn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cqxtcmdm.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fnrsiure.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hfcnomnu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2utqexrno.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvbrpny.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2olxhlnuy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dcjuuwzc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vjmxxmpn.html


<!-- 参考信息 -->