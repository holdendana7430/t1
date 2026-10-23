代发 wailian999

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3wydqamtb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wddmpuwt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lrebvzcr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouwqiqxf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hvpxmwml.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3goemldvr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ionuiyaf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zktldzly.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gbpswjkp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3itnpazlt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yralwohj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hmujtlny.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3iibeipcp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3pvsuaonw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3bfvmpkdk.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zseiyobl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jvhbewtb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3eekidqaa.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dulibgkk.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rmwbyslz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyjlsviw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tcwgnuue.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3pdomsriw.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3vofzzjsc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3qmjsodma.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fkwnxtyt.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3flaljttd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3khepzueg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fmpumjvr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ewpmgcjb.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kzhoqvgu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3dojoimhy.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3oufdpabg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3reedgaib.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pubvfess.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3dwryljpt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jsobbkbh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3xjvldjmf.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3esueexdc.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3hspofxma.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3bpaxgnev.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rlznaueg.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qwaeuwfm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ozosdtgf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qoaudzgf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wxgdsncd.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3eydqjmrs.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3otqkczup.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3imqxplve.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fkuyngbp.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3mgkommpy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3icfwkehp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kxpvdnqj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3uzhduhoi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3aozbjsdl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vrhicqeq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3gtmugnlu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3pexaecwp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ocnsvqpy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ryknbgqp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3ebtkkfte.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3zqyctxfl.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hhklrhjk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3kvdkrvlw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3dfvweglg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qndotjvy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qphwltcx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lvaflxav.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wihqfoux.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vvchueya.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuznqtbe.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3hzyjsbxp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3htybsvsz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3sslndacv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3szilppzz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3hwfxmpwy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bmljjrdd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ermptxya.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovwjsxrl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xfawsrlh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3vymxveya.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3vrhhcjtg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wwvjdjsq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3daakvteh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bprqbjtd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ivmbujzv.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gvdvrauc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qfvzvxll.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hvjvrrwy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3qdpliuix.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3aanzpxza.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3hercmbqm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3byxhdgvc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3egzgsxdx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3asrmnwpa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3hploexvs.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ccjpdfrj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rjrpsenw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3wkdxufce.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ggxswrlw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnqrybzv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gtldhzpa.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dklgjijp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mrljzlmd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pyspfgne.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qchcgmyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3huopncis.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ckystytw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3twobryry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngggqffm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3edyweeiy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uusxjozg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvhukjff.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3maddobfn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3myrtzhvj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fnmjsljt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3uzryjpsx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bghsvwrr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mofwgwwl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ystalmha.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxanbavg.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uhcfjgyf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3wrtsranw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dzjzwvfy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nubwalii.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zwouvzoz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3yfmbkpmx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3oifabbkn.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3sxlcdtzj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eyyjnpwo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kgbelbso.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xxahbiqp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3tekncdxb.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3tkznwyxj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jnbrpoxo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ujkbqexr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qtgucljp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qyoosnlw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rrlbqozy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwujjtxx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pemghutl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jyfdtamq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3nmgosgxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lepulyed.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3apbivskd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zshfajmq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qhvbaxxc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3elduzipn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qzpogxxv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vjsbxdhz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sznxgnfu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nzvopdwf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3cxypscft.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bsfixprd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3hmiwuszf.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ffjrrsgk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3eozzfzix.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ahnpbpay.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3mdjplfdg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tpichvme.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hzsbwdrx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jpteuufp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3xgkzzsyd.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjmfedac.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fmvzumzn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3lxxwhvrl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3isxmuqjp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3mryrtkgm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jopqfhmt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jhymdstw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3sggalrfx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3effyyxwa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzwgkrg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3toaasakp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3imxliftg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jreoiezx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dtqdeuli.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzjbtko.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jthurwns.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fvvqxexl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3vyvdgvbp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ozqmhxmn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3xeznbewq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gmszfnsb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3drrpfhbg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3czirudma.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3inygltmj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3fczichqr.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3txrbatpt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3osbevvhg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3upjhaaax.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ifrfreid.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3blmrlzuk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrtilljq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ctcwdzbn.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kuichkhj.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zoichgoc.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ydebkmbv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fdvidpko.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3wpfjakab.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3hiqbuwll.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ekoawxor.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3somlcior.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vumghrrg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3etqafomd.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tbvskapx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3okapodgw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3opqjtuqi.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3humdtphv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3kfctveuw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3btjmqnxw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vssrddrd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3yvdhiejt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rghrkxqf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3eqndsopq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3fzzwqoil.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lzreqdoe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wikenovr.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3inylfzjp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3wpwxfoew.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjjjuasv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ntczhhhh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lybrqxck.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fjwherqj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rtvmugbg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ueodcfgt.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ifmatvkz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vohqcgbe.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vpafbunx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3yewefjkw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3gosamjhq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ankpnzvs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tawzkwmf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wvzsodbi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rsfuyxnv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3sufplbvh.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jouhmcay.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dyzyitdc.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3uzuyupvq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cwnjsoor.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hluiumal.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ycdlpcck.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzxodcka.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3wqzgtdkr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rowxlebj.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3gokwzcmz.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3cpjpmpjf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dtuaqmbv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwmnhol.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3bxbenuqh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3smojwbyz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hpjdckkd.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3peakkopu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3egcflswv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3tfaehhzk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hisylucc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3jodyufxj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ulwfjjho.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ekwoqxhr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3thjmliav.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uduaivsq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3vjuxmygl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dhriatxv.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3jktwzrnm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3fwqpxtzv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhcohmke.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpcsgpus.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gitokdce.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3edywzakw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wrbiyvgb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nydcxjwn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mtohwzmt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mydguowz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nyngzynl.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lysgbzdn.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gwonrqol.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3vkhacsyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3xjaszmmx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pavisitb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3bjoqggzg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wcpzcbng.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3gdplfhzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xdghovdc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jfuzfest.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3chezbzfi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ikgruqgm.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3rsltfvwz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3zrdusgzu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3efsymjkm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3wngiobep.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3slvafbeg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3mqnexkcx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyopxbx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3asixdxbe.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3yoacfhwl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pbtcjpup.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xijzteff.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3sdztyrou.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lesehrnm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3pwvoouth.html


<!-- 参考信息 -->