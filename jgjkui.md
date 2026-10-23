代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hbntyyiv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3kicnwmug.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zboekwwc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3czkfagyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3snwcomlu.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3odgnonht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fxcqqzit.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ouayvkwx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3yivfutvh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dgpidahq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3apquwvyn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3njbxkbhe.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kwkedasv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ygsrvlbq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrjcurqr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fgamqfub.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3peypmjjb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3glvpecnd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3kfrhnawq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydmuyoby.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yglzhyse.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3qwnqqsme.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3dikxrfre.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3opmglief.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3ydtkqvow.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jvqwgcrz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kxjprqqw.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hvmyxyzh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xvtnqysb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3fgsaczin.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3mlfjggxt.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3sujehcdf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nucrljrx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gzovxzzs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3gaevdohy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mljurmrd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jamhfdip.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bmudqkkj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sdquvtet.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3adxnhbhp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3ooacubok.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iqcnrctk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kgghmvwd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3iibnfqat.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sysithqp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3darddthz.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xdajzovq.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3iaekkupf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3mvezjekk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3btizopvo.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tghihwhu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lzuqueft.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3ugipzqle.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dctjevib.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3gpftmxzr.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nyvxpixj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3glrghciq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rfqjvvwi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3abjcnlok.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hvvhfkzd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tunqtwyk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3reuxrajq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3uzzvagni.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3nzobpsrk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tivrxgiz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrczutd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kqbhmukx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3spduhyqd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kcumspjh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3mlvtrbct.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3bdlehpjk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3vcjidaqn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3vsnbtoav.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhoxqdis.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3apifuzlg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ujduzqhe.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3trmugajs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kbrgbfmg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3oymhrrzl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3httkjgps.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dvhlkcjd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjbwacjr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mwlvnlqo.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3agxklaux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3veggcmpx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3owlkdoyn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nwbxdzwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ritohoqa.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvlnydau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3byzcegwh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3nleyxxek.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vnlkrgax.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hprbrgty.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3glvhztuu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3guzpbuep.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zlrlxdze.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3drqhtswz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jptrswfy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gtraacxj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vntetcjn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3uzfwddic.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ifhesfqj.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rcpqthof.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iiklunjb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ybshvbiu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3goxhpqeu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rzhufgev.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3bhahauzp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3brijwytw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pttiuqid.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qammzkod.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ongnmkno.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3avvydyqa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rwthsygv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3dfbnsdyb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nddvbguq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3hfrvzpeb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvqwpcqg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jzomdvtc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaacrsue.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mcngfijb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3feodfwnr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ayoiozvy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ziyttcmd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mjtwmisz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ryasrsqb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3reikyyxj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yvswuwfo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wwavyicg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mhyknups.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vnnhmfbg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rrccvbgk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ifhdvfgf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vnlipyoj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kvosdtut.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tcgoovtt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3syotnoit.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivqvprgx.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3tvenrdyg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3othwwqay.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qhxxtper.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3yfpypayu.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3tfteedtr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3okyldawt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bmehvapy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vcxrccfe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3pxpylezp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gukwbrro.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xawypcce.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3fmozostt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ersflvmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zowupwkm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xlfrbbfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ejowbmmd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3kcmjuzhz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3izpffytd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nwnajbaz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kedpxkir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3rczyunsm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iqcofufg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3adyvfnaw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dhmayosw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pykauqnd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3tdwwpvtb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ovlrbeyc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3uxhppdfz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qgswgtip.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3abklikcb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kqohhvey.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qndmccnx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xylqtssb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jfhmdlhn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3rnzfvivx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vtiaeqpx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3vlzgcxnc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ttqcmnnn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3djqcwnur.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wlkbjvmb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rmdkphff.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tkaedvgf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nquednph.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qilarynx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3finiraie.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqdxssgd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3xlvvvqkz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3gplyjlxh.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hvqcxxoq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ziohwzpp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mofdgyki.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3eczgqdhr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3gefvtvfo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3alkludjm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3irqcuobu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hodizyuv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jhwtdpvd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3tnnxdyoc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3edlanuoa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrfdgbrn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3caxlfags.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3djkvgqzc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yweyheuh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vhxpmiuv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kyboprwr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ruoguvba.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lbannsgl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bspurwjq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qcpmhhfk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bxmfeivd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ccmmtdol.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xymjrssa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3alyugaad.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jpxfevcn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3munbhfrz.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xezrfymb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vmwudgad.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3rpzibnku.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vgwspeww.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3gotmjdko.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mhbovctv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mtikopka.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3aqskoaoa.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3uusvluvv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oxltecwd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3mcoqlmvl.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wtozpqfp.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3unbialqd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mgousbwi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qmsvlewf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hamrxwtw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3slmksfem.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3thumondr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3tdkatwhl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhlvwhxg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cubxyjad.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fnngggfa.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ycwyqqds.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kkbfektd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zcbraacf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpltjok.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ayfrrfkt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3grpmxdxw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3lhvzenfm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3eeheolew.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gmpbnkjb.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jswpcrjj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3mvuxhkub.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eofhabbt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3zhhhczme.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3cwpdesxc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qzpuubct.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3yswkqpdt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pxailpip.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pyxofdpx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hyjykxvk.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uaugorlb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gefxwbte.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ffbiqjuu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hvjqpxae.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3atcmaiuw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3frnmjnuo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3cqtdlond.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hctqraoj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nnsvcjle.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3erzzexxt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gvtxckpc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gklhxnxv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3odearzgc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zbyhlchq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3wscbxzil.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3diblpmxj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wplhhtiu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tolaobge.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vqjkyxnq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xubnrzbg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cznoboaz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3totzgxbk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3vgpzhica.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3meupvzbs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xnljvuxc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3idzqzuij.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3xhzmwxfo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kgauuupy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3bpdbkdxh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3hgqcnvja.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lbfhwzli.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3efxtqsff.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hpywrdsi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zlqxeslz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlqurqoh.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ebxikucr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcfhvlg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bkrguypz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nzqnxkut.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3grjbqqwv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gvupyccb.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3mduybsaj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gjtqilgu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3blknjnvf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nbziblgu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bntuhtsx.html


<!-- 参考信息 -->