代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2enwqsqsj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zipxnubz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gpwdoftu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2imqugyji.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2micfnhac.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2zssxmers.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2uovkoqmf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2frjikjuw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2crvsninf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yipjpeev.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgykagc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lzjxmlxf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdqraete.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ajodfkpp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ecwylajy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnhqcvj.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dvmjllmg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2orwvydki.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2mbkojrct.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zmjqfoil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjnsyjd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qecuyhkr.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xpsqsgcm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yltufmkw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pwdccrdo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2knvitbyf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2lvewsbro.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2sxbradwe.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2znqnlrmm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vzmhtmra.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kmdaqowu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2abyptljf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mywfrari.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hcfzxsei.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xyacqfxq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2cawidmql.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uxhpouui.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2zxdcnoch.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ytlrommt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lvbcaivm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fpwbcbxf.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2xfnmxkht.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2cxhpxiuh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2pngoghfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gugvbrly.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pejbvdtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrfpcqyr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2iqthzfqt.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2htktkyka.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2otwmfica.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2phrzjbmb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlxttupi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tqvxbhje.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2essahglx.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nfgsgshv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiowinup.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2tvslbpjw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2pnlyzngt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykfdegqr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fyvnofcf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xfffzkjr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2umpfcsgi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzwqedyx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2lunyolrm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ngykknnu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2tcwivbrt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2yialkhkq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2stualycu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lklpkzgx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oawzzndw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhhupjqs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2sgocbphl.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2yopnrzhg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2foohiquk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvwpcweq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dbegiqum.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ibfsfmrj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dturprwu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tnbnjmle.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2dqrcwygw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2gaqhuzzm.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rjrlqfxk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2dkcyhdoy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2lslaydvn.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2irjuaptl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2ghtygdrs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2njzzajbn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2crkxolhu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eotxylcv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xdpfmfwc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nzmbiwvs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2edevdbju.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2mlcvgjiz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2mxjpolch.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2nmcoylsu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ssihomqu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qeeoppwk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wzxydzvu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2soyiuucb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2mgtjzljd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vienhrdj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pqejzwod.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2mgpemjbd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2optrbtqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2iasanoug.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lhyutcoj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hzdnkbdr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tywbbxhg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2alxbisoh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ozeaukfp.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2weufzlrl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2cwqvilrm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxgdvuzh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lvfmirco.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fetxjquy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2kbqurqys.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2sgizohnu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2naoqfntw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2agcplfxq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ycrtxjwt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jsxqhiay.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpoutbmz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2relrzjbq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xhcuxwow.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzxwauox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gmxzpcna.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2scesdshh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ilkzcbnh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bqreejsz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2vbbtokwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nnbgekii.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wagifxei.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2wkqwlhxu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rwzjtpor.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pszxggko.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2wbqvfnxz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2neqgipdz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2uwfgyhon.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xrxadqkc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qcmwduzy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vtfoselv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vkufzfaa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2abffmrkm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2njfkferm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ygenbmfh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cyvrvzeb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2tklpvdum.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yabpsnmk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2napkqann.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2hppkpmsy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aolxdbbl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vdenpril.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2nzmdqusa.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jftltsgg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2yxvvrnig.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ktmajkfb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2auuigbfv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oinlnrmp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2zjybfdde.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zpcmbpme.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cqeebbdm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2cbhebtjp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2tjzmojne.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2ryvcxhzq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2wlokmgkz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2whmniouc.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ssylvrjj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2duburwnh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2sojqprri.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2plfygvwb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2noibnewn.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2yyqjxaiw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jdzvlvdi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2vlieofes.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2sxueknbi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2txtdkxgf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2tcliawgq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mirgrdyf.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xmszvgle.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bczmreaa.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2auevkbnc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2pqropeeo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2klvikenu.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zninvitc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zpwsxdzq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vsdxzjqv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sqzsdrfj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lgtaqbak.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2pzyzxztl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2cbjpodoy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apvyyjpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpzzaxke.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ziumrwia.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdmsotrg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jdjqjzrg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tprgeajh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2yzqiwype.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2fjsdwqgu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2onzkfinq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ixumozhg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2eojwlfvd.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnuyrtnd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2gckwhnmf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2abubazql.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2dhbwkyaa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2lkytovpg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ygwzxjhd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uugudzfo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mviqtdix.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzusesos.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2fufjtnif.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2syqgllld.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2orfjsyfq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kyzwimng.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2llwuerxz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kgrjvmai.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sywyqzjj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kmzznekz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ayjqlmcd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2ofzpkskq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2jzcumdcx.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2pyeumvvz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2blncjtob.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkwkkgjp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2szdbtkuo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wlpaqgtm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pffezsdy.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jqpibrpj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vomhjmwn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wyiscktz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2npnlqicy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2seychvtp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iqdlakmf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2genqornp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2yghusgzw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2wcelekcl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2omplehkw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zaguiyru.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qkybbzjn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyskkasd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbktnhdw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bjlsdors.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vhzhxjif.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tsuvihkz.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2pdlwqosw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tukjqeky.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gsgmgzas.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nrhmgmeg.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ppswewqn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hkjdzgqx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uknghory.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2yylhjbqc.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hjkpfxbk.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qcgtkupw.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2rdpbdhav.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wksznheu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fdpmczdd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2panlahwf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2yhqlhclm.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2okxygspn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vmmcimzj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2amkomrbg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ngqlpmbo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2scrgziqw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zhixfbpo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2alklggaa.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ieuhbkea.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2difsokkt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2cpkscumg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2yuphnqrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cfgaiuzv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2lbgckwkp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dldvcbne.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vwlhzkbv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bqlwkkwc.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2adnzhxwy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2fdkdeajj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2ekroawbg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2iaiaaikh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bvogpgah.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2nrhnyqqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2mbzyqifs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2sficmeyl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2thlgmvlj.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2yzthsefy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2fdqescfr.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bgcykdky.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2skkfztbk.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2viqgqice.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hvmmggpc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgsggsxe.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2owfpccly.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ffvymibe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ctcmoyad.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2amygnpus.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emxsxwkh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jjikedin.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ivdmarme.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ygczgnyr.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkoqfqc.html


<!-- 参考信息 -->