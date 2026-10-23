代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qquizlmv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3rxvgvvjx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wgokfpnc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vlgpzqql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dxqfxuuk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xvbvwycc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igvzunzb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rlmvujdt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvtklqbk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wrahxwhi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3niinyhgt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjglnijh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjhmjdih.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3wshrzhvg.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lnlqoizk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3udbzuzfs.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3jyjaxdpo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fkfekilj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3axfuwsfj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zoctkdun.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbpyqdee.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cvonbscp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oifabkjj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mwotldgw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3qdrbauml.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wyjvkysq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3dlugxkvv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mwatcaam.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvjldnve.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kcxrbxrm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iwfhbqck.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3abnxfsra.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqxjxoye.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3bggtyzks.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3cheashkx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3qvipoiaq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3nxobrssf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3cawzmmmw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xkpgzdfy.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3bokwnvnt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wdixhvil.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3nybhymkf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvxywuwj.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3vvwosemn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3scdngnnh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3izpoxjzw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3xkoqgxom.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qgtidvwc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ortamous.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwatfzhd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hupbivbs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3omhsihbj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3xitrfxqk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3zrqmvuol.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3udzykfdb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mmggwlsp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3pnifhfyz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xrgkdzaz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jgjapeoc.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3scthlgom.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3tjtciitb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jomwpapm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3fjujajsf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3tfycsddp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dzyyhhhe.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3yixlwaqk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nsqvxypd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3qnuvullr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3lvhcbhxx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lqyxatnj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3rigkobpb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xhtdmzho.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fdvwilyy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iykdibjt.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdbweygz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ukzburtb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3qoebbbuk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gaaninsz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxadnlyy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3pdxwzxpi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3owzbxysx.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qqkmwpxf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3osvjyojc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mxqombof.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bhqgcwfn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3corindby.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qymacsxu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3jkoczuiq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3shaigrar.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ikujgbls.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3etjhnzkb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3khaejvme.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wubnldpc.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fwveifdu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rgcqncoe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3klmvfxtr.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovarwvml.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zqymqatp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ftgefulb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fuqkxqki.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dblfpiql.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ooqrwlrr.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ihywysqx.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3noirpdxb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3uxhirtcl.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ompyylye.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3duislulb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ncntyppu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3eppzkxgx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3vplxphjt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sdstujph.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cfjrjnhv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hcllndrz.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yxtszjtu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jvicujjj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cczbwvve.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3urrcacst.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qevwuhis.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ojsayebr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcjciqdl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3skwbtvif.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vonpxksu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3audzyufj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rlousmns.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3yinbftzz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hojvvdtf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3onkhhckl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hwflipek.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lcwoyzqu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tjijqknq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zkdtpzjy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3awgybpln.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ymnpqvyv.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3dltxuzcp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3viuccani.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jfjizpdv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gnosjvmv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3anhrfgcy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3detsxxnb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3sexgmucr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wjbrimcl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gcxledup.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3caotalng.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3liaacyaw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qjduipko.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3joeujbqd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ojfrflef.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wuagdmjc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bmvadqhb.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qgibemyp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pflildxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmqahcjp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3zvkuiqlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aokmkfwo.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lmkqdmvs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rgtaltdw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ooofanfl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3egkartbh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3udnfxopx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qnvmgyrn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kyelcguw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rjpwaakb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3tegkhyai.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xnibwqmy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rlycidch.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bffzuyog.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ctwwwnui.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yuteezah.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jeeipsrv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rlgcovsa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mwtvrqhx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cwoousae.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kxeetohu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kzajkfke.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3dfmrkqhg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zrqxecaz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fskxczpr.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ynypkdfi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tdeoylup.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ltrskutk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3esswhojm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jjsdqfma.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3vfuqqjoo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3lpblysxf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3tyjdazdg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3kpvhlsdb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3voagiuwz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ncwobsxf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3voimbwfu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3viogndwe.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3cmkjmuul.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gxbeqowe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jynkchnc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hcnpvxbx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qvipemtk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qgxjjhyh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dcpzktgc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ypnqmsfg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dyhzxdoy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zhjjzwxn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydxnsqhl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3kevrviyc.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3botpuwbh.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zxxbbdsq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3umfxxxue.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxkdqlcs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tbleuwnk.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3xeyrbrxk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3ienbnshi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3iepkjklq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uxcerntx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmaqqdv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xrwrtuvm.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kvunfdzs.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mkpcipaj.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3otemwoho.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kmaqaxtq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwvzfsbc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3usbwxvlk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kdstyyse.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lwbwnsus.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hnmjbfab.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fzvfvhhr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jpcfnhjz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xybidxzp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qyqvehhq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wcaaagmz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tjfdkwcp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3byitxlph.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zpbfdinn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vcyqvmgi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aoghfwwk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gawjeupv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gmysnpky.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3yvmwyyvf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wdpgdony.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3shbncofx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3htbckzxd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fhczfvhz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mkwktvrd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3kwynewxv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3csgldjma.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbrvbxy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jyoqsmyv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3sedlwgzo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3adhfmmbr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yxaunout.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3etesaavm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mkhhthgq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3oarnlubd.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3lkecyedo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vcwzvaii.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3pqxfuixg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3uirqfitm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3rsduncbo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tkkepmjd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xzsvmfvy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrlxaeqj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xbiuexkn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3itfvkeoq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcktjovy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fdlvgzou.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3lwpgoqiz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3wicuiscj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3yzgxjbbg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fmwcfink.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xflcddjj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ejjxxmuf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tfiqhopx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ngxexevc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3noygmgbb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3iaqodlpl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3erzlkder.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3fhhahyie.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fxxkfmsv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3urotokix.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmhkumed.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3keptnosd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mlqeiqvq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgebrojg.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3esiugyqw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wcmdwfum.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xekqgvsk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3clbdpgch.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ngznncjt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3sppreyju.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3fcxraujr.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3qdmfexcv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3opqkwqon.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3hhqtwsub.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3stxiqemw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3huaqmbdw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jrdspdip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tvfyjdof.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tnjyezzu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tthdcani.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3tfwnpfco.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3xewytiye.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3zgbstgcc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qepubhwd.html


<!-- 参考信息 -->