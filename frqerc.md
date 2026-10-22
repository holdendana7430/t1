代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2bcclotqg.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2aomogayr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2abalrihe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hagynsvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzaxcrej.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2uvoyhrzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ylcgdmqy.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysyubjjg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zgfcldvs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hbyqunva.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qxchzcsi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2exkwnodi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzvmtvdr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ktcojsov.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yhonihcs.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gprptcoj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2htwgqujw.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2znkbgrxr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwtczwmt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lemomggk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fbvbntbi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2stbojtwu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jsifarmx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yrhjnjif.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kybjjvng.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2camvohie.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dmqbklxm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rhxtuhzu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2wwujlsho.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hkueqmsq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2dkssgvsk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2lvxgsrnf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2kokorypd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xjrypiog.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2evclkklf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fmwisbak.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2jeqnoplo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wvflqkgw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cgearaln.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zoratyqd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2bcemcplm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gwryqyyr.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uptokiry.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hfrukxjb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uexeyjxh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ftsftdgo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ggkvwkdn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ymijuxqv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2mmpjexwp.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2kxjlteho.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2rfvpuutx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2enejgyju.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2twexekrm.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ttvptkfl.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2kdpfhyku.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2husqlqsv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pzeijndf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vhdwybuo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2evdwvxbg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zprchzas.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ruyqxxat.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vfxzgfop.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2gtjudxnx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2cbqgxvjw.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jrjngfhx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2kodwvsox.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bnbculpe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2krnqqquo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgelhqx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2issiybdz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2itibnapk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2tuokppqw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlgjiqgs.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nbazkbzp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlrchnum.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2gclbudkl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdxqvdk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2qbuvtfiz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2npvyphyh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2wmjxjshu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eyaxxuht.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tlihvkas.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vprmajtj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ffffowbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ivmmigah.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bzbbhywy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zegapblh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2aokvovtq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ojfcdiqg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2tenyymor.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2owtlwmjl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rfzzprxd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2grfotjid.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2otybkfch.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hrpqfttf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2bcpnngnr.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xxlqzour.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pnrwaiwo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pdqnsqgi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qpjkvduk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2njeivhcz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2tlnuptgd.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2caqvotzu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ccylpabu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2yjiqvnil.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qbuoemln.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2fsdtczbj.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hxidcqgq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ritjmmhu.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2eygulsqp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lldhwegs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2rpwzorae.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2gibjpnkt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dsbuqigx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zukepgrv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2yktfkcme.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2uhirkhkr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2scajkpzx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2tllpvcpy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cwneoczi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2affrxugd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hvzglqlo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zmgvpzrl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lfzxeuxx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbpnpelm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ikjoejwg.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kbxexlfx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aonvajbx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gedtmtsi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tkrsdtva.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uunlsozb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sqvidudj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2slvikvnx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2rmgltrfz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2etahhcao.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2gzsrzger.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yyxogimy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xrhkdpoi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hvvqwdvd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mhwjesfm.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pvpkomks.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2npvvipve.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2kwoeejzv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tiwzzbir.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2frsuwfpa.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2icjoprsc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2nzytljzy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2obqdjblh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fbnntgxh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2utyrtizh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qwroegby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ziqoglyg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2akjfwdsj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yptnsjga.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qkrgxqxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2polmskpe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hwhpxnap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qdpgcrho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2gawimsfa.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jyngyrxg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2ifhzoklr.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bkndctfi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xfglcwne.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ctcftihu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dsjktkgq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rddsuutr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2keyuzkzu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2rxpcvcjz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xmgntmed.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ucicvtsw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2wgmsmncd.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zvjsbntq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnmnxuab.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cxxngnot.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybwbwrma.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2narxypvz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bljmmqlp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2esreovjo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlkwzts.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gbbnvvfa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sfrxmdjk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2frspkkue.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2clpzpdka.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2yymcejnm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2glvofldi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hpekhoyq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzrgermf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbormce.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2lokzdvun.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rpoporjp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2oxunrdpi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2unkaypfl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2szcnjgrx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tqupvxmy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2edxygjqa.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ixywwljy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gfbzsqpl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2gslonjkl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qlrunjez.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oeofokgk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dqifgzxc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fogfgykm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tmelackj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2uuxfaouz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2izqqhbdq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2svojtljk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dcuwakgy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2chobakqq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2lrrkvofb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hdsbshxw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rialcmuv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2refgjyag.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yvullbyx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nlmzmicj.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2xllkvjbz.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2idtbxaff.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2okqzuqqu.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2lehmmpoh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yvpskvsf.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2lmtqlelm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2ddefdjgw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jfnvulbr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cntkoxmy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzdwkud.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ddgjtkpv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2okokfvxg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cewuolxf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nbkfoiba.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dvlikkao.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2gttulcft.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2isazkpkv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2iikpcizu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lnvuixat.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xwvyefak.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2uxebkpbr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2excegxpx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dbchefpo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hnpfrkqi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vdiawafv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2akhczzzs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ztcbblim.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2osykgubj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2egphllpz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jzvcqpcd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zxeileqz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ngkldykm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2eoeehudh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2vsbyhvee.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2urncpwlp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hlillhyg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gasokpqh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2dgsjocmk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jgigkjfs.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2svscrrvg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2vxoplunq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ykrdqcwj.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qcfqugig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xjopiqfy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2zpzlwxsc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zukzgykg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2zebjqqxn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2vynbjmvz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lspqjloo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jutsztox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2dpabethn.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rnbnoyrv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bbgbzmxp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mateyqwk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2jggtufon.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vqbsqwrh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2cibgmdvr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2hcfwkwxb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2qhvrjfiw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wbxzsgln.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gguhxlnh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fmckjhqz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rynnlhqm.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pjlcgtyw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2amrbptrn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ikzzflgj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jmyzcsmb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2whhfulug.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2inyqerfd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2aleainsa.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ypguojcu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zdgxuwjo.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2azvljcuw.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2imppkbya.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2milwnisy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2fetuyjkh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pqwvcagt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lymrovsx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bxvcomsb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bqahyshn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vnfdteck.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qoxdfcah.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ivympxyd.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2faywwhkk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fxfweclm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2mlfbeeuw.html


<!-- 参考信息 -->