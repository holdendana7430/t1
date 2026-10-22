代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ewpfqjqs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2izobzyxd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kkjdgwbb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ennlrmlx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dgzxvawj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2acwqzccv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gksaypqc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfgpnnay.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dfabzeil.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2voarmeye.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtecjxst.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdpujvii.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvbijx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ckrrbfkb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2yynpkmhc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2utgmuklv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2umxvpctm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yfsllajt.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2eoqdygvv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvdwvxay.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsddxcsw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gcinsaok.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xoazgyua.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2wcbpddov.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2vsncrgxo.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cebvncmh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zksgochg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bvapuokh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2uazvewcc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cclapffv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xkalbvvj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qerxhtkq.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2lqaniimf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lnuxwgmq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dvpvacli.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zmjnvnnk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2muezottn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2ydaougfq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2mehtjqcr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2dphbvekx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nfzojhmu.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2pmwaszmu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qsgsnorr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qfpuquqt.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2giwdxfju.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qxrkpive.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2uynjrsfz.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hfrhdqnh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2etwduvur.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2giwemuju.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mxfoqugc.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2iobygajc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qmcxibig.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hffejzzq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2exyvgwhp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qdildrht.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qtenlzzj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gkahzjft.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wtsmndhi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2usqzvexi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2lbptsavr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2logdknuw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rtwxpwmy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2zocdzzpx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ocsxxnbh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2irnpqxah.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwaucvzj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2reqzrbwr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2omlzkxbr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uktpbmmw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qfkhfaff.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xkxvcxbm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwlbzyz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lzlfttjt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ujnfbpom.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2udurcmvr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cwyoflge.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2ddazdslt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfxbydon.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2pastbyhi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2voslfzwt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qkzemidc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mrkkruae.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xwahalzm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cuqbxnhd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2amcvwwxq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wcabfrjf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wdvlzqtx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lscykutr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bkowyktm.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iriwkgex.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cbxvlmiv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2prrjuytv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2drsuwpmg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2smvhqzoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zafwfwoq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2hqxtzsac.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2woohoajg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2jiarcbvn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xanrnzjv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mqzrptxz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hlvkfqnx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2dsvkjwnd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bikawhyo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2quodpgvq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ekhdrhvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yacwhsnv.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vilxjeqc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hdduqdub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ierphhiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ahdiqbyr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hmxcdkzk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqzjyiou.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jbwvxnbj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2ydjypaiq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2sykorlhs.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2euwvvwxd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mzbswqyu.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sqhjjjzi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ezpxbral.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ggkeorsc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qzolfrzi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2iktpfmso.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jjeqsgxp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2kzrevgut.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ebulyeyr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2uvjggjmn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nkzopwif.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywbjvwtw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwprqflz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gfzekjfd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ondoifbx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2xfytjcow.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pozqcqdi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mogphkoq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zenyhetz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tlluktbn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dacfothj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2nxtlobci.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bihvnkli.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2adaqvxjt.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kzgcwora.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gszmtykm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryvlbxvr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xbuigbhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqctunde.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uhxavhsd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pmwevroa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2isnrxyjw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nwdtjexz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uevngirj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pcebcinj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2aewtsxvw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2eqjpqvuy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2cihfcmiu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ambzpsxn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2eyxuqqjy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2tjoejeat.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2irmdfzql.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2yqwaakku.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2webyrxmd.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sgakeuhe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ccjroyvc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2plmfbyve.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2vdlsxaoa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2coijsubs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2pgyjjjen.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2nenlkhaf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lcayjepf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xnfuhbab.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2bdxqshkd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2obhgzqod.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pajsueic.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2zsxdyzsw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zbnlrrnk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofttouvd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2fbiecboz.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oiprpopm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pkbwajgd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wjamzvko.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rciyczpn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ikmtaudr.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zhqawmlu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sufwkmsr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jyfekhsg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uflnmbzy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2rmxfkrfo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2tmtklfat.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2odoboulz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2suckoiye.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zssuevga.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rvhhqdzj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2wayiauqg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ydktueri.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fkgjeijo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2eokyiksu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kwoiyvaw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ciqgmltv.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2dsfugced.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2aeyhnmdm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ejzdguml.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2qfikzpwf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pmirxqub.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ujuhdxpq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msofzobt.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hvishefb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2irqzhsms.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2snccyzir.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ospwbyri.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xivrhzed.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxzqzki.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2weokklla.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2vbdmhalu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rteickje.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqphfooc.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ltqkpetb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rxtjcxft.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2izehrraw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2gfekoxlh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2iqqykzpm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ffoktcal.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2cafcomxp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ivfpaont.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dwohbglp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xgjbhpfh.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gxzevbpm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2crbuaymv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2kmasuddn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2eexqcmhm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dshcjlvm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vekzwgvm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cjgbrpml.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2aptipsod.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2oyaupggh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vwddslqs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2etimebup.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2msdxgmqi.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oxfkfmzu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2scnylfek.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2uvmfhidq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ayzwbmaa.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxvfnhsj.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrvpbrde.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kakksnqn.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2iwskrolx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qpefkoew.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2wrjalcqe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2zyjugtqb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bdwicmng.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbeltmu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mflwjsjf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bsrvgpcu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ahgdkzno.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2qaylmctn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2kqooavan.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qhlhugef.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hpjcbpjb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cymslrct.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yjfqifgx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2pjsavbgs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2wvvqzaoj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dlfbywpf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hglqhskh.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2lwozmdfy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gxqkjbel.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rezushcc.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qodfqoua.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2swvsfcoo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2yrffummo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xlrfiofj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cpvxveqf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2oknuizmv.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2rhjphukd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rujwbkdu.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2dhzprskc.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2fwhwxvhp.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hqagbmci.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2apuuixvs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ijzobbps.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2oedvbmin.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lxfwatkz.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2bugxofut.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2eulgodqg.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ttfwlquf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dyflnmta.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2lgfrefcb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2wvhtkdie.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2qjacuvpx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2kfsbjscq.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ikngefue.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xldqxiqm.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnezqera.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2kvrvqyto.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2seclvayl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2pjzqeowp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dmpoxqhq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzmslsii.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2kxwjbjyo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2nwjqjpuz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2jtvyjrum.html


<!-- 参考信息 -->