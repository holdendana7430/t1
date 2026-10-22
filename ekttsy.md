代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qkqrinhb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2abfwcxlz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2stimbepu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2qmcfslly.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2sgutxlwr.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2afvnzyzy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ahtkuyrs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wuhmsjvq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2udonjtfq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pzcabjim.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ratglfgg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewbnlarn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bwpmjtzy.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ycdaftsx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2gcrnutue.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hcdhufkr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2jfrehvae.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tbxupqpq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2niobllou.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iehdirtp.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2skvdmefo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2inbalown.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kgtshhft.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ugcrmpnn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2kupzbhwx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2aewfwjhu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jkamfuqm.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hjftxxff.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fjnwdpky.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2quyrncoq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fcuwgwiq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jddhxacg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfydxwre.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rzdufgoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wfbpidtf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wmyudzva.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2reukjseu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nbzwpcfp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2icrudpet.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2udqhydab.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqoujyrx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2usodnspd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2vdhqzbkt.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xejulimz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2dqatarjy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ottcjvbm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjnyayoy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqmkhmno.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfregtlj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2piwvghjz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2slmrinbe.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ognhetny.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2fclebdps.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pibpggho.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2eelzagal.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2lhrcfjol.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ygrebixu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctcaxqgk.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2wscxvwxr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2jyecltnv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nopxmoxw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2olobzzzs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2atdncque.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2exmlymum.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lzvbpubw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2clqghsre.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2qyuskoef.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gytooqes.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2utptwgkm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgrdovhk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2hkvgskqi.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2kvbkcvww.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2avofruvr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2feueodhf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ofgdfpka.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ykzrolvw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xnzauvzs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfxgnjbl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cxbrkyli.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2kmcvqchm.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2mzzaciwe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2azrzihio.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2imbtbdgg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zzoqravf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2syggspvr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2febfyqxp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2npagjiuf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2uypojkoy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2mufkxrvw.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2obsrhnic.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jxykwkkd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2rscjnecx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2clrfdqvv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2tadsjsww.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lnikgyvl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2myvgledg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2qayckzsk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2qusbvsgy.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2syrmqsnm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2exvlezjh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kpritryf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2kacfiorh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mlwoohmp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2pmmpuvig.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2anrtuvjg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2iqmredxo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmnqkcu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vqcjhyzn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmikeqat.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cstffgqi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gowasmug.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zfjbcopv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hissjrwr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xsoebggd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuhihvx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wrvlvdmu.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2erbwliaf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2convnvim.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2rrveljlu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2pmumilbi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hnajykbx.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mycmzwyt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kmiuetpt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2tetfvomj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ncjyxarl.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wrutvpcj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2jmrfvnld.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2hhhireah.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mjidfxuw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2owymwsld.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2eeczwars.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oiyuzwlz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2xeswoiju.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2xovmzaqm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2dfzzngff.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2lfgamcoe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2tmfzsiwc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2cimlsktv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2tmcbkkwk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2gytfdhvv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2zusjevfq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fxtkronx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2rmjnzcto.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2uotzuxkz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vqxypgzz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2olxxsbbm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ejywzkfv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyaabdni.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lceibyip.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2vlwufcnj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2gtmvwroo.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gyfploaq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2mgpvnuok.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tvqyuznz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2shvigzrl.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cglbuzlz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2dwrobdkx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ibehibjd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2akgaqwhk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vaqtlhys.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2tkhxxstv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2xviaacrf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2rqhazbyl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2cwmxjian.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oydhkmvf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2cfewsrek.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oykchjyc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qhhvxphi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2qajthlqe.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2neocetjt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2giuhsfcf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2neshonlf.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bsbzpxun.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lpjdzdfy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zgbaagic.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdceijfp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2hbqgovup.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2muatknke.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wvnprvxu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hnlitvts.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2hbtngbhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nsudsjaa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qaywdfpe.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2twlukzze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bkzirdbt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ldgscnmu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2oqsiorvx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vgradoql.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yhcxjqgv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2phjixowp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2maswbqqo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2ltmkajvg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pvoaaqlm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2muylkkke.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sqjvfccq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2utkcbbwt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2midfcdps.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mlxxmrcb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2mmmeopwc.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2uljkrurw.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xouclpnx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wstofibv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wayoxmyk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fybakmit.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qsizsbys.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2srxbflrr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rfbeurqs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lrtnydie.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2csjvynxi.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2boqapptw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfgdeikv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2reaypgyj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2senpinkc.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2pfniutpr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vxuogllo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2gtgylhyl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2btpwqdpe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ymmnupzb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tibdybhz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gqgtxibu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2oqfxanmg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2newlkrrd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2epzhfbjo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2rswbarnj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xufmswuz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tcvaapgy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2riyntmcp.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kccfhsmy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kbaumhfh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2lpkepjue.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2zzybwijl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zwhvtosl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2inycjcej.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nnasptnl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qsckhuly.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ehqyjgko.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2euyyadzq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gazkoifu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2htjjhzmw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2etbgactm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2goadilqo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2puvbadao.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2cqvggjwz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lsoigkqg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2aczmsybk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2kmtlatfz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2xamtjbxl.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2xxhbtzzk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2esepfnnu.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hfhxmxow.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vijqtuva.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2gbfkdsvw.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2fkruebcs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2xyxftaxj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2scvrhwjw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lhugmmgg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ytmffzpz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2zablrnnq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2idmuhkwp.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2wzgctzlv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yrqxjcqa.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2veonfvxq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qjqiwuqg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2dysvevgn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2sweylsmy.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2iokavcwp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2wxdpesbd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfpdubi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jltfuoha.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2jkvovkbl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2duawswwx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2xqhynlhi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2qbcwcfnk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2njehbxfp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lswzggvj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2jvbkkpci.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ljvchnbh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zkcznixq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vubsjbfq.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aqlhnwpt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ultibvmd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2orfeisyq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2tqvgjput.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mxsgbued.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2jkgjfskw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2addewnzw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ppoonkzz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wodgnrsx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2frugkopj.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2gvxeqoao.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2ltlsxfko.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jgwdrpie.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2fgguaebk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2qxcmsscj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2nbxvmuhv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2exzsegrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2xddhxkxh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2esrwsmhu.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rfcklwny.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2fhubuigf.html


<!-- 参考信息 -->