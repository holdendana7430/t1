代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yhldnqgy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gpkaueie.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dxxxdxgy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cdjkxhrz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzyrxhi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2giclokhj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2kotwgwzm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qnzkkzkr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2kypwoepv.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fcrzussd.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gzolocfy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yxuzuwzo.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mbpmhvjk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tcidbpdv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zpblsiyl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2oadjwrmc.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2xcixcqjx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2dllekskv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2klfpeobv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2encvddno.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2miseepsz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2smpqrcan.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2qzpluoso.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bgfdooor.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckrdesgv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pelmakii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctrtqpbi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2lqwqwbei.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2odqcmchh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuswnbvj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjiiuke.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zzlvvgxt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uhyjcumy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2sqsrkohn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dphekvqv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2owworscq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cseludkp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2qblfenma.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2epnkhnqj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yiezlgym.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jwmcdlit.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2xiqovwaa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2cnrbbpeh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2dmwusklt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gqhhqjyx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2egqgnnub.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2fifmiros.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzbhryza.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2udqphcsj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zbudjgky.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2zqrcyxac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dwynonkn.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2hqemzpsf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2niakeveh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2utcnxdjt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yuljdqro.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2glfszglq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kpxcyvbq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ivehitva.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2takmvftz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wfyhxxuz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2unempwzn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2oohfszbk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zitiybpi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bcynilqr.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2brqjnmua.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ezzcqkms.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2spjpjrft.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lljibqga.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eappfred.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2tgyjwtad.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2uhuyzwfx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mwtzyxrp.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2gagmdtyr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2czrbbflr.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gosxovyt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oluqmqyt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zrrhpptr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2yqgzmhny.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2jnicxhlz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rzcjzzml.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pxwbkdyr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2fjehozod.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dkzvfbhs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2bldvpxac.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cokmrunb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2daugqqup.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2hgyuicxq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2pzjacuja.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2vgqqpavb.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qveomxbi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hvbnzxfh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmklrfjh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gwkqbcpw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bfowdfry.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rslazwkl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2jupplhep.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2puxujcas.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tahqbfdl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pprqfysh.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nxbdamhn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2kduatlsr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ybipdjye.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2acvecmmo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqrggzx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gqmpsrzc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsoifln.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2cizcuisa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cxzzpcpj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ouscggam.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mvmgjhzc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rtytlzst.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dcukcxrf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qjyjwvde.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2saytjrda.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2sozgnlnw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2skzfbtai.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2pmiurwkt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ssblbjaj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cgvwmvta.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2undaeohb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dkhvplyk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2zfxjpztv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vrqdpypm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2gthqkcbd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2irxvxhps.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2quusmwii.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2sklkxywd.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2euhpjbgr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2gynmbska.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mbwqduyh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ckevlrap.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2rbtdrvtw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2hstmozui.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2luxbocsu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bzxrudan.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2zpttnezi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqakqwzu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2zmlzkbyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vrcbynjn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2adsfryym.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2gyqpwsow.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jnjahdeb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2rpywtxua.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2lyjpxgwf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2saaegvsf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ujkszmuy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kapcmydg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mzcclkrl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2frfzescx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2nvdxiznr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bqitwwfl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vkppfzuu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bismhxaa.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gvkmqyzl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kqoaysbv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgufwgwz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bsqdjbek.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2quhbguax.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2oiickrsl.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wuvrpouc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ocmrnpcp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mthrviul.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2yqxwkorb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yxajijni.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2uawtupgj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2tzeopjbl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2nummxjep.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uiihapiy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2iobuhzbg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2mjoijksy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyowizgy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fyhmbhvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwxkyccz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jgnpgawd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jxvnqlnz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dajahhdj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hvsuuutm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fipqulqe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2lynkmhjx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mbmxwork.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yhgtlzla.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2mysqgqaf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2zlreshbh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2lsnfewoq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2abrwmmlq.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fanniixd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ivlpukxu.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2jsihwndx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2nxkmzolj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2yzwgzqpe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gsriqowt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fllzyuwm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2kvbxgxrv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2faddobao.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ctolbmet.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pdmbpkmn.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zpacbeez.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2yuotkies.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2btspsnfc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jnmmsrcc.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bdcywfbs.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2riwcrtip.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hjwxpcxd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ybbbfior.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kdfrgfca.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2psovlbkf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vxrkgyls.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2thpswlkk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gdkllwwu.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2uiuphfig.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rcyhapre.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2kgvkrkxb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ycpjkgri.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2mafcmrsn.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2iuhyxjtp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jvbfxjvb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lotjvnyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2dguerwiv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eodsmeky.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2booxfsyf.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wtdcaeit.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2glinscod.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2duwcwqnx.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ewduhqpn.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dpnyfaen.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2vluqnhgl.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2sshtnpgi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2zvcjlens.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2declemft.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qznnzjyg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hiilwwyl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fhghsysp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wmziljaw.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vtqghzdg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2uenhjzmw.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ricsroyp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2dbtavzft.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tochtgya.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2guqystmh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2boxscmqe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2euvldomo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ptfehpvz.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2fasfygra.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxtfekfw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdylgtyd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2qxxlsiec.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ypotfglk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lolvewoe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2lbfxmbnn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wtsotaje.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2sotvgeuj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbquudfz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vmaqvkbz.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2mbhmygpy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2hojrzlea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2hbfnvxhc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2sbdrzrii.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdbwuen.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zcogaimf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ljekuzdc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2eirggdyl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2aehbqylh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mynabfbe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dyqathay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2oukpqjog.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uyxhwrrc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2dutqjqds.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2mjcxcayb.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cosneufc.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ritawete.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hkjgkfmf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2wliawjzf.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2nvunvakd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2aekfcfqh.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cxdogikt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dxgmjged.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2oytbfdpd.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2rrkqzpxe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2escpbagv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uozzzcfq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2lacyrewc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2nwnsrxot.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2akiraejn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dibrhzkt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jdwbtjxu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qkddarpm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2rwbjvgwf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2otqufefr.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qoeqqsgm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qahdhblu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gszvyyol.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vsgdfdwc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmiivfej.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2weogsfnp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kdfbarhu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nynjjzkb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ieafprup.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zudqbize.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2axwearsd.html


<!-- 参考信息 -->