代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qyxufzno.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sppfznxu.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tgwvuvuz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bgtsojpr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3zgnutiil.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3urphvyyo.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3sirbpxfe.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3csqamwmz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wypmhmll.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3beajtlnj.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3dvxxztvq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uudowbti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvzappuv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jcfdgkaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zovmrpus.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wuxvplis.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wjpjywet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjhpjjav.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehfajmdj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aoluamun.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xpopkfbo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wrgyrmba.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3danrtjnx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwtycdnl.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qzuwfrlf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3gxmhtegp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ligrwyna.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jlwitjtg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkpshdm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jiurnmst.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3kewfxgpa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bayrrevq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yjkqqmib.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mzultifl.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrcrxpy.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3etythwbz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jdtbbchx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3huvtzddf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ujrlnrbl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3fzqwynrt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3kligqqkv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3kmoxetbk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3bbxxvkor.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3leyjwziw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xavxklzg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzfsavqa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nbrwxlmj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vtuytufb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3jvjdmseo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3fxapllox.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ynrzrcxx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3mppwvjha.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3secyojhj.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3mnneylkn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3picqzqnb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jxzijopi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iobrscov.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rnkxboet.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3bfkzdzld.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3oyxzopsd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3rkdeczuk.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3nbrisvfs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ehoqqjcq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ymxlwgjz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3agqwllty.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hezgykkz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rwiunrls.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3lcdxffod.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kfvyyakq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3endwwwoz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3cohganxh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3phimfqpx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yapnncic.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3oalkrntx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3tmhuuhgm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3arbdusqq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3ntdmkcas.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3binteaok.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vvfzhmjt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3ymyjdyfo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3wqshocpi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mfkovlnn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3clkahysf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mdkifrhc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jtpcfbqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3kflxwgpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jbcehryo.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3iwystkqh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3spmfnreo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ndgatjhc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3myvzzlvb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ijuaontv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3nygxrpfi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3tcucaxej.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3soffmdrm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cprwbcaf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bdotbzdd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3hhpfkpja.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3swutchml.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3varfnlfc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dnemgdsb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bznygcrw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aarmajpd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xouhdbue.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btpoolpq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mxelzvvg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cvodpsgs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dfiwmsac.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3rwdgmdas.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkhlwe.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3rksxixeu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3hdrmdter.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3asdcdxyb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3gmhqvjyr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3venqjrdi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3uxikfese.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gokmphfw.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xmrmnttr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mhkdecqb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3xcrngcbx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3egicvwjz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3bymyskqn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xmtvrddp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3kouwgmvd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3sodsoozv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xvkcfjqr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nxcsaijz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rijhrrnf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqznpugc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3gemijniz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jswbkrmb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ujkcftcn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zwczlppt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hjtwtmri.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ctdlicff.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3daosfnkg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ywznaodp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zgsiyhrl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3lmvjghvk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cykxxqfs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3bdfmrguv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xfwwckfq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tmchcunj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ppwujhfv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cngfzcwx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3elzausoe.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3tdbcwpdo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3waggfnlq.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fifliybg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3fitjwane.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hifvduqc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cejedxdq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gcznhidf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nsjdkxqu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3alwvopqe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wgfrkncm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3jgwkqtcz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3nnlorfmn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pggzgseh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xeehxpst.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3qjzlzjcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkihgmkf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hflboqwx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3vucvgqhx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mlopvnbo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zgpusqxm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3usdlinaw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3oynthpdr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lxbecizv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3aascvila.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3cubgiayd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3shetlzhl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3sqhmlzvb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jetviwoz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lsqbaajy.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxqaqegw.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qiltrwic.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fjlmjqeg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tdtsjteb.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tbpkdwan.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3cozngfqm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3nurbrapi.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypkfmoor.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3pbpqeaup.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3epuvepxi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wecymbav.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3xmumzomj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3bhbvvqvr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lpgtojkh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ndhydflu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3aalmvlbi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3vvokirpp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3uoywbqwb.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ebjfrjqu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jnjqwtxf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3wffbwgja.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3rogzikph.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ffeadkwo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3axqujhdn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3eoexekcj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mfdoubof.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uzgosyel.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3nxfgtwib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3upkybxep.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ncrfoeti.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qluhzcxz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ierwmank.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cgorixiy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nuygqdal.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bsoclncs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3qcjiybxp.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjgowuor.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3dqrtykhx.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ujmpfxyd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3mwezwput.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gegfozaj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3msqgrdxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ryduvxcd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ogujsspr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3aitehotg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ztwqdfal.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yfmipyci.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3kzeneiyh.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3gtsfoudi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zejuanvi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3dkyfwcny.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jpkrpnqr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xruynvhs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qxoypcte.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zrjmsmzu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3myvbdrdy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zqypupck.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3spajtmut.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qccgdkgf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zleupzfj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mmivgvcu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xmzxvicm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3swbqmpmm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dgyaerst.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rswzouav.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xqskrtrl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3uuihahou.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3uhqfqvek.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3lnzsacyd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vldvrsnl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xtnfeejr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ecinpuqg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hcupvpql.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3sgufegnr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ruzknoev.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3mwgihfmf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ihhkpovv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3woltramr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dftejijn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zjyjgfgp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ywzxejod.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3gkfcjhtl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3tabuijvl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jivamylt.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3exzqavnt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3jxsezpce.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fsuujxpl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fphyctmk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dlecfpaq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gtpknbaq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3klmmfckr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ebdjzkox.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktcntwnz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtdoluz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3pcchwngn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3nkjurljr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3mhrbbfzw.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zfwczujl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pvvpytku.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sxgevefx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgwlpdpc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ucnbyyvq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ktplvjyi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xnpiuhfd.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ilcvbmyp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3iaixpscw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jpjowzny.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3hwjjbexo.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eqdzgbeb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3weccjqjh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xudfanbr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hjxonelu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvnerkgc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kbezkxlu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dttmbmiy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wtgtzsyt.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kgqfwtig.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jzljzucn.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmalbe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3sqqyibkj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbafse.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvefsjib.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3auzmzzfs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlyooxps.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cqmruqba.html


<!-- 参考信息 -->