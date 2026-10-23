代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vanwcjbp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3abuawxpz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3tqydpilf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3wisdexbu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ingsvyrv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ymxsugyb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bzargfwb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ykfhtgyi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cguymdab.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hqrjwroh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wisydcxm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjryajcv.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3onbuexzp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3bacqodqt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kudtvutg.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pfqclnrs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rwtenshq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3chfuojky.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rmsvyqde.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3imnynbdm.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cqggmhkh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uiiqlaif.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zcupgaxl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jlpdqryc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ldpjyeaq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vhgeukzi.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nonxfmvc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nucdcily.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpljsme.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hcvcxvvu.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3rmqgtgbr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wbuxpprs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaoqmqzc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vnbbmysz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ourgvnsg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ghjyohrl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3cpmkuzcd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3vhkfuqpw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zarbztfz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhznsqgv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3unpcxafr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mqvjlawe.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ctjngzad.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaormsga.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3guotafcz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wczzuhlq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mkkaaxjo.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwgychkr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tvqvffnw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3fuwztywr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fjxvvyya.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3xkhsgccw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3isjgauqx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ndndkqbn.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ffxpgqbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nhmvocsk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnpmaokh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nitfzvpt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3auvdcsgk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bquvfmbg.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3nnmsjfyu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3vcrymhhh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3ghjilxof.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3eyrhqbub.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3czszbeeo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfupuoxj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3swfxcfvw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3vwfzszmq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3znbmiryv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aklujgrx.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3svanmlkh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qcdbrnft.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zxkupfys.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qwntzrup.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3enrylblf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3glgnesyu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tcphdojz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3yvjukaoy.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hqqileox.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3hwclefwr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3svrbuvew.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3mydwpqbz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mhovrbjq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kloatbha.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ksqlhuai.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gxcjejmv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hvpuxrxm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mijrwiov.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdcgxyl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3gpnralui.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dimrakvl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nqprwuyz.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pbmxvzkw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3ivmstzig.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fyiuabxw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3xcbjviji.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3uyysqttt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vnktndqf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ovgugivl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xsbcwbnt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rddniewn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3syotuctv.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmuwrgfd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3swzpfgbw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3awegnveo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3guipgvyf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sgkkhqqs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3aozailbd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3caieqfqn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vvyvbhax.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lastuibx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3myddnamy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yhitokww.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3yfnifqrb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ojbocdxl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zuyqtigq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3epyshhoe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3uhwuswgv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3atztwizd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sruovowb.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3knsquobk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3btgyrsgj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kmemvakg.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3gsrufomy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tjjsbjvj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kpynnckp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nusojgnu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3yawkdvtr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qygajsfk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3oiqmfxqd.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ahioilly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fsnfkaqf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3npolpfhf.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vbaerves.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mjkhongl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3utobvszy.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3iwvoffed.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ccerxihr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3lalnnjpq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3uruflwtl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3wpfvpkaj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3sebqpatn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3fkbdyzti.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ubzlcfyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tqhcbyrw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcpxwxwc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qfiqhlbs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3whwbvnqd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3efjajugx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wahgcppl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3disbbezm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3rkjoeupi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nimozxgf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3unjngwkp.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ndugjgtu.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ogwiqqgz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwxcfoxi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bzdhubsr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3oiuqlswo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3utavgofv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3nceynuzd.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fcvkqrvr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uchhmojw.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ebpiujxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyythhmm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gbgwszgf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qmvnsghv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yiohamur.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3skljyuyx.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mrmbutae.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gcjdncvo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3stffjgqr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hlcfemnv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3erhibhee.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3piptzglx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mulvrogk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qxhdkapw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3nakklndy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bguteggp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xoqwxrdl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dmwrrlae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bulggvre.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3hrnhduaj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fzwgubvw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3docohbdw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3grkyolgb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3gxonulqx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jegmkqgb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zzgpokct.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rncbtaeh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tmqwabru.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rptydbqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3pkvwpwwn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3fbuwjtpy.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ctyaeqvn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3sfsrlwbe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3mbdxhkfg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3huibjoxy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3cjevkdmq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3maonpiyq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3vomhqpfx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jiksajdd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cqjozgyu.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3duvmlqcm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3rormlfkg.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wshmmeey.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3tslpdexj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ghsatfpy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tgqchcyd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3irubredh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3vtibqjdt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nemsllvb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wegcqzna.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ndiifmee.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ayqxjqdn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3sozmofmi.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3zoljeguv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lquekhwg.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkmkcloa.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jqcaxnrj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nnjnwafw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kshugxzm.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcrycmbc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3wayhnznp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wqjadndu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zlznopon.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kfafecbz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mgqijmmy.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3viwcnxbd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tjvsboma.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rnhhfmta.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3uwrqhwqy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3unjvnshr.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wibepwgd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3ccckdrah.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hvjfwgno.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dbtxggld.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3mvfjyxyw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ecdvcdhb.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3dwqeihyb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xchbktub.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lvbrmmac.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gutlaqlv.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rxcxwvzr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xppiyneu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fsnynsow.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eyfwpqfu.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3prlqpsmd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ixjvzlmb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ldlikzng.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wtieywtl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cnvsmnau.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3rgvhmyzu.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3waydggjd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3rapdgxxt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3eqihmglo.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ikdbqpzz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3kuffdvvf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3kliqlmbs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ygindpeo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tverfttg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gagslhtx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3boqdzwtu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cdwigywi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcwyunv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mpgbmsed.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qmzzyege.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nnqqtgyn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qmbpycan.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hrphaurf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kmqhnupm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3imtukkkv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3gluyurex.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ejlyhnqz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ndxwmats.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3spzwiqki.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3wvlaxead.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3zlblxqou.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvkdhftv.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ewarmkvw.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tysuapcy.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bordrplb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wgtqdmts.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zucxeaba.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bcsdhnef.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cilkhlkf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3qcxmrpjl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycsyabug.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nyxznqke.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtqmcob.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zfqffcgx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hblrzlhk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3recnhmbv.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cnbgigld.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vqdfihpf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjucltth.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3txzazags.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3knyhvipj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3byqpvqgo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3cynkmmio.html


<!-- 参考信息 -->