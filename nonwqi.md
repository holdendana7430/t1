代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkaujgti.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3myalfkqd.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3acskzoyw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujmgncui.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3elxnyuwn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3tzuuoyes.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipeyvoyd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnfiulno.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tvckzghz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3nvunmfjg.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oeefeyrd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3yivclepj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mrwdjuhu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uyptkhnw.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3wohtfzds.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pxzzytsl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3zxywjhej.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yasuyaas.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eisoekmj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3stjuogex.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ucekepvd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3swralxex.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3mvxtsofs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xncahdqq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3tqueipdl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvmieacd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bliuizzm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3nuuzgtaz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vdlclksi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iinwjkec.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvsgqdnq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ccylxnhr.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wcolxbbt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3camxcpke.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rgkeoavq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3cfdmwyjd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3dxavezag.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3rnrcgmgd.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3iqiaxxny.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ljpsrvsz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3oelbgzvr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3xvhlqezc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3tsqqfbnf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wreqvbdi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yvmegzlm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3lgiwktnc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ypvkjmyl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ycdvqlnp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3gfpmmcas.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3qywysekk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3itreyvci.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3giovtxuv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ngkxjwpk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3isfijxoo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ritefnta.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fnajlrfi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkcjbkr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ddabkkvg.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kjqaejuz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jfhswnwy.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3itxdeiyl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3itvufvta.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wejpbhwr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3elcedvxn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3hljifnpt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yruwhier.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pebinlnf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ndciutth.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkxxvex.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqvzpkco.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3izbhcoew.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3zgezeopm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3rhyftryq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ovoullqc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nvvdhyhl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3wbhzqqrw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jxmrjrkz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3bbvdhfme.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mhfuvfyp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wivffqda.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xmpovhol.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gcgxujjd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3eubhfulr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vnpezugq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3beohotqx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zuavghmk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wiewbqqy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3latpegdh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3sluaqihu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mcnwpjgg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3bepiyyfo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3fhzunpwo.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3jrdishlg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3eabsaxdt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pxivsvhh.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3gdtgxrfp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3irtdbpxt.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xyfhaodi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gnmucgvz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3wbwuimas.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3giwcenpn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hxgarklp.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3terpxnou.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gsnmxokb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3xuxxpqzt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gvkiaqqo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ikekxkzc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtichqyq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tdttkqyd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3itudckzq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dkhmypgx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lmduixom.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwsbzrix.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3mrxnanvp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wavahjvk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tqoftnar.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pudzriqq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3uvlitigg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3joylwrsa.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3isbjfuge.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3dgypdkcq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3lrnybcmb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cfkzmuxt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xxprtuop.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrbtylqi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvlixaro.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3euozxmnd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3aewgbtyv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3qxfsznqs.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3knkwnjzy.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fhodzsqp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3slkkxpzh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nlremzcz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3tuvhebyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3etzgpsmo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3fsmzqqfr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3elfffktw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dpegkzqw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3zuaspanc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cwcztssq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3csfqihan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufyjampk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ksfcnjul.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3oncjcdzp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xfslyyzi.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bukkbmzd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hoecvrpq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3odaylrra.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3sfhgupte.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3kmrvoezd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pdwajwpw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3uucfmvix.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iqesqoro.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3suekasai.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3adkqtzfc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3swotphsy.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdkegaet.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3gewvaepy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlcmfsg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3nhlnbdvr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3axfccugb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3phrljqaz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3vepavzfv.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3nhiqwjgx.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3luzfpeno.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sovifvfx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dsxqeijt.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qsypwtmq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lhnpzakx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3zdmcuxmg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3odnyuisj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3wdxkejni.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zgrxwrzp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmufafyf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bzqstmme.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qerinsjj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3fsctnbss.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ctmiygfo.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vnaalwyq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wzlpfdjh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rptwsotr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bivoqcoo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vqjwiuxx.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jxfhtehz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3shtvrdsi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3akfpdsgb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bgybmstm.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3iiffusht.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ecvvjfrq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pypmyxco.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kypgodkd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ylflrkts.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3rioiumqb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iitexrvk.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gkrbtipy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qypumted.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nifbeecm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3ogjtknjr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3osumiasx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3idgzoozw.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3oyptxkxa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uxdomktf.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3mtrleiwd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3xdkbrsnr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hcxqytyv.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3tmbsxbdr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3cgjaypep.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ngpenwpi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gqebfqva.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3pyjstscw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gauinbka.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3gzxaeyom.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ghcwuqxo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tnwkpjwr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3vniabbzk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3tblxokmw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkzhswdm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3hmgvlrfk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fmgthmzt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3wcimnzfy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dceynayr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hudjztxs.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3bnsqvyuy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fthpujmv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3pnccvoxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ijxjuwfz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hsrjmcmd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3syvovrrl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3bxojvjio.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3wufjlzti.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3onzkuugy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3uofirgjh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3xrreyynd.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3ozpgmamb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hbefifvp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3jwbirjgw.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ewowreir.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bxpnkgue.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3thmnmabj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3vrvhhjgd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3rjdidzur.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jwyzpgiu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dqbhhapy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ejublxhq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3scxujolf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mxovxoit.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3seobskul.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctziarbo.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zkszcbda.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3msvyvuvx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3lpkkatjp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tzeiphwt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hugqxwuf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3xkijeoox.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3zdswbfcj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uudpdqoy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vhcnnhfw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3extdybdt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kyvhwjfi.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qposevaw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cqnopyho.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tuofhmgn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3azimlgkb.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3chgoirnb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pplkplci.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3dhuorjis.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dnsjwnfg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iuczfymt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3vtiqdjwn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3kwksjktq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pwcceqih.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3omxigyxa.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tyutfyhk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bxevgras.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3oruydkwn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3fmxqqtjc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3tbouhcqd.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3avncvnxn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pjhlylct.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eliqxgwp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3eozylpqr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkzmltkp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3dqcjshcu.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vkrfagyw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ssgupmhf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3pjcvkbiq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3roytsqix.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tocyfekp.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jrrmaraw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mimeczaw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nkflrwzz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ijkkqsdc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3cgdwfiem.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3snnegzok.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3awcodpyk.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3bipxossn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3quouxujr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3pinkhoam.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3eknaajlg.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3kvtmnied.html


<!-- 参考信息 -->