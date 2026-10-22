代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uiemtmsr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2omhwtqev.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fqwzseec.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oeplgxtf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bmlhqhyw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2qocbpsva.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hqemscjn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hvosegfl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iznyfnqb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2zylskahz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2eaunmior.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2deqkplop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqskffxk.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rzomlysl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnezrdnt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nctjlssb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ypbfvttj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxluqmdy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2szzlntyd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fadaaewd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lvzrynxk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gtotimqe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzlwfgzm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jysfwdho.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2endktwkj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ktgyvkso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mkijpviq.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lyaxvraq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xzaldhkl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2sfrawaas.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnckehyq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2pgttuolo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2uyghykfx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uquifplq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xaqmecme.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2jjarjfhy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2eykmoeya.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2uxvxpjuk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2nhhjmnqf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2efacuwbn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2nhvniujz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zzistawd.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qdqwxrrg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qaihurct.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lydzawed.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xmzibazx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bgzobufg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2sctdzwwk.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2gepjfmdp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ozrqymzd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2avlaeuob.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ybotgaxc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zkhzhfus.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dytonask.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2aujxymdp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wrzvdygr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2gyxgtbdb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2dcqwfuhp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cxcqokbq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lvoovzoe.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2npdbksho.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2yqdzsjdq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2shotovcr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mpjathbx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2voovxkar.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gqpnevdy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2eoiyltky.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dfzdwavu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nfqgjzmi.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wjsnigfo.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2tqgvybng.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qbgbzopt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2oipgjbvt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fpfjkgqh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fmoqemvn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2ckejstmv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kucohdye.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gjrriwlo.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oulasvzb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ontigjcn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2zpkopeqn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2yykizpzd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2zoyxpxxa.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mkpwaava.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2rrwkichq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzocsoie.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2piejpfyb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2xlhuulyz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hvvjcoda.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qsquadzo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xfywihbi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2egkpmwqx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxaewkto.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xuijuosg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2epglptra.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2drvkdofi.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2geuvdxtk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xbovzswy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ycdpdwzm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fmiuxnyd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vujwmnux.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2fobhhoix.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eeblyhtz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2yvthhatf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mtspccwt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2apitkuuk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2voxfqioi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2juktwofg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gtgncsih.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2brbqzchv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2bkbnzjgh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oasmsumx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2nsplngwf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2iepshmww.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ikkmlgxb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2iaqmqftl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fhlrcfro.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rdzwopwj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wkslyqch.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2vvghmlxa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dwyorvka.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ryankrrz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mxkljdnu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gyqaqslg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zxwuwspp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxmuvjes.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2asrbaypg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tywnzvob.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffdjhzxd.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2feiwsvln.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xsuosgzf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2troxpjgz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nybhmylm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hmawqgzd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2uwjqmwgj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ziiieaiv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2glvlemce.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lkbgfqdc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gdswsrvq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ijnbkqcj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2siyxttol.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2gdfnlksn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2wcavdvzx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2pbpgshpf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fdciqypx.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2mhdutzrd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zhafddlg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jnusfffu.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2spxwgipf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xjnmvvjy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2twnuxmdq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hqqotodl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2tyuwhwqe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2cnkrtqnq.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2qjarbpuj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtjgogzk.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2zrgpzfdh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2rkagsrsl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nlpurzdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tslftebm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2bhtrnphu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpgwndke.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gseblyao.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2guvmqurv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tjggavos.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lpmzybkq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2kxpkisiw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2tkuagiup.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2nddclyyp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ihxqgwod.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dztsjdrm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2sqvfomxm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zkfjboyh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2cvmrpynb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2apacpdpd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dvargikm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wwygtwsk.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2lxgzoiko.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2euckugma.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rpqsxead.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2lqrmrrgt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ooplosrx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2udhyeyto.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2acsgmoyy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cntomwlj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2rbahahfw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xmkihfbd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ljciztls.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dxdudfvh.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2nygzovxa.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2aaywpmiv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nyuaufig.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2mopyfque.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uenutqok.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pczlcqvp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2faabwhpe.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2cttwjzqr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2xqxlcrgc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fnwosprz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2mxlhjwlo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iqiwiixc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pztrwxxg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2yiqnlhlp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cabzktku.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rdvxmmvl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zubyjpgt.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cjluinsm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2mhdcdxmz.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgmwyhgh.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vgrctadu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxlotewz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2frqnqszu.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2axpsvwbf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ulwssrcf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pohstruv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2losnjdlr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2blabsnus.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2amumrxxv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2gkrmbjtw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ccjyylqa.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2buluxizc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2snqejxzu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2ritlqicn.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wvuaesyc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oknkowol.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wmkclewj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2msbrqhvp.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nehtyevd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2solzqwhn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2foosbuqg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2iktwecus.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fiikhevn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2haqjulhy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qynycdbu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ogpjthws.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2epkdnqfc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lpbnvwqg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hsfkcrol.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ewljkkbz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2uzeyhbpz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qvnnfkqv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2yhjsembf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ymphwixs.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vzkqegcs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uagttqem.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgvudnd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2frowflgq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2xvxucrvj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2vornyqcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2eyzizutf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xivppnmv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xrdhyqff.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ohthacvc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2muhpyiij.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vtgxjprp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2wplntmph.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xerkopdj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2inudhhyn.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gcrpuqcp.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mhrparov.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qrpjhjjq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2vhwoowgg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ulwxqlmr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oisbbsun.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2vhcooshe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dsurhmrh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2gkvnwoue.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kgemqobd.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rbbuderi.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpxvgps.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2rinmbfac.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2bgtlgziu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cdqnfiod.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bbbooidi.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vafytbiu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qaniifww.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2fusiksqf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dxibxcgf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jemaxqow.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2clezwasv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zmvbtayx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yojapgzi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsgfenr.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2biitkwmy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vgtmqzvf.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2exevsdom.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2lcuodgsu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ctkzqdqo.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2kzzxzefr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lznecmhh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2hfvyuyiq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2vyzqkqfk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2rcwtcixw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2spzujrdh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2iapjjcar.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2fugbemih.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2bkngwznd.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tajipdqo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yvkigrza.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2erlgfcul.html


<!-- 参考信息 -->