代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uqhsdqzw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qxlfpbyv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2skmtdurr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2iuxbnduu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2fxrxlykg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2sunqfame.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wfwzdumr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mrpxxfne.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2fnqotxam.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkvvpukk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hvasygjz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2itoyfarm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsuaypvl.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ijjdefeq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2fghotrhc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2mgmdfljk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hlyzviqa.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bplmolee.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iuqhfldr.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ralykdny.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2okbvuxrw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wyekbjnx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2axhrudxb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2itswsqro.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2myhkwmnp.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ggmvgikc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2gpcrbdkx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2eoxlsglr.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2mjyirgzr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dlrcggzz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2sarnikyu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ehsokihb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jrugoegb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2izsvhiei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvjejmvn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2nuanfmnj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2vgopkivb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqtfxhxl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jpthulib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fvjtsuib.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ndlzsiil.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qkhnfthg.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2fvygweqq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhnvsgsa.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2fbldjvcq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jbgcpcur.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trifkohe.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhyanlgf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bnisekvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2cmkkwexk.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nwcfvllx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lcheinmz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2hxrrmppt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2zdbejmbx.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pevtmllk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2fzxmfmej.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cmwpwwtx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2jnvujybv.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vcuqrxdi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2tqvklqae.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2lefsvzyy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2lvvcserw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ketrwiym.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2pbogtaqh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pxcqxqdz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpigyykj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zobyqtnr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ucbhlzmp.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2rxvfluxk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qlmdhnkl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkzqcpql.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2makmsglq.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vkaiqjzr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wjfopplx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xuvipnuz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2thmdipnb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2nkeiiumj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2zkuouftn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2nqsukwmb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2talsbugg.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2tnxgyxkt.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hyhwrukm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2mdwvagnf.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2hjehupvx.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lzhyexlt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nnwljnpf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mtqvnfgz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2hgijyxoq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2szutxewc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2huejjgix.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bxrjwmch.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iukyqtxq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wxjjafyh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fslekkvt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ebwdggza.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vxrpohdp.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jnqtmwli.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2adptimff.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lmsnchwd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ogisjnxd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mtwdldwa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pkgqghzn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2umfwljla.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2vnclaohy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2gfklbvja.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jbvsdfli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nfnqktqj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kkmljtfa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ohxctumn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zlnwinsk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mrpkajti.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2pujvbhnh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2lqzatuzq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yzocrtpc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lkujwefe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2annvgnbk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ydkpskuh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2qeyyhdts.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2tzsbjbvu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eiacxyon.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2digflwmo.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fljevpcw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2zjzcczsy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jwksfzhh.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2gtvuwkia.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ctvmjufd.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2mkqmxmlo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yaadwanh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zblxrlej.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2bfgiozxp.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jyzgvyew.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lpraenzx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2psfatkwp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2lqcmyeep.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2oqdydaco.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vtxyzuke.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2thjqwukm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bkrpghsa.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cyzfcazp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2equgnhow.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2phmcomrt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pdyqpmnl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2eferkezb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2nxxspboc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lbfxdzlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzyjihkp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ybccvaqc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cmcoeytb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivqlaqxn.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hffipgvu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ziwyonyq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2jfdgbijg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2qufjvyqm.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2awstmsve.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2traaktew.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tjbnwlht.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rlpjkkcc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2twaaqpxw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kplqgauv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2icxfdxip.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jlujoydb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2orbjsgiy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2qstpxnmk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hafyscoz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jtffngrw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhgvqbtf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2alvekcdq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2nkgxvaak.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bktkxyiq.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2brojrmbv.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ghcsbchg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2tkuljtkh.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lvvwqqpe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gezpojzd.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zxngtswu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2odovfvap.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2ivsqdaew.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2pmujbqws.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oqztwitb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hvxyeozb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ngnyvomt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhkqnwvy.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nlhuiefg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2banugvpb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mxghbucd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2eyhcshvu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2neqntohr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gyexlnwh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2axwhkotv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rhdwmlnk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2zjqpidje.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qgzecxln.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2motivosa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2ubgdstuz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2izqikvuc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zuycgmqk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjwzucqy.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2koclypfs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2rjcsvecw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2hafkgrfs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2cmwetuqo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hpnvptoo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2tslxtvxk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2svwnbmsk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hommlhss.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fnlphfty.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xvoliyej.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mewnjdld.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2pfrovwcb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2shjgoqvb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eazywnra.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upihzofz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gfoqdwkc.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uuslmyaz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tivwztuk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2jtwpfsov.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2zspernav.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2wsjjytzk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mxyilmyn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2sbsrrfvi.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2idggmpdv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vbmfejmk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2phfxvqkl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2pffxhvld.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wxnmdgmt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uyhshbdf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2confqsuj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2awwozskp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2anfhoznn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pupzgjkd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2svmycmkz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wijrtair.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2unypxdar.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yxbyagrp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2vxfauvib.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2oqymzkdr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dpprnwjf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rxfwzqqt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dmdlmgdt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wsnihtic.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2oszaceiu.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2gvagbymh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2uewnwcqx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2ikfcfjhf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bxwaaknn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2eusgviqg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2skxfoaqo.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kwocpcuo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2gjmlnakt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2jvojadfb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2gasrspdw.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2awbikszc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtmvcnzv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xjcjzasq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xcntjqnx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2adtmiiwk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qqfmcrco.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2duelqcab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2bxrydpzd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2kxgtocij.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fkiekity.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2jhylfjwn.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2hcgtqycr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2bljbyvzp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2defcsnsf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ydlyoeta.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tpfyfnwf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zwqlkexf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qalppnxs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2aeslsrsa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2eszxuqtl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2srhuoekg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2swekgchu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2kckjprtb.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2zuvvxgxx.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vaizsqiu.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2iqpundzh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cygukaxf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2japwygyb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vongfnzm.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2lpkkjeqc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tnhefoml.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2qnjzrohh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grhxwkpe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2cdbakncg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dpilbaql.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pjczrkks.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2iqeuehzu.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zlbgbssl.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2iwennatw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2lvdjwzdb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2qovqkagt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vhzlevfs.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2koyzjigc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2okzowjlb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rbqaklte.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2qjpdhqch.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2dfkxxylc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bjabtmre.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2cmhohcfl.html


<!-- 参考信息 -->