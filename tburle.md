代发 wailian999

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3hlqhxfqd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bhzlclqa.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vluyvcvh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kewtwbid.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kbspaurf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nlmytzjj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3skopuyrn.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3azerylhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pveqtnsi.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3kihpbrsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sbmsquwr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3bdiljusg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zeskjwzk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xohyaoin.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnvgdoho.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tvibqmmn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ohooheyt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3hhdaimio.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ipcqialj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3vinaoxpy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ndwtnroo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3efartvnz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3zgarfykz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vdyxwscr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhcfnbzs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3vvzkbxxe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3nlkevasc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yrjbedkt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3eiuqyxnq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3awuhmlrs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xqecvucs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtlvjevg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mxqbtjkq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3hqipyvco.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3oijqafqy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rfgazbta.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3okweeyiq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gqqrotzu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3njyflofj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3vdgqfyqs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mqfycqcz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ntdwapho.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3auybmhbm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ehmfmlnr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qebmosuz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ejumjqhr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qckevnug.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3zfvkympy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3eivjiyem.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3yyaaywdm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3lbzqcrsy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3tzqujfgp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ajjxzlzb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pfrobapj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vvwqwuyt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3lannnbbe.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qnnagchi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3acoicmxu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3rjkljmdf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dddcpzla.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zjgpxspo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3drfnikfw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3xomauxcu.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3tbnmzglx.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3btwjzymg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3oolvyzvk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3inmcgxmu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sajhqtkv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dpyhxbwh.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3vztkhrgu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xreszsjo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3hmrakvdv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mllycioi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vylhymsr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3bmnavabg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wfiklypj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjwbdytj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zyymqqfz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3wopoddss.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gjpdzsku.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3madflpyq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqohctua.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgytgmtc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lwedeina.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xnxznygq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gzpgbaxj.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pxcjzlta.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3reyiutip.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3azshklzd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qqpchbxa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xczzefeb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nebuznwj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ccipvstg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3qqwhtmol.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zpulhsge.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ptnalrte.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lzdkmuqa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kuyqukhw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3cxnjyrom.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3owbmjqzx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nrkwdmkf.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ompcyocb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ymybpezr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kdzvhkrd.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ulpgksip.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3nfckwgwx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3tevkjyug.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rbxpupcr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3etaxckws.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3yokjcluf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rvskthgd.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vbsdwsrg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3aswjncao.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ozpjjahc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3adelgcnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tmvyufxf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3eerzjjns.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ywhsmivf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pkxqepjv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3vqnjeeyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qugziqhl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vqapmsxh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ofybafki.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3bylifjud.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utrivbuf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3yuxnixem.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kmdbilja.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ckbthgua.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3mkpjuime.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3knyeszip.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ezrhxoig.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xfaruhpz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xctaahyj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3znaxudnv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3wnkdpuiy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mpvdfhix.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3xnmmvznh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mmwiycta.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3kppfyjhh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3gdaxkndv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bgiyqxiz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3mkqdjlcz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3buitpvdh.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ehvicuor.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jmyowibc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tbqpzhhf.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qfthflre.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ilabohqu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3duvabxjl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3uwmybvad.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kxgxnujy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3splvnmgc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qpyrijpy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mziganrp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qsajzwek.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amprfkmf.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qaokxqrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3envypmmy.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fugkqgmc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3nqfjeylj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bvpmleuc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ovpmlpgz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tiuxhhcu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rrnkantc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qrzsexez.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3zotmbxyt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3bhbnzpol.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ocoaedej.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vroesdae.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3zikmvdvz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqbmcopo.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sxaogdfy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fixsytgk.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mhbvigsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3aljetalb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lombwval.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3awuarvvf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aoehevvc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zlicrooe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3jnsueuch.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yegqnedi.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wpztprkf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3pjkwahaj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ualevrlf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ugjuysss.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jhymdjrg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mslflhjw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3noprdqwr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oirhvyei.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kuqmdluc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbepjgz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xqplcffb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdvzuen.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3uvsqkawj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ipzjpjwa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bwgqhmjg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fubudxao.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vadnwcai.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3weqylrqh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xfnkaqqk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3xbrcyryx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3trvjnzbt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ennwylag.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfqsogwe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axmmfebu.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnevablt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3hqirndkc.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3njgiuoul.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3yzicotwc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzukmlwg.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3qvlhsztn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dyumkwby.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3anqtobfc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rixemdow.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ueojxlzz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lmxbvmxm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hofuuncy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qjicsqwp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pwaucaha.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3owpmawvp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cqydbldo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bmbmacej.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjacqjn.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3axtikttt.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ttpiagdx.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jogxgomj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zawkvihf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fbvtnktt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oczeqrxa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lgxjgtjq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3bjgorqvp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3dkzwbwic.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xulkeglu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iqbwqhka.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3cemtbxva.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3agzidhks.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jtiuvlqe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3msfbtlwt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yimefnjl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jjkhphaj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3gohmmnsz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3sgzembfg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3dewpojfm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iwcdxhzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3izsgbsns.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zqvhobqq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3slcqoscw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pggcgcmh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dmjkplxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3chxkvjdw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3xwkyhjvo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wqnaifcd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fnttldwv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3jjvuncoz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zmgdhdhh.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3lvwqskex.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wrmwwoke.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3umdtzicf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3oxtuynce.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3okdrupny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gnfvjnzi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3dtyxqgln.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3bhhntzmm.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3zbabypiw.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3txveamos.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3tlrfymzj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ojxnjetj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3spzmpyrx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bbaxqcnj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wpwmcvmf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uuifjpju.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3yskkojjk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rudnibhx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3lojgxhne.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bvpyonwz.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3ffjcfmgo.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kklururk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kbpcjwos.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hpedyatc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eairsyap.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qhibwdch.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3duwfhbhi.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kdigqjtg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yexbcqaa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tyeicsxo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3wzimbucb.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3uqusobkd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3sotycrvi.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gufdjhnp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gwpgovus.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3uxflnuwg.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3kmglykqd.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jivgpcne.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ssbcyjvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tgjtmofz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vxfsbpxv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtffhqb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vmnluriu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uiqinsmb.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3brjejlqr.html


<!-- 参考信息 -->