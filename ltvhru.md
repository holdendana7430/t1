代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2icviiwvf.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ffacschb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2lgscxwdf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2rkogilcv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzskaimn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2djudegmf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwwpuqco.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2typnlocc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2grucgrio.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hjfwugxp.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2fhlgewdx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2suvbdjwf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2uytzouex.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vahesbnn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wfrkqdrj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cijwrtpk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uqymrucy.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bqdpbqbd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfkocbid.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2kddwspzd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qusdwxio.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aefjcaps.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qrkzfpca.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2emnjhsls.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yfaxedzd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uahiyiig.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vvwryzvt.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfvkgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjmvmjne.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owjptzka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pwqetcte.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kmdtefgq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2mvelthnb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2wqowhwqt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iksufoxv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2itwigkid.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2shjjqmra.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wczdqsub.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nqzibxys.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xprehzhq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2vyclxpzx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2nwcqbmnx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2gdmhcsyg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2czixhsiz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjujlckq.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2awkxxrkl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2qqebajck.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2yhdyhvpa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2sxluoyah.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2daezmvno.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2mgmpumhh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jjavofxg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2talzyzur.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pwxdtdbt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bcmbilug.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2onlvykby.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2jbuaxibz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2phhoqzrc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pzmszhpy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2rbshgvcb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2andewqne.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fsmdojtj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hwjhnssq.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2zdvvtnsf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2podomugg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuzflal.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qfhagtqy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2bpamrrpf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hdonkbjh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2firdpikq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bepthqlf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wanwmimb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nknxreiu.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2gutfvxtd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2wclsskfg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ffkonsos.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2arjfjujx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2qgiritfv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xqgwqqhf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hrhihvwo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zlzjxnxf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bggphxcw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rkjxhmel.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbasfbv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zzvqgidb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2iqyahusu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wiyhbnny.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jlhmydra.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gmjblrua.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2vbmeyisq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2omxuchie.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ntzqkgmg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bcwrykvy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2dinidbyi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kdxdafub.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2gdhazobs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2arpoylsg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2btipvmxr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lvevtdka.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mylflaae.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2byzojznh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2oyirvgii.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pqaxtgkx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2nehhonve.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ebqcvgnl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ppyrntem.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kqvhcpbl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2rngeojfv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ghmveiqy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2quoguynw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mheoeytq.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2dnixmwor.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2anvsgzei.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2yhwpeffs.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2puexfoam.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2akgqjrav.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ezpioldo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2osbhiuxq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2impmtvmg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qhkeoizf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gfodukyn.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rnvklgua.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jobgfmhd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2szuanrso.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vknvlcnw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2movolhqc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nzihytuv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fdzeilrj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2flyllamt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2jvlfslzy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bwkyplkz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kqynhbsc.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2dudircev.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rcuggvge.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wmljrnpa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ozuymrir.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2xnwqforf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pqegdryi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2raqapkhl.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2tdbrbpjw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qmpdzzey.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2npwvhztp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qscynzoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpiezxop.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxnhxetm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hnebttck.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tluffpeb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2yhflqema.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2vaxrdsaz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2tuvhibwh.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ayeaiqae.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cfixcqbj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2irbsjqzl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xnvtzrtx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2najkxbzb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vogzymjd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dizmwjyw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2bbfspsey.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2hgrsuvev.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rvoatryi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwldzpkv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwjddpch.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wfwqcfaz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lincyvms.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2mzktvjvm.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2svdtxxod.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2jxfykjms.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gvvhzdwz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2owiwmhng.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2uocazvaq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jnwhzhuo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2chponfmi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2kwhcdwje.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2viwfsowx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jinvjwfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kbotengy.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ipsywexc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytesqvaw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lkcecubf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2lyikwozw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2clgrkxyn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ndvnhfed.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2biaatglt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tgoxnjdk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2idbzepgz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bikpthob.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wlqzpana.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pktkxkcj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2xsfgllee.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2suxrxpvw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjmoxkw.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2seppgvcj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2iapvgqpk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wadrvjji.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kkphlgbr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2yennivpy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2iaivirhk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bpgqayis.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2btapfgai.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2hoymgddz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uchadqfz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bzwyhzqq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2vzywdsht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2kwrqvywd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ijkvnrdf.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ujggvgxp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pkoamfjg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evflries.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2avvqgwih.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wtkvjynp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jdjrrzjv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kdrmbmma.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcbsvey.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2yvxzfccb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2darfqdav.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kdiaokxy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2whwvwrsw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iyioljjm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2esitgjgd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qyjobkxv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2cmtuepwi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2duxvucew.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2pcxknhpy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xrmtztce.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pspfcxbn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2hefnxynm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2pqxsjcsy.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2clkwwezl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ahcrsvqd.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cstycblf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2alvtdbiz.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xkljbrpc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2sgoomevf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gbjdinhw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hkxfawzb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2xwcuzxfg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dvgyftrs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2movcyeyc.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2fgfmdccn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nroveuzg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qtxqonnv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2zhyzsofl.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eofftqyb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rflydxqv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2rvtkogki.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2egjjhkau.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nqljfzcs.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2duanyope.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2dkdssmej.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2trkqgooh.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2tuebivwc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ihhklstb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mwplcccs.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ydkfmbdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gcjflqyg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qcjdjxeh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2asorxybs.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cceltxet.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2kvfpffvx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2fvktpcdv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xsatoaah.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lndpvzwk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2aimucsuy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jyphokio.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ttougfwu.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nnxqjrmv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2minaahro.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2susnfiwv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2nneeltcm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2isqohvgz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zgkewaop.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2skmaevzn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ulqkblse.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ypvhbelt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2makpjjqj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fceqnjoq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mkkfmups.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dpfuplvn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2nmgwjycn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sysvqqfx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrzknra.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rjccmfjs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ujjwrykz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dqlojlsh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2izjmjfrr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2yydjuzby.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2hngphjda.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lphrcggv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bcpkvnxq.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uudbvqkp.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2uhgpgcbn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2lbtevpcm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2mwmbnekx.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kpnzyxew.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pdchbyhm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2muzsbnqd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2xnslcyxd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kwijpfqf.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2inuxfvqx.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cirstbvw.html


<!-- 参考信息 -->