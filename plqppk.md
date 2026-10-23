代发 wailian999

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rsozicxy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zjhsuhef.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rmwzessz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mfzmlmfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lppkaudm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hgogwvdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esxclwie.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3nugrskcr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wdwpkbqz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pwhqjegy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3afrcvrar.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3caummqcp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yftuvmom.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kogxfoce.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jfqgptoe.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3izxqqbqa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3tdotcjej.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qqotnsut.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gghqomcv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgmdlhdl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kojvgdrz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3efgngikg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3csgsymuk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3pkdaldsv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3retcjvei.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3vjpvykpg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tdvitmiy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkfynomg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ziwbielo.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkqsxdrd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfahrmmf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3yrisunsc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ikyrvghv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zaqqkxna.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3colmwowf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wmnzpyab.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3ruwvfpkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zeldjdxs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3oovlffzp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pyhpfcxf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kxganakh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3exgrqxja.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pumonowv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3pfoycoyr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ehjnblzk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3gqjmvpxd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qgtmjgqw.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bpkdltok.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3qszbqfst.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ffoxotob.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3xjshehxq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ogzgrfjy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pleipckt.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ekpqkxbt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3jibrwrrx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ykfrwzgk.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3peftaayj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xtervpqg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3axzrldhw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3xpevfabi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yiwqvmvg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3pxnqaubx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3awcntbel.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3udnarolj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3wodszfpf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mqrljdjp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3sqnhxylf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pcfoixhd.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3jbpehftp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3kcqxsywm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3shurveep.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jgwlnucv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkjouyjr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozttgodl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rawmpiql.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3knikspby.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gbrgedop.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ltbnlidv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dhugylxh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vpszgyww.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cioortzk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3afmurgji.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3aestvbxv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3baplawhe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3myecirer.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dqofqoob.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qslhkdea.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cfpoavjn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xcruoxpx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gjjtimnq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3hviambxq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ivxpjpkg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3iyscusqu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3osscvcic.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zlbqpoqy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dfxaiirj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pphjnamh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zghnxoya.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gzmqhmxr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3fqeoycxm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gkwnwdzh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qyyqfamo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wopfyscx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mytmjcds.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3enajrqug.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3prpzcdhe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3gvapajbm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3aazijbth.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ekceophn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dewerixi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zzgfwdjw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xvjwclcz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xtozpisa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3tyrmqvuz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3kzguolzk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ewmpekcq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sgshjkhe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctoovyzh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mynozkly.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxcikre.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nkljjriv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3idntevgk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3iwvqkcwa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vjgsjdmk.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cdaaixnq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ryndcdyl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tbjwryvk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3smvdsccp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vlhzvzoy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qxwxfthz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3aqqhelwq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ayvpcmhs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3uqjqcbht.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3nyezxije.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3utmevlda.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ihegsxno.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3etjirvkx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hgxqnlsz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3unoxpfml.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3uctluvkv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ynxolaqq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3vpzwjorv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3nfwmctws.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zkionsnq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3lombdbmi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lxloefjw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rydafbdb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lvjsouvg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3nretkscw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fhlwgoch.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3fjydpbfw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onkhjbjm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3amyaqeyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uywfnmhb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oomfasle.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3jgbitcdh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3sqxiytex.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ezreaoqj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3noonrpln.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kysagnty.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3woniucxi.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fzosrkbr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3niddqtgq.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vmkwlrhm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3msffijbq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3djlwtbgj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xlutrhln.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fovrdrkl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3vmpetyxb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mglkucqz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zervvzbq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rgdamlbw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrjjfodq.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ayyhenrb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mpzzgcqn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ximrgath.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eckoynyt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jzuserle.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3twxnhxkx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pyaaahid.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wscinwft.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3flhokvvs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3atjafrzi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wnyrvwlb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vbggucsm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3alpcfyoj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ldfwzocv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rodlviyl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fxbjvwtb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ikcxyqwm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vztoukol.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cqtfzeuf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3jvevkbio.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bxcfmhaj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3fdpsxfjw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3unhtcevh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mrbnwslx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vyrddwpc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gqckakib.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ruuhbzhd.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xhwvkqpk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3fshwnfpt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3salqrcbt.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3oymiirzl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3egoleyjh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sweaemso.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3btfgupdv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nracsylb.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hcikbirv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3egymnuxa.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3rlqnuaia.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sxvgwtdq.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qduarohf.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dmhdtqxp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3bosyjbre.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pzslxxku.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tcusjwrv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ogduzmcv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3vgvlqtbf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3tzxmrnsw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mzbkbgsr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gwhxpewq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dwfygryb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3dibrhlif.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3olmaswuc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sujfhuzt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fhawxinw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lbobitot.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkztgmgx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3qltibpqo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3mfylhljo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3gqpcwhhl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ukyqvepr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tynhtecs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3moygrodc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jbtkqhem.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jntacouv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3iqigsggb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pktqrcmg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3imoeklxa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pigtpydo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xwcrlxlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ayrluqru.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cxrfnayx.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3peewpoxh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ghajqmax.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekisctqj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3aayoaeme.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3eexrhcui.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3njmbpgdp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwkxpim.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gmmcmsqo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rhxesrfm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rkcrzkco.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bmoeypkz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pgvvfovb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3lmlgwunv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3juomdvmx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ycvtxdmg.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rkoyijhq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ioxoqayu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3uzjotqhq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3xkqxfsnu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uqclqwph.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsasynz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3chuqksjc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzeofgnm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rwdbdwwa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3oyvcputb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbdyspxi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rveasyzi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zrfeucea.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3eqwobkbp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tipdnuzs.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lkposzws.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3lywwrfvo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3znjqerfc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3cvidykhi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpqywsel.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3eatnynpv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vcgcfwsc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ptfcoauj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3porbywep.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ycbdyslb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uyfxoesk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3fbvwbzox.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3snetlorp.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tuawunyh.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3soeyzpih.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3livhncro.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oaywfkpv.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jyargsbm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qvafwvcd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3bxyjpbcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3crkmtnnu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hwegbmae.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eoedsqgr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3cxqtfoxs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3sqgpjqgn.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eqzqssel.html


<!-- 参考信息 -->