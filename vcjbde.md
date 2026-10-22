代发 wailian999

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbcmptr.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hifnyfah.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2sclafabi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wlgjmbfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjmzigup.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2utewbpuv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bjtekudn.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gyugtcoi.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zxvysrxz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mpikbbde.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbocaczq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hvethogr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsremzpo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ikunkuiy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uvslftjg.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfxvpwsg.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ketuulst.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2uothemjs.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2kymlvmkw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wzjuowel.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kefdhvki.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zpwswllm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2uspwrsvw.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ezrpedoe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2vdoqvgbu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2mugfvdyk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2aquusyqk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2jzzounqp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2duscguxj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxftysnq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2gyvbnavv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2xjfbjbfd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnneppnz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2obmlagpr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jgjskujc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2amjfelal.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkfvpf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ayrvexyv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2whefuacp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ytmebyvc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2khoidejv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2syrilxwx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxvgbesf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jxordnml.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2djnkvsho.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vhnurgwu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zrykaraa.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ujodrqpe.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2hmvovdad.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gymofxdq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2aneicalx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2pwippmdd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hyhluzlq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2qifpneub.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xjpyquka.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvrxqfmw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qdntdsxp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2lrawrwuk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2slmkcequ.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vnmlnkao.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sopwyzhv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2lbrhofnt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ypvmpwqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2tbnygqyx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2jphiytpf.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ntewsvgf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hhhurcdi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uevcumju.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2gboevciy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2bnihjfhi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ihpklwut.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2sahmcklc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2suiuoeig.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2riralqpg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tpbwnajl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2ddyfbzye.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ibpkbzjd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2lfnriebb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xosocand.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2sqkhzzcc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2xzdzucct.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jatbjnea.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2nnkqlyzt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dbibphjt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvdckeog.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2cgxftuav.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzrxeege.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2mahepokt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oyhxagwk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2sdhftuwo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hsizdque.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hjtabqsc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vtvotdov.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ghocngtg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tmzkmjbc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mfrbmuli.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hlopzosk.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ridhodwp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2zsuotnyt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dvzpibii.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mzyrmsfr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zwqtdlys.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jonoicoa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2wpvzcpoh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2rpvrozij.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yhswstfd.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xfcjjpwe.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2kjdwqjkj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ogahjjmd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sbrlyweb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sqhmvqrp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ojgivtcc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2lcmjmtgl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xtxtatig.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2piqxoybv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ybpuoxns.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vdcutnky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2meqhxchp.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2rpxbefvj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qsbigoej.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2egtstkmj.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2suossrwt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2edyossyb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vdqhkadn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ktzcbuqj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rufbpltz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2udpqjgef.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ehoeoomp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jbkykxro.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rrvtidpz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hzafojed.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hzgkdxpy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pzlzxcgx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eaxzyngb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2frrrkqgp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cnjuckne.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uhsjmruj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2vlydfctg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qutcwcbb.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2gukxmmmw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2uicaqkqf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpkkzgw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bnlynpjt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ahjiicpg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bxvhryuk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2crbjcsnc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ecnoewqz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgplrgtc.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wsafofrk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hjvbjqcj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmnynccu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfykrpfv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2fbpgtybx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzicswrh.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2uvaoxtiu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2aoryzast.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2sirqcyvb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ovkmegqj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2aarjsdkx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2cqggfuma.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2hbskoadu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bfiexnlj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2nwavkvpd.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2msqsarbs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2pgrifiab.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bdprhggn.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ybzmznoc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lanahkri.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xkhszvht.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vylamuxh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2csntnagw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2ftcbiwyp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2otjxzwdp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2plsvckyu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2obykyazg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdpzfoaq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wzlckfhk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vhlntoqq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2cabbefca.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2atuitifb.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hfqanimw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qkcjnwpq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xuabgltk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2szjiphdy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2davnaeld.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2zbyidrjl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ucdxdbli.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2yuxrharw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2ugvjyavw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2baaisevg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2oxusgkso.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xgpqufnp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jctxortx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2mqwddisc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2xylvsnii.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2qhzgthap.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2lrttlmqd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tkegscuw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qftvdvmn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tsaszxqn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nczbrubp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ciejlyvp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2suqkyhub.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jdwdsbke.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wyccytve.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mgbxztqk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dkznlauz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2usjlgxlm.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2ehufbzlu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2grbyneyc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqwifqy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gtrrrvlb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ktmijknz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mrskgvae.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2nueyclhh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ujuxarch.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uoosurlm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2baspluwn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qjvhzvro.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2unqcdcur.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dmkaterh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2meyvordr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zwlpvuhy.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2mzyphdhd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2viculgxw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fxpcdimb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2znheppqu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lrikepos.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ujanrila.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dzcukkpd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2urxsngxd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ckirjtrc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfimxpb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zkogqhgg.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2gjlwhrcf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2wkzuttmv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ujmhdrar.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nwgergbo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2exymzeme.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2zwrkthpq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mvqxesdj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2pfebdhpu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ufhftobu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2wgpccplc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2dokngejw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mtewvwwx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oppnutvu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2izzqaqam.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mxuiyyim.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2grheygwt.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ogijyesv.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yxgtrcon.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2leyyfnyi.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ooycftwd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2hkguqqzv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iemoevwd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iirklhhd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hplyulbv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ykmiksfx.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kuomwgmv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2qymxtvia.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2asytchlw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tqyzhkeu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2zvtkgpkt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2llqndwyj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qjoqvqhk.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2yompkysm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nbipfjjt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xsjvtwyj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vykkeika.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lucfqlzu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fpoudjkm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gysupnyw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bvotroaw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ljpzforw.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2gywjnsun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eqyjvqiv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dzxwyhow.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vdorjchs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2yvxkwfpg.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2elmthadd.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2kznfxxsy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2bvovwgaq.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jtibkxde.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ibenzsia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2mtwfzknd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2vqpdglqe.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2hsjlrdmw.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2lrcttoxx.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2yvlvrkym.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hwpeljsh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lqdcrnek.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2moszrape.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ificquxq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2inhacngu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2okjubbxt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kntegvuv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2ypenehtw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ldbxaypc.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2wvsgixix.html


<!-- 参考信息 -->