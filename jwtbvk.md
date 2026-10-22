代发 wailian999

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2werewefw.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzqdwofl.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ttlnkwvd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cmrnsfbv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oxyjxvrc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2whzztrec.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vrgvoavl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2vdpunukp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2iiydbjli.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2hxmhjoba.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2moqauqtw.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wjoqsjhd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vhafdyyy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yfyuqlyx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qzmtvowi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2chjhijky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbjnkesx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bimmcrrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xokiyaaz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fxyfgomt.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2iolqlqfo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pubqpyuy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ydvhcxpj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ibgxgdoy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2urbdrhwk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2yfqvariv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bzbvxloj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fiokjnua.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cswfkzkz.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2awbhzcao.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqhvxvne.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yuhotssz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rdlciniy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2gesqfigi.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2yognxwjt.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ovdqsgvj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2cdxqdreb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qtiyyvxr.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ialkgjmh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2rujhmbvs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2heyqltxl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tguwfbvx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wyyplnwz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2oebihizt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ywiehwpt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rkoarmdj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ogjqiswh.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2cqhmuiez.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2odpfjmqe.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2furboyqe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2gadxuwdp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2olepferu.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2naanlnus.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2myprckcd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2eicnlehi.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2bajolmhz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mdfekwjd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2whuxanty.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2fnjmwuaj.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ifqrlfij.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2bynhwdfo.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nmamhwud.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jnatrgtn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ljidpbyy.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2xtfzohbe.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vcguisdk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2hnkumshe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rstbujgl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvuxjcaz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lxqdtlqa.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hbvmxlpt.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2yptcitqe.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xbbqhnpe.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2eynzjnec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2cprewvhq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2gplrldtt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ihpgwovf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zagffuye.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uefrxxyo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2rdiqrqpy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jmtnhrma.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2xfrpgknd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2jwyhrhew.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2yyuxnipc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2unxxgnly.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2viaxzlpp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cyvhnxkk.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2fqjwrrgg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2wbgxwraa.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gqwlekyi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohgvblog.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntdttwmn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbghnppt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhicoyzb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kpmsfwna.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hrcaylui.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tmxwkwsb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2txszdijq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lupubpgs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2nsswkckq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qiwbnudn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2majlrkce.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pfstjqqa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tumaljcd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2goheboyj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uyffsrls.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kqwkbcml.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2abmmhxpo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hpnhokha.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2jsltqfvl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zpvprosm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2buguughj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2tccsemwg.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2soizpuik.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2svydxhnn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xuzxnocl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2rdmnnwci.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2eujabhqk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ujbcrgzg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lvkdpuof.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jpdzqcby.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iwjvyctj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zatpndlv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2trnsdrwx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2dttgpzlu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ppxjvaeu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mawgfohx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2htxkbzmh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2dhlqksiv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlqiqmfp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2qwnlcpjf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgxefcmm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pdddsxcg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2bqsdbjxz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xjhomqie.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2myvunnnj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xxgzmtpr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pxqmdwfy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cfmzhidn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iqbbtima.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gumbaamo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuqhuhb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2bndajqbx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hhehtzmo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ishsvjpj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2inraepdw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2pmlcyzay.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vhawtjqt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2julpqxys.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2btymnztk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ykkfcivf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2muevhflb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2vfmvouip.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2halwxtzy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lxexauju.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lwstrgii.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mgaforvu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2woexxcyn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2xiznmpxe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhklzzhg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2sovxbelf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bghllzgu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqsewege.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjcnjusx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uymnecyk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjafocpr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2apwldoxn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kbblykne.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2palobtun.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fluiovtm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2lteehlzh.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2zwheeefe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2nomhdnwa.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2svqoxnkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2rxztydbs.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gioqaywf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ofdbwoyf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dhxkvbjz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2dcxvhcbt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vgcprenw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2vtmtywut.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2njqvtayh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fscwbfev.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tepjbdpw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2iisjcrwa.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2oundmlke.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mkxxliwu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2tpslrzwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hrfvktrq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rgmuwgbw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2irptrimo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnreaba.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tcupurfi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkoigred.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2unymgmgb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wwrvdieb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mvimeudy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2xmmnkqjy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2prnhjboq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2sixucfxr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvhsbpb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ocrghzsy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uqmxdhpj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xizmpwwf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2diibxeoh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mkxyigsg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2qdgwksmy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2eylbvjss.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2maisfipa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2thaujaly.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2nsxjjuqy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zdorjiur.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2chqhfdqn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wqkobirn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2onmkdyzr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dhixhsph.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2lizwckml.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dojhwtgv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2xxnhuejm.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2mrhbdkhr.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2apmobtvb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2onkcmwws.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nrecdthj.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2onconwue.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jxvkjvyd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2bjksudyr.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2akodmhug.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yqsddcvd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fitpnozt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2emseqqdz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2htzylkhl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2dcysscvu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vylvfclg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2tbptqfjy.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2awodwntl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pwetwdtc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewftmnae.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxlxoxjg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ymlljvax.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hjzxdhmn.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqggiblp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2ybgrvncn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ifegtfln.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vehdlwny.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gukkwkzo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vvquapiz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ajlebfhh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wgbzkcwq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2uodobpjy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2tvrnmijy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2jcubabtb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tshajpru.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ejmwyviv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2nwdkltyw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jrwwshbw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ryngpxgx.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2zzqpxahd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2olukvuit.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nvipujhf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rynlokbi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fhtamujc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tmjqtmsp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjhhzggf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2lvhamgsx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2qhsfuppm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mvhabyxp.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kooesbit.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lckwpdgg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zteyjyfe.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvtgmkjc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2cdiqdnss.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2geqhhqoj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2suvsbilc.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fgsitjbd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2gbecqzwo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2sjsxdlhy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2kcytesbi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fqabcnme.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tntmvutz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2ybogynwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2rswkbcut.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2jqnujmvx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2dhkyfant.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2yvnmboph.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2iqtadqpb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2idqlzrml.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2cgaysvpc.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ixgideys.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bgfdjtei.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ohjwjmcb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wmupvozn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rqxwbtow.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2jwufnwok.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zqedmpse.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2thihatdq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2arrtghib.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2xspxnmuz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2nrsfesry.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2bnmajcyj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2qzpxpvxz.html


<!-- 参考信息 -->