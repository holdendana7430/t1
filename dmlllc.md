代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmogcryo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wwlusbwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2knztduhh.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mggqspdb.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2nmijuqdy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rjbtvmwc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yhvfnuqp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zkwhbxai.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jvsfcmxa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2llotndki.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xbtzbcbl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnicdd.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2sjhzadhg.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xfrytxbw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2npxxrszb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2asoqasnh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gciylalx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gervxpwx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhvhwg.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2bgmvhyib.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2inurugkz.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2eozzusur.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxicluz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2meuvzvij.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2llfdnjhl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2luutuboy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpjnbzna.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ekgftkai.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ibysoyre.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2kzbsuvvo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jpdyjfqv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2rlrmfiuj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2cnkleuut.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nlmklbds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2exmsbucz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2dgaltkmr.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2askhmssc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2semzzzpo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2otkdrhpx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ybdnwqhf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fvxhspqu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2pogemkvx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2firvqxcb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xmdufhua.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2rmgfpzpy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uicyxacx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2cfmpiqci.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2rwpusslp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2opayzhcb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yaabhcus.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ebsminls.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2doddjifr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2utzpmpdm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnwpqknl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2fohbsmqo.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2gxdhudyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxevbjya.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2kiyakmjw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ldgdsula.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhzsatdf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2arwealam.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2wljbowzy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2kkvvntmr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pjzaddwc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pbpqhjki.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2imxiwkac.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ohvwtqsi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zlabacuu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlvkcmij.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tqecfaor.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jdfoqscs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2urlvrqwy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2aktvcyqw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2pzuasyjc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pizqjrhp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2uxfbeesp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzkewuse.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwevuqaz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fwcaqsjm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zdwoggbn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2epaahngc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dkbjkzfv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prryfmbi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bufdszgy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvfwtv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2iwwfkpud.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2gtbpvkkw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pqevlhpn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yqayxnnw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tyvnzhzy.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hrzfeibd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2sdsbbstn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2bqswymwc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wsnsczia.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2sbyunxes.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fcuixwdd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2hlyskpiw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wjakdxnh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jcfuhxdf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2dqyfkhvg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ebzpgykp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jhgxrqfh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cxmldkis.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2bgeycwok.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2eucridxf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dtkognje.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wjnyubku.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fcfttiab.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ydigibvh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dmtzdute.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yipbjryp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rolinhqa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bxnzflnz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lsksaetg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ogifkngw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2krfzscnc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jolfyzll.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2llppvisa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gndmgnya.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2shnluuwd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wzlyfkrb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rqdtplhi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2sjtxukya.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2kvkmjkuo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ngrmayfd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nugkbuwo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nnfbhdjj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hflqzolc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jdytdnjs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2qsqpkfbe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bintopxd.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2yvmpfpyb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gvjrknnn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2zzcgqusl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fxkhwqtz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iybwnvjs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2avkrgqwo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2pkblwudm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lssmdkgj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2xtnzkcfc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nhmsqrjc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2mekrkuhk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2pgylcmmh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xppnegmz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2srddxqvk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cablaqvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2urtnbtnm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivjvfynr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2amzyrjic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqrqptzk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sjjgozjl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uexpeulf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2iqvaqqgu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2prgycvld.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mpvpfjou.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wgnhoprr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2gnoulnng.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2dxubwrlf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ltsblstc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wfjqptux.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rkwpflwn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tahtsphx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vrrelgra.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2wbvmxddb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iyqefaiz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ukkijhcf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hvqqnbsb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dnjooejr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2flwwhtjw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lwgkkiro.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2qsgeszjs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2bmkjihvk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iqdplphd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ehgechbe.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2wwhmbgna.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cwlmqvga.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jdiludxm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tnxrxoyn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ppqumtqd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqdkrqym.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2nnizjslw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gdwqgnwq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vzhlvzyz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqlpdnr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xkeiqxsh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cxyoowxc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2pqhkomcz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qeuyppdm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zufzbnee.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ooabkfup.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2dilypqyd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2saburejk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jadmlvbe.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tmvmnjup.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2azehkgmj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yuxeffxg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jdbiiwmv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2obaitkve.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2meyehzcm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2kijuubrc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2dstlgcfu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2giwkrszq.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vnjnsthg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oeeovfhy.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2bzykppik.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qofvbvww.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nocyvchl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bghadvyr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2tjwcsbbn.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bxrrnjrf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2imfcbsec.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2slpgsert.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2vqppkbef.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2cbziinsu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ixjnonvc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2movpgssn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2jphihjkg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2awysdkyr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsfyqqxv.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sqmtcoww.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2adxntwmc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhbwxzkv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2epqeruus.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vrxaloti.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eajmbeay.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ubvcvuhl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2elafrgwh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vtjcepez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yihjmpuu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pxxpgzjh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qfupvfuh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2mrxgplaz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2metqyxzu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2erajocnq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nkfhbscx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2udszrpsz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2qedfgphj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bxnwbkqg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xorsefcq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mxhjsvtl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jpudzmeo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2putqfltb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ebkapjau.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qphknwor.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uduiymic.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2herpmziw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2jmusxazn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vlieciug.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2bfyiduai.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ahuvxtkn.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hgbuantz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xyjwmfsf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vniveauw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2yaxmuura.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2wdmuthbz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ncwpposd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oxtsnmhn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2sgltjsvm.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fbbnovjl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2commtqbw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rgcyekrk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wbldiuxw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sdlzdlhr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wbsvopec.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jrjdnbwj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2htudlzmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2wbtwmxtr.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2uykgxhuu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2eaubszcu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wfoorpyw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2xtgtlsaw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jrtnjcza.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rjcxtxuz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2atdkngvr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2swpfiknh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2joalspyo.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pwrnyapr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2azmrtlgh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2zvuaqpke.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2wbgggzyu.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2oldfxact.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2iiihmikv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2zlyykkuk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2dcfhlwzg.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2uilrchwo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2iveseixi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfhlvqk.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xhxzgebv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2sdcfpxcm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mxoqksge.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2zazizyfn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2xcpeykxy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2ymzixwkm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fdzgxjso.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2agsxwcsn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2edljqxwl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ewzwfqrd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2vitvwetr.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2lugodmro.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uslpzbts.html


<!-- 参考信息 -->