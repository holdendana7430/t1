代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2dguubvku.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fpmmjdlv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2szzwlaqq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ipjhjyxw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ecfwpwmx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oaseozvn.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uenqowfc.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2fxkvvbxm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xvqqduhs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2vjnoqyvp.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2usjzljde.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ipnzrinn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2svcdbiwx.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rqxxblao.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2bsdsfafj.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pkidnesi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmwzklec.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2penspydb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klxlqvca.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mcumnkmi.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2tqmbrjmw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iesdeixs.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ebwfgcaf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcrtkhg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvbnvoiz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ufyhthut.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2vcwxwixx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nibrhhwh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yqwnydhm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wqofanhi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oynowudk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zjiopzba.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhooqtdr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2ohdotzyq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2jrzhpadn.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nmkhmwuw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2qxucbrwe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kaahsmsv.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lhrvvfyh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lafdttux.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2okkoxmyl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejhdgaul.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2loieirio.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dtbsiqbs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2cuzxptes.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ekirqysk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2awnhkfjq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2zluzzpfo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2twbyqkht.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xazjjhaz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2xwjyoqja.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tgpknlbu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvpavcit.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mhgtoowj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2bzilxiai.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xwfyojkq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2beygydcz.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nwgmzgzw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iqlnfrck.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2yunzpaef.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2hfzoldlu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2nwxzapjb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yavzihuk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2jbawxtgo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lsbsmenb.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2iijitnxs.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qdmvcnyd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gxslvwxq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2imcvbonq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wjyydloh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lnpuumdv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2genmineq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2patticjq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2coajuonb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2utxpulns.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sairyoyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2mmeeqtbr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2mvthwxcf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2inftmfwn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ukjvsizz.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jljouzvy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2eiuaxqdr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xkbkrvmj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2iclvtkgg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2budqrwvn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2blxwjnfv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwmzannk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mwcrcnfw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2srndyqdj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2cqjuciub.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2awqoyvdm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dqeesijg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nfmgwunb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zhihhszz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qtzjaskq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dyoelvkr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cplzhlgc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fgrysnzv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qikilnry.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2niobqogu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mvzbeqfr.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2xptefypd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2ezfsdhup.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2noqczult.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ubulfeos.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gxzfgwhb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbwmmxzs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ulgyzpjt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tjktphho.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2msklbajh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2qgxcwhjr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2roqxunri.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ddhtcfdi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2dgyjfhza.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vmpsfiuw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2eatagmae.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2kgfkoxfn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2utqztthz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pkjaaery.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tojjogfe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2qzgyiqpm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zsjpfzdu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2qpvnnmtz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2flvtmcuh.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jedvttke.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jzujqtwb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vrmmubab.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2aeptaxwn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tjwtlgmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbgbqzt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qmazrreo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xfweyefr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rvyssiku.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ifakmkjb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xidwntgp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ynfevfoq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lqhitygv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mkbkqdro.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ungepoeq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tjtqyten.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ttudxqwt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zwhfvtou.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2upwkcnxz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hqpcpjyr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2umyhrseo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kbunkqzy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gcobposw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2wozzqshs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxqsokhs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xlloydqm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bvroikrp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2wgbopvos.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2aesfnmvj.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vnyecrwz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2zdflnbie.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vvpfprmi.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qgswgfjz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ezvkegpy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgchknqc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2iyicduyf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cvbpcldz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2zjjqdiqb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yygwidxh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjbprung.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2esnjdzsc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chotwqzp.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gssxunpa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2plcxhzlx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2njnmhibq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ihwsgazd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nvjxhivb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2uujpugog.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2eyqecgba.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qodbbxyp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qnmuyqcg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fsqiufde.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yvstcfld.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cflwrokh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2weciqlcl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gnkjwnnn.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wmypagmf.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2dlndjfwa.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ghsjhjhg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hzvvzzgv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kzsxjmgy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rfsppygu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2biptuwmm.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lbakcgqc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ulxsemtl.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pyhfqolb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsjwtec.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2goelsykq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dbdbpprs.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rlllblgo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2srmpsxvl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2wfgjurlu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yhkxrksq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2nsymznfc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ucvomxwo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jnvnwvhf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxxmzjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dcwgokvt.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vsjblkaj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wudduljf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pivjbnxf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ogzeciik.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2alcfwomd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2gnomdhmn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zypakjbj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vvatrrvb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xebgdtqp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2tnikiqus.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kmdrmwgv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rgntwczy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kwugovux.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2pkxdcigk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2xlqiwppp.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxlbqlst.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2gcragzgm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2afwttlom.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2krbnafoe.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uwpcbcus.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2pafrdwru.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jtiozkpn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdvdxyyr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2guzcvccy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2raztvgml.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vzbwsqjz.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ieieeazc.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ppswalke.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2puttxmtw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dcuuyuyx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2qrxezznv.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2fqyedcrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ngazvehu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2avadzpjb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ftfwtoox.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aiygvyxs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rkpxyfsd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ikvfavnb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbdszzyw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2woasflrv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2owhreoqz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2oybxffrw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cgmksmem.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lufqwxnw.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2aublsotp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2shmcqoxm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xernjlko.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xiwioukk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hmjdzegu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2lbzqtoqd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2yzyspxgc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2imupytmj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2soqggaar.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2cxuatoda.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ngeihcuk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2euwnubvs.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2tqpsqyha.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wurenbtm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kyqgymhp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gnazketg.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juaszeza.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vmeiqqhl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ymywycyw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2tnoozdbn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2svzyjsxr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kpubuxcb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2wzutosho.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kdgddswr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2utqsljdx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpxigfyl.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2pblsjrdq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fdrnicga.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2iwaxfkyt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ujeztckc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fdevbbfr.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2abmfujyz.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xtnryizz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mjtdorwn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jkusyojz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kzomhzhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ycsjlwfm.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fxknbjow.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rpubxnkk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bmuarzzx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2jpuokwqq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2riztknjn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2vibrilgd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qnxvdqla.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yexpjmvv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2atqhgqik.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kphpoloa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dybyephl.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vsnrptki.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ygofvvzg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2fcffcveq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2zfidrcwe.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2itzqfsoc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2dtytmdlg.html


<!-- 参考信息 -->