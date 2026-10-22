代发 wailian999

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2taoiuvnh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vincpced.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2jjldmaks.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dhdastqi.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cqpscroy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wuuyljrj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rcmsbycn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2orhmrjeb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tnydeubf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ahtahink.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2okwznhwu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dyjhmiac.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2oekalzoz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsquuuwr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aepweepm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vulewvpt.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2igrvlfjv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xyugypkc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2mabmxmua.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jadvbixh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qthfwluw.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zaigekaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fjvrgnbu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ljinicdw.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uxmanojk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vejdaemv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bruwwhzv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eijzsvcl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlliugb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tsfusysh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cldoxoqo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfsknyvw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hgseiqky.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dximwefz.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2furhafao.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uaxbqmmr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nvqjftbo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cucbnxqy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2afbjddkt.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2srsuugtu.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2yrscecav.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghkicjxu.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2nuydyajj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjuwejsv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2avyboyuf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2itcwiirr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ygvbzpqg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ncvakmlq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yganbwzl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2rosschrg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2jtftjakn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jomsslrk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2akuazure.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2svopvnhz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2pcrdaawm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cuzgxhsb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2iiwjxvpn.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmdxcmv.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rrrcbbot.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qmxvyrhr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eipqtvzo.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2opzdmmnq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aandjwbk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ndmdnful.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2iqlfhvco.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2fvyanuif.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2iuacdxek.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2waozpfwg.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uxlaswfd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2prvjljcv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2nswgkshv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yenrmnbr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2fnppmqwi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lyhnmhib.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2tyvbfxit.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2wcbdmybo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eojygyah.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2doprkati.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2sjardtnq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ewsmbxpc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2hikrrucl.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cmbxyobi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ucyqvops.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2naxwhlvx.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tkjssbcw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hfeumbee.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wodfkedq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2oibhpueu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ejatzdjv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mtkbydza.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rjbsqpmz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ewbagacc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cmrwjcea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2dykoexdq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xubeejso.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hcqbecja.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zhcnlrfb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lksybqlu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ytywvmbb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2euvetffs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2loebmfum.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xyxvtdsa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2tpoucshx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2bkhckliq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dzfxkvbv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2gptstioy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2eubwoaoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iijpxjun.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hkbtdzsj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wokohtcf.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dhcteuep.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2gauzfkdp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nqedosjs.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yiwdhsxb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pdyxajqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wgucdpli.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2dykkfqta.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2nzrxnhqf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2emofnnne.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hzdjekhs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rclvslip.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kkspzxcv.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oygpnwqo.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rofdygso.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2dvdacbko.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2jkgipzxc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vrjrhuav.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2cscnxxfc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2vsdlsehf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ybwkxnvg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2abmanuhy.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2omffmdmt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2gkpnxncb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dadfclmu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2edrcivff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlriygww.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjekinx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2addfkcyo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cseiguuz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2llahkoqo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pfdzygst.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2sxpqnacj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mrorfmhm.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hspwakjt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2skkempur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pibrkdkf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gwqqmwfl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rikooyld.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2sxgyzfgs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2thmppluw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cvkqcbti.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2etencgsj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2immzguao.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2yldarrww.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2svtxryxm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ubtsghwp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2hzgnjaxo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2uotppwaz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wzygsvuu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wrpsijrv.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2tewvxssg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ogcgfasy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vafveiqk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2coakydvm.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2poamotbx.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2eqfwmvkb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yivzgqew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2earzqenc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2egbstdci.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wldjdxas.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2aanfenda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ckikruvk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2aqxptyyc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ukxmzblc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xquwlfrm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2hpzxwjob.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dzmrrwci.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sebkrrzt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2eqjtywcw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xlzvimcx.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2dnsclqsh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2siifeshz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jozxvuki.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nzjghlbd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2famapalc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gltlxltd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ffkbezpp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbgqmgll.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xjmspbkv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2joacifgj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xmwbbqrh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2jrdybuzh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fzqhrdfw.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2luloyydh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2grytfujh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2lqzilzkn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zapjesqi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bkjwjcfw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2zfyhfcuk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fyaqzhir.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2rhgbaxsy.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kxotkqpi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tydiplyg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2rcwmbtru.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ozxbaisv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2dslneslg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tynnbpag.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mxlukrit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fyghowmm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwonxpt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2eiyrypmc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2pfaoiumq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vefydibn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lppioxhg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pcmtxlpv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2evprfiey.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2avxkdpow.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gdjopxer.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2psbdwlmi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bjbzfluz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2xirvwzoh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bgdoarul.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ftsfcwxh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2efpcnzko.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2wmehsyul.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2rnypdpel.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nnugzzqn.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2japyxont.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vawadhnx.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bfnndzop.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2xnkjdoba.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2emrqxrwi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yjhmpjib.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jfrpsnkx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekmfogjf.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2mteydajx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vamlnflf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2igmjmmby.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2msfcxhqd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2qgadnxpp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2rrzydrex.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hyflwrpn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2mwxolohe.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2teoovowk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqwfzwsq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2aeavcpwl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wxtzaagi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cpdlwuib.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ozlurnwv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2rnmuarnl.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ffapywhs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2xokocgwk.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2mzexwbkk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2cbmveufp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhhomil.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jmdthwsa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2chaitfbl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pzfeilrk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hoxherci.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rftjdqhr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hdsdqkwg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2xwzcrmra.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2glavwjbb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmzkig.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2yfjodvzh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2wnahyswu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xzbionxq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2budsvura.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hdvnbzfr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fqpkstwr.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lfkchydh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrswuxn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gdgtvmfo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ziunxmkz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2furkykng.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lvabcwrh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2txfopwoo.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ttqgafkh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2zinmysoe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dkqktpul.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2mlozgxsq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tmzqcicu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjarknu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nvhucsfr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bpwkioed.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2frvocrhw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2syllfdjc.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2ctbfwexy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vdrtynft.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2lcxesdhe.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2nbrwldym.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bkclgxjq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oftejkry.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ahgwqild.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ifhgnfwb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2egyitiid.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gvaoiqdm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2dzhzbrds.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bsbovzku.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qpisyqgu.html


<!-- 参考信息 -->