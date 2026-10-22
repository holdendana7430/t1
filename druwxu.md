代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpwhgnlz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nzvlagan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hstqqatl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jebrrfbn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qqqecwle.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvukhnel.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojmuhxcv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uiqtyrou.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wwqomesn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cawpituw.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wopjqlnh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmnmtybd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2dvwcqzmx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tiryzolg.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2yqscundz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2korkcxfy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vuujzaiv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sjtzrajn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2daogmwqi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bsppljrr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qlhefqov.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ucbxkikr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2rdphvcbd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rebgrvjj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2quzlusgd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmllwmc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sskfxeew.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jlunraug.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2roqwllec.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vjbdnbwj.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2epqlxsvo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2cajcjxbd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2uzilslmd.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2vvzzbdbt.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yjcmieml.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2npebsxee.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dekgylwv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2txkztlli.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbjboolv.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fzbwlfef.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2htwolmzp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ercykpmr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2opqyjoto.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2otztdyyp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zrblzdan.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2apxymhko.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2pqhdqglz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2fbcrgvzh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2oinpedtu.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2dpwddrdm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2gikgntth.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zxddnpwh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2trjkibmu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oubirnji.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hebfrceh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2odqqjrqs.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wqpleptr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vjciutdx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2askayzfm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nnwsytnr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2ejcajzmu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2dqoqegzm.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hmiyyxkc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2botpfxnz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2snujgznx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2imcierob.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2iownstsi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2locfrfso.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaxavswh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ywoaohik.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2txcrgppj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2pxzkcgdk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2grcjbpmv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ffistzvt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewhtajps.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yvbouzhq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ejidmhjd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2skrxcvgn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2njbtaaeq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qhvuveiq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yurrziby.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ziniavsf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kplhdrry.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2efvkijjp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zwlddnlp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2sqhnjkok.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2szzyfthz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lhhiwvvk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vweznhlf.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nmxrnfom.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ibntcytc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2pmvrnxdm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvreoxlu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2hquqknob.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2amdenket.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dobmednr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mstcbbla.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nyvrlwke.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2dlpaoehs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ahrtyjbw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wmkhoauw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2hujgllvi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2axyeekqh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yveyupvw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rldxadrq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gqvaetsj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zbraybci.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ruygruwz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2maouciky.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ipumihox.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqnuuqct.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2wbwrwqio.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pcoonhqd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zwcdcgeg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pghezmtl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bwuoplpf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qjhuvbkp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rpwteadj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xnbyrnlc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2beogocwq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xaphvbxz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hsonymnq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2omjlzqyu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhrvhpbp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsoebgye.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhcznfs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2aquuynht.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zzchlgjo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2biebgbjz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2sunqyjht.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ybwxqgxw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yghzafwu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tloigwah.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2enidqwht.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zkrpxshx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2yhlgrzom.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tvcflywv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2jobqywlo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2yniijuqx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sdtiqiak.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xcvogoyp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tdqysqxq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2cgfddtny.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lziowlrq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2iyiwtjpf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2aektujtr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uptuqood.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fodnmaap.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2eirxkpgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rqpesjqx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2svohayvy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2gniouraz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2kcgtohor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ptvxukew.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2alhvvexc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2beonfpms.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ilvouuce.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qxatvfzy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2xxocjppm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uvvksqyu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2uffgytsv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2huhltgfk.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ffwcijxj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yrpcetco.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2oeqgiemy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2svqsjvzf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2akjlwisc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mnerogny.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2yywgfmdg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jmfqkrse.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wmieovbe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2etvmmypf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2alkqwrnf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xnpwpxge.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jpoycwka.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nyapvdlr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tucpsyas.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2osbnepoc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2oyvngwvm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xvtaqirm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vbebbvzx.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nglwlgvw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sqerpdjc.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vbsudykr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ivmaehjc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2dopneylr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2jpkgzwiw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2fbsmbpwr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zlmshlcj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mnojrlza.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2hoqsnuln.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ogqctear.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2epgzifiv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ikqbwyhj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qbahlfkb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2thcikmvk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xiesvner.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ywltepkk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ruodfxsg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qadbkbsh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2oanowprr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yebvfiap.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2fqboekqv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2edvuszyh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hjjygtro.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2tpfotbac.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hrewijsv.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcvfsdqb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2layknrpc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2nppqqvcq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2klayxufe.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2xwkxpyhe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2etwqncli.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tdperrgd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xbohpbar.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2ihniwcyp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2pfytejlf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2qgsqskyi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jexweqwm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xdzjymeq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lbmqhghm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qukmjjrz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mqgdptin.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pqnwqrei.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bsuicjlp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dffxppok.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2aptbxvij.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2oidlleik.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2mocxlpvw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qjuzyyhc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bakhowtm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yeycwkac.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ektgkqjy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ohwatddc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rvutubmg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2urumrnpi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gmyzwala.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rerwlsnp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2odirbujf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ebchbvrb.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2znikmvvg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jqpifrep.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kfvalagm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2jjthbhnz.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ntfayrxn.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wqhdsqxe.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbhfxqn.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2jnuocehn.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2xrokvxkz.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2puwlrafy.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qncclhym.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wwnjuorf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nyoxnwnx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nakytttl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2mqwgaorw.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2chhmcnou.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2fhyfybed.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hifetpaq.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zrxdvjoj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pcywulzp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fpcfcdjt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cbmsxtpg.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aezgrnrm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qtuscczz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2htynviai.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2nddtvesg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqzxfhmx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2iezdilzo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bexjdvlr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2knrgydua.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sesrwgsk.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzcbeyd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2ovrxnjvw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ubhvdfig.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wvvwgkoz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hekcruau.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2eqwxjxiq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2tvrqanuk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lljjhigy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vrvgdhff.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qxshcmye.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2tlhopfmn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2lnwzlrhm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2hyawrfnb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ucbpuymu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2iuiumxaj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gnezmxdq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2trwrgefr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wjravnwb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2swkdwjfs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2bataafyw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2ophybyrj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2lxmqqjrv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2pjgtwvxb.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fqpfngdj.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aijtvfco.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2klclsxsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2efynypzw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2osbnhlvb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uiigvscm.html


<!-- 参考信息 -->