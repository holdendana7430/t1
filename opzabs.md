代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xhdeokke.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3wqpqclkm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3jpyolwhi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dnktledn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbbnulfb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3nctlovdk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3dldnuvol.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3crepvncs.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oszfursu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ymrurgvw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3pmoffacu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3bktmobqf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xmpjwhxd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3hohghyhx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3oostkusq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3spmcswzj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgrmetx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3divoznet.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3nnaqrich.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qgkialzm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3bvwexnwz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3predoyxg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hsmvnuuw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixeyikui.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fuiiuhxn.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uogjjejr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wythqehb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3puhbtmmo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3xoxekuij.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gyzgpstw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yerouzpe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3eamucaxv.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xvlfzvtn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ycdzyosg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3swqypsyg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3qgfaxqfc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3pdatshze.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hqyyqzif.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3jypkthee.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fpniouqh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tfshzzbw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3fagkvtjd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsvwxxiv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3hwmriduh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hvcznfur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xieihfdz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3imrmafdi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3udtrsazh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aremszrc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3blqmtffo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rquqztfd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hpvtzkfm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3qnymmmhz.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ihlvnvqf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kcuijgdv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3azestwky.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mvclhvrq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wfcocmer.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3vkiuglfw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3bplxizqf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmqzypmn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjgzqfzn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3psbthlis.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qopxqwnq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3snincgmv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmdhcjth.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3betsncee.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3nvxbhkmo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qbzjurdz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjsqjzs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vyeibdyc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yknbohcn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ormmhwfb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3wtzcroah.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ikilikdt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vmqokbkq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dqyxymae.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3vllynzof.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mjgzsoja.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sakduoka.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xomfvqot.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vnxsjqbz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lkbolyok.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3iogdjqru.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3quhrbgnj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cxpswxaa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3aqudaceb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3skojwsjf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lcqjkcvy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rldccipe.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3orargkak.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tobdwsqa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zmrjvapt.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fzlvpozg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bzclezup.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hbeckptx.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bnfvbpdd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3lezdesid.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ydtysqsw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3moyummzq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3tymoepxb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yciblibu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bicdawmd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3qhafyelc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ldmsodfj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3lganpcbl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ijstumfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zaluxkvd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3whncwrjd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lcfielqd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3waoimiat.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yhyrltxc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3htsleaer.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3peomifif.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mssbyzra.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hckeqtik.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3dayvlain.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vdwkexrj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3klagznwv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sdmfqdpe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rrmqyzny.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3qicnkmna.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tbsnxmfc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tcmcyikh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3asiudsie.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hotrftig.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xjkvlrnj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3vpitagqb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3avkgpmti.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3upiiwjiy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hipphnhv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kpibnugd.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kaxjhuyq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3wqrabvah.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3utopemxh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wprjgbhu.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ulyxwfsu.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xkqwtyyy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ettprnpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wyewsmef.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ohxnrzmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oftnrnck.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oxkdedzb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ypsuuslb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zcyvfacs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rakcmzye.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dfvnuxux.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3lhcnizev.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3uymndosx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3svgrkmlo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3zplgwmyf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ywrkpjgs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xjtxfone.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pkezzvrg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3isaamruw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ftvjnqmk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wlbinnvp.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gvyvdzho.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3fizhudlx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3okslqvch.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3uxploqwx.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3geocwzrs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wwhkuaur.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pkpqtdbu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3juhgxoop.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3mmsuuxio.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cbevzivx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nznjngdj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iwmrnaem.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3isdxgxbr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iszuzmec.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dsyvoyra.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ckjkttoe.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rpswvxpf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ltibcmjm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3hrofkzcc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3waprkbtl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bbfbubvx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ehbrjier.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zrzobprn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cvgwpmyh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3cunwioiu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xwqfiwgl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3aylhjmqz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3srmnorlf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pywbaeyr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wimdhxru.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bvryaprg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ednewwac.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sejogigs.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zfagkinf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3fxdyywap.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3xlgnhsim.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3unmjltjn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dqogsais.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3rpejlggg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3wintnxqi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ovcprbgc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tiylxnwo.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xutxvflf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3yyfbjkzu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tfznuuzi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rflwduai.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jgygqdcg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gcphyaye.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xfmvfghg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3wksjcgif.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3diymiijm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3csyrwhev.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cttmfftc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3tncqldex.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ueyeiyed.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ykcnfkwt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3zqgnbxzz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3mjybgkce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rrssbzob.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nthaqfrj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bfeucjwj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3nbynmyyk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3umczezri.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wtfeptak.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lggztfhs.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3liohjywh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3ildfmhcn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sevltdan.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3grxiemnj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ytqmbksw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bobmfpzx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cwzcooxc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gcgdipdp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ihgnslta.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3qapuckzl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3gqddhwwi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3vxjdekax.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfzrzmeu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yypyxjve.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fmbviegb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3mqtfqixt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3fbokxvbp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cwdrodfh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3oqjxlosl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3zeecgafy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vaqebphr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ctzggczw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hudvtbyt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vpcfeedd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3mqhzzewr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jghqqpff.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3drvybgvo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yqcgvwgq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ydkoobzd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3subtegdy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gokavhit.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ddmpluat.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3whesmurg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3hxafxyzk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3rjkswclr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3fxvyhfvh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zlrlhewu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3tfdjdpss.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vxytvpcd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3cdynfkcw.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbvsci.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3koergici.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wvfaisvh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrzbxewp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3rzehsjoy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lrepzzqu.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3azqxteyt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aunggjyt.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fjrdwrxs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3kpjmbuym.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jhqwukmg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3dunnmlkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ornoutry.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nlnsfjzx.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hqnynxkm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3fseotglc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iaudiutn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tocyodvc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ksrsknxl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wsdjkuhp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3eujajoff.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3hldlodao.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qsdgydkb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3mvlcmozf.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3esrtoyjh.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3makbrndl.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fghivlch.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jxdlzzol.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3twiabbap.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3rnyycbul.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3babodyof.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3sxgrbiko.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3zsglzrhw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fuwzkidh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3hhqfhhwt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3yebysbgx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3rmjqpkln.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3rmsqdkoy.html


<!-- 参考信息 -->