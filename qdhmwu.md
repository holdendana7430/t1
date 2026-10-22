代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwurvafg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2pcwzeekz.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yguabuoi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ovqhqrni.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2avkwwydh.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2dwygfsrc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zbwvwcpo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ykrlnesr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mxuwwwer.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2upacxhtx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cyftygbs.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yhrobule.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yogpndkc.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gjjnmnfv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bmfdwhkk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2dqckbnbw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrfykyia.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lwxwrjyp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqxgwwxu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2ujwxphfq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mkzsjnln.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2fyblekol.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2fzoxjali.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2asovimhp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpqqjtgl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvqcclzm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jexkdphf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2stnlvgtd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfmyonyb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjzunzl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qykssbpm.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2itqkozla.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xqagonef.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zqdzelwb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ywypkdey.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2tgpaxgub.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qbsnarwv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2sdddvdcd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ymxpuomy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2meuvlwvb.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hwbhfijt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2bppvpauy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2jkhmbrnw.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbxyivc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2yrhziqai.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2fmgejydd.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lubynvem.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2okniilxk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xewiwdpr.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lajrhoop.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vmbdnmor.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bwylpoan.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2rtsmgxwi.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rgkofgpl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xtikiukh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jpevzwqs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rbkuxvbq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qrlgkhjk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2abvoqswc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2pdgwohqj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vryydzjh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2puuwzaiu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2aldjtjlz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kkffsfhw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2vugvvpsp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2iacbholc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2odhhbnuh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2yhwyrqhb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ekwywgwa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cqnlbsux.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mpukciaw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zwcuxkka.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccaiujgw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2umwptrlm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhornkqt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xbjqbgap.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mlkmfiyx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fkrrzhei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2qoypdxqx.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fogugnhq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zrutcnbo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pacmdpxe.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oazpalcd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nfhrxjph.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zuucwmik.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bctrnmhk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tcmktkok.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qhkngwbg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lspdjupi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2juatgazn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2tismnqtm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2cealodmx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2pqmftlyy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2kzqpuywr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qzwzihvc.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2iqvszqcy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ewwumkxd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2aujrszfv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uitgeaww.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2jyvqnxkn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dxnbtaup.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2qhwmpgpc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnsqlkhk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2sovjpkkh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2deljhqhr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ekachjxz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zcuxffvu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dnvsskis.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipiuckfv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2fyjatset.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ipfywcul.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2awbkhjtl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2zcppftnl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2jshrkzbt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2truffktr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rstmxzwt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2anvrgoeu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcdlllbr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2rnglcgnp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wylmzzfd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2xvfbsxbs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojevguvc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2usnmvfey.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2teansrwp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2yawdhzgw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xavinank.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xofarmkf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bwysqijk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2djxcyfpd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vqoxgffz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2twwakkly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2utdtyjgb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2srpmynwz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qcrekvuu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iypemsll.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2htujokcp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2tlrmaamq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2fnxwsthm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2olgibplb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdwonkjg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ljbrsblw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ceuvqnmx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2imzknulr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2arexhhuv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2aevmfesd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2smcryrbk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pudhrgja.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xfyshqmz.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ttbeiuou.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2mtzqhcwp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2gsgeqjej.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2klmtquhk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nbrnjqjb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qdfezqyx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ncxbmzyu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lamnjkvx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ykgqtdyl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2rbkoeyjz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hzfaovxp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fozezmsh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2byurilgv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qbbrlarm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2sbntmrci.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2clqfhkkt.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vjsukuir.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dtoucwub.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2iqphxqqp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kmkhkveu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2voflgnzb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2zedyftdc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rakqmegj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2leghzzsh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yklzaapk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oteqfyfp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bqocfcja.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2ivtlbdzr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qcqgxjdd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2wwebdmar.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2lzhmonov.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tnvpjgwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2hrnhvdvg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pzdlouqf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cvwadrhc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2mamlorlp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tsdulogq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nljlfwci.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2sbnsaomw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bubhddrk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2aupewwkb.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lerffrqo.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2cqjesxkg.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2jehzbenb.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2vxbhqqqk.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrfgkwk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2teftvmkn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2wzlhplby.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2aaghqmmy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gzpnbtlw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xjnnytcb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jlntjwiz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fsepcdvg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gesbfplg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2pfinjllm.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ssdiqcna.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ocqzmtuo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2ahslbzyk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lotspvfh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2enswtsri.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qidblosg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bjzrnses.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gbceprcg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2utkrnepq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jksjrdpz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eiylnaqm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ieqxvpwq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rxzgxfbr.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2clsomgfx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dillykuk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2jbdvlvtt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2wsngrkfp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxzjzkci.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zhftomjg.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2elwidmvg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2qzlwocns.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xqqurfyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2axpmoubx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gucomzqa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhmczuk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ubqbbbbe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2cbzkomcp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mvkmltmm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ekgiuviw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ddddhtjr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2qdicrkic.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yoybdqgw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mersmbqt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2exvlujcd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2zlmvpaad.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmhvihqs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gwnxlckd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2oleqjqux.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2urnoejrd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2bqtgswxt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2pzsgyqtg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yvzgvxne.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pakatuql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pwfuckjb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvigjon.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cxsutltl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2hryvxkmq.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2juppcchm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2pszyvidl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ynepowgi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zazhwany.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qgfrqwxy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2fiekyrul.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2aevxrxjv.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2wvrlocag.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xwldspmj.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2oklelxvj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gsepejtp.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oymccpnu.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2tlnhcznp.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2qvmfhipz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2qjwhdpvp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2lzmyxuno.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dcifsvvj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jasbapcm.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2qcohygie.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qsmgcnyp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2glqegqyn.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2eolzfnnl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2uqimmeli.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2omettiwj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2cvcknxgk.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2bdqnvsze.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2sdqjdusy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2qxnvtamu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lizhjova.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2bdqetqhf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2igurptlg.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ooxeyoal.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2ffzdsydv.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2vjnbgkwy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2wiiebksx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2vvpxiall.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2vzrrngyq.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cbgttwmn.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2txervwfw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbkaihb.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2dqhejqsm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lpzowwvy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ayznznoo.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2kxxjtymp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2izxeyvnr.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2hhkbwuej.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2goeyevpx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2badqekwj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2mmbzpepg.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2espvovgv.html


<!-- 参考信息 -->