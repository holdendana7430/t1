代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ymwopslf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gicnfqcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qynwhvam.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vonlqzvv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xuubyqhl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocrwspfc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xbzkmwcj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2acvgsovn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fdasydnk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2mgeilurb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhdfwkgb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2aohuznjr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vvqjzjie.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2sbomcwbf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vhonnnop.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bttowwcf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mbdkrbeg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2gfmnmuon.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qcgrmnek.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nqixrypd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pmuvoyri.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2srlrecyf.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dbgzycww.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhhzrs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2pfksnijl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2accwiivz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdewjdn.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2srgjhwbu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2myndalxw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lbpvqern.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fuirzgfu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2wcyijtjc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2cetxntft.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wmyygilb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nobppycl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2luydrhud.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qxqwqdcj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cebcughc.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2teknyfbj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2vohfhwut.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2figmuwve.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wkcevfrt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qpwassgy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2immgiypg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tekeihsz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2khfvsuen.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mzasundi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qdzsagck.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2awnmqlmi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2gqpamfmt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hldmgesk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kofifkfi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tdyezmjy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2djxmyiha.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hiugkgei.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xcfwebel.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nvdobome.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2eibmjham.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2iqjcrkgh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zswvoceb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vqccucyd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fpdizbqz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gqaqspno.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jogubdsm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2qoninpdo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zykaanbp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jqdzuczf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2txnudobo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2tunfoetx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zomxjnyt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2qrqhxohb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ibyzhauz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2emgujgot.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjeqbrrv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nudeudrh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zczattjg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qexqjquu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgtnwxa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2memxfwnw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkbzuc.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xmioymbx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2wsgsgdjr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luoillwe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qnacdgge.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2zyfbhdpx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ddejveja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2uhsrfwxn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pnetxkcg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ezvbvqdc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uptyhbar.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vwclanbo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2gapoxvtr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qlhftukb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xnuifkmg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2znbbeops.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2njlughpu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2wxqpdkcy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2zkmqcafx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2oprdpwse.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2witiyisv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2cxabhrfz.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ekgucbvg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2abfvufjz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2oaeimqef.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2obxklnht.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2pzbzuwii.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ycwenwny.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2aclydiaa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2eqilvqfz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mmxbqeyy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uliywuhm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2hoflfoly.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ploylvob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvalxlri.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ieplenhi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2emonkjfq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kcbnnxse.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2kewixcio.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2nfjzbjcg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2gssuuwng.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2eqjdlhby.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vazwagkq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oeskguzy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2odhbcwzh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceerdsok.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aldpaope.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2uvjvvigz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2frmkjbap.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2fncfmqvz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2raiptgmq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ttkwyeac.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2urdsiwyu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frghblej.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bgpyynxw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lyvcrghs.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lsqriktr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dwmwmrvx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2qxftvzeb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xnfommwx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2slfnenhi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lxyqwmnx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hnyfvkrl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sipqhanp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jcsudlxh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2luyypggp.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pbdsvxdu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvybfryr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpgsnwoa.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wqpzehgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2algmojeo.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2rzbhpxkf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mfnibiul.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zvvvmnqg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2earydgrv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2ssiwctiz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xrdzrtlh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2qgenybjm.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rjkuaqkl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gsqvvkrq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fyhohvgy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2smluvvhk.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xqqfplcg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2izktxifn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2egxoapki.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2esjxfixf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2xxwdfjyo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2khhcpmaq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qofniurh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cuxiuqwj.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lzxlqeds.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ijuethmk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ycdjivgh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pgivrcka.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fjkojahv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nxngohvf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ctkklotj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2iufkogmr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bbocbxjy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yiknpboy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzywtvvc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2pgwejcdf.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2pnkwjkul.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2fgtbsmoo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dnxumakm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rytlkmsl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wwqdcbft.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2agogsxkc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wtbhntnt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xohxcvxy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cmpotdnw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2qrbkdqpr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rmgpmgda.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hhnodkpa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cwdvhrmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2xcorjcge.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nwdtvqom.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmfezwdc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ohbasohn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2llcvrjfc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2skpxvsbl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pjjyflva.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2silcslzv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rcdecxiv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2pgxebnqi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2jswkyvkk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hmrhbijz.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zwrbtxuq.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bgacetrp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lkzsgora.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2svhkelxu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bptijkcj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cbfcmcxt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lztzosrj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2vvzddbsu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ccillkpq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fpjiuiga.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zngoxlgg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2evqxjeak.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2crbbpmgb.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2nrmkbmrg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zrsplrxd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdknmwby.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2vutzhvmy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lsufhrxu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lxwrhfdw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2etygbvdh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zuguhyya.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kplkxjni.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zmasjhuo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fblbrhnu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2kefdcjyo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2zxgdtpyx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbjhwvv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2aviitwwd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2eyrqlout.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2icpzkcka.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wnmbairt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2ffakmetb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2uhjvkomj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tjthegoq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2vzkcuqoy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2uvwfdqgz.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibyahded.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cickktvy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zvwplbda.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2nsvjpzsj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vowiphvu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jvnsqxya.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2crgrengx.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dkzyyauh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2mnhxeynm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2fauhxoul.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvnmrmc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2padoetqg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2crlkuwol.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vkhpstyh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2wrqhnxlz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2umgjsmon.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2mxsbhoho.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2unbbeled.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2pikoestm.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ikabehlj.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2exhojtzv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2gteidwkj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2cqtkmzrp.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xioibrus.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xzavaqav.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2admfrytt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rpqlsfzp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qozptrpl.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhlxzsrk.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qehhylvq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cjgbclin.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2jqurkbtq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2pjvctthe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2renvmchj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nsmobqxq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lrlvlrjc.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2wjjtggww.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2iplkjcbe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2kjenndbe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2tkxvpfcm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2uflqqstm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mgztccwr.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fpvgghzz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2rzuvtgxg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2riknhwdz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jdsoxzyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hxtjdmua.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqchttuz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2keibxnxx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2lelodjoj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2hncvljbx.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zshhhoie.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2llnkhyfh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgarow.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlkpeoqw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ueidqmbc.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ouaauuon.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bahuvivp.html


<!-- 参考信息 -->