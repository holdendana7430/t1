代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2cplsryom.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2brpxouti.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2arhaxfgv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2feqcnvpr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dmaxmrmv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mfykejkf.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2dqtogsbz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2glpkngtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hddzkxie.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2tdjyoppy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jqfungfb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iqksnops.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ihdwrfho.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bnheacff.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hizshaqa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqijfpmn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yavlxrza.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zckoeqwm.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpulluyo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eejxxyps.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2hbrlpygj.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2cpaoyxrl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrpvfybm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2elcraroy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fpqesdsn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2skbvcwdf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2luqgempa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ggwclzuj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fwbjylrb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bhmnxedh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2shoulzce.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xeuwtkqx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ipvwolkh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jynestyl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cvdbztdj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2vtvgpulp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2brhddtzg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xtsnwxfq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2chfteqiv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2vukzlxuw.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2pjssmmsl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcomlxga.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ijaavfva.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2exrfgbze.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2phuuyxrk.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfihcbu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2tscxnrxd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2rycplodg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2peyadsdx.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2znuifbjr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hsxrbfsv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jdvzwsia.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2fiuixkjg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qvardnqp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2afytfxep.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yqdunhtz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2yunozokg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2tkjemnmk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pabtgizb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nxoijuim.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jtnitifa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2yknmkkxr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2izqplqne.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xtfnopeh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gzsmphkf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cpbeszbs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jxhtixaa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zelihmpy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsfgayy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tauqaaoe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2chbrxedg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tasivlze.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tomgnjre.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nssusvxg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2dfwxmpmx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2omascyvm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fttfqxfa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hfgyvkyp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eqpwpxaf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2rvwanhjo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2cykabhlr.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2vznjkaze.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkuscqpj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pqsefmly.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhrqyzsg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bpddczmv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2craocvrg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fzgwowws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hpktfonu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yjccjime.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjcgkwzj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2znophfvu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lhllbkfz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2kywaoehn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2echtznar.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rageqavm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2evfqdibk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oqxoqhwy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xpgsvcaq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2vmoddgcf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2elfqsafz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2mcipfxgr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2wdvfmhmg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2gynkxbxt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cojqjgad.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2paqwarqs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2phbjwfqm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xrhqwazj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2whzysczm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2cnrfsane.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cnwsejre.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2skwrkdbe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2iobeldon.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jyksqhhz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ljcxucmp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2txktuprb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jmlozfcl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2pnbfobnn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2onodlbpr.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2qtfzvzww.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hkzvwohg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fsousdrc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2pztqsilz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2funppwxj.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yostbifa.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2phcvcimr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2viksmsjj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gxlaybdh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2jqiiwkih.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2znalhryy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2awnldfew.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2insycksi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxsrapyl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2lvhouaqz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ieresnjq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pnsowjde.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fozpqqvp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2prywgwfh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jdeqehxv.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kexfdgve.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gcqavrqd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulyumywl.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dzguwgam.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vzxnerwc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2inoguzik.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2seqjinvw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2wtrssgrc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2fwqflyiy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2anszxlik.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2znfiemzb.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rbyagpkt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2irlzmlta.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bhiakmlq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2kpvixxfu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sepsqicv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bqvphrly.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2fnogcwkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqolofdd.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2eqbkrabl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2caxywojx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xivjcvqe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jiyhptzh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2pvshffrl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2yjdyiyqr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hdutixyv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2gvmrvfcc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2aphqtpqp.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wisctfzh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2zcdjtqqs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iplhikzu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2svpkhfek.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hsjaxtnf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eqsoahiv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2uzvoeepx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2hmmkigpi.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fkdevgyd.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2gfdiwwtp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2jltgwoql.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxvoxdbp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zmyneals.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2feonpbdl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xnojnaoc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2prrnfnoj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgvfrels.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2movtfrsb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gthuqmae.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ajnejqqe.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tfdyplvw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ghzsmiun.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qldngcdc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nqaruqlq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ulgtqwht.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kedkezoh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fxdzrbfm.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2dirhzsgy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aefjuayf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ctxjydfe.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2iiosqbpw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2vdqyktvw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bwameezs.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rqutjcqw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2puhczugk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yarbmaoj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zoarpuzl.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ouaskphk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xlhoojch.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tbzhfmbw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wxbrhins.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2milgthnj.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehablwfc.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2awzxtyxh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ljcttrod.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tttvvjfm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kpxacfrl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yfdoxwuc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gwxvnavb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zatqamih.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wwgydfgh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2bkyjxmib.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ixjumwom.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2plxqreaa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2twiyisqu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dzzbtrik.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ekiyyabu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kdyssjmr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xtmvkpri.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2huidrcfu.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wivbzlxl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqakafea.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mhwawaib.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2aovhwgob.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sigtbfir.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2gafyceec.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2drqibffi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2zlpslukn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mabsjxle.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2paneirbj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2oaregxrd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2qzgufmic.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jsjiotel.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tupzcrnp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fncceeou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kmgwouao.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hlozlusf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qmtbcvls.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2phhvrqms.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ytkywfpn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2nlzgjqsq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2nshkwfis.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ycchbsbw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bajmwumi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fidsutxl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jeiaahbm.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zbkpjsnv.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uthlvdak.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hxyrpnaj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2gkfbqdor.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2dspopliu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2llhpijrw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itgxvekg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qprmcrtv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ocvjepcw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2qygemlui.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2maqdsdgd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2yjijnjtr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2ocmfepms.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2boldgycf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jytaonft.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eqymgfgo.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rjtnfapb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ymncxvro.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cpbxkeja.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xnjdfufm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cdbfcniw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2orhreveh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2gywavjhv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2bjwpedco.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ibhhvxtq.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brzeskog.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zvyueizq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cyfdrvuj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xqzsssvd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2dkfuzfwq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2bmokrpci.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vyfkcdtr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jbjseygs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ckyxfzdd.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2otpknxsp.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2tzvckmij.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2txcnrefm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2jzzyynam.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ajglegti.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2somrtgzv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rlhmjnee.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hhjmziyq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cbtdpgsc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2adlwdfxv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yugpeyon.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2figoabhp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tvjqvgdx.html


<!-- 参考信息 -->