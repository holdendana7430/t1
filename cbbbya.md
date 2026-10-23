代发 wailian999

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3pvqssncq.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iedsbtco.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3udxdysor.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mzaupjat.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3jpdkzctr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3wwmwuoup.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iyqyhlmt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dqovqilq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kdeljmxs.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ygtfgzxr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hbaqcsfx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jmoxkjdr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ljqyxlqr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ghkedmwu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vczlychj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3odnepaxs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdntriao.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ocrvelff.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jyvhjerx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3hwfkitgt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3fulluvor.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vrvfkzte.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zojfjpkk.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mtrtbxjg.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dmkklvgf.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gnfawzad.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dosbaqbj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ohcnoydw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ssxjeiww.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3yznpmavm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bngwikrh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3svjldene.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3utjhxpwj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3dtmxmzgx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zneypcju.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qxzvhvxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uujeanat.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hvprxjpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wjrkbgeo.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zzxkpwiy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jreitavz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgiitxby.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3toolivvw.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vueuwezr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aiufteci.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mtgqjfyc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3onpsfemy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggxnblqe.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3trspwcaf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3midvgfwv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xaoikpcr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ygqsnorn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yvebyyha.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ghzmaxua.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3oqgtkpbx.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zqdscmmr.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vupqzygh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwlebais.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3hgwesbjj.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qzjuxbwh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlrhjsnq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3tygbdgtr.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ipglpetz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gsykihti.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfwhraqn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zzvsngnh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dlksrcyz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovoljvbn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3nlxpfpfo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3qxjctmgj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bbwbqaeo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3yevosome.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3cqbxilvp.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3krlecksv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3phmjplli.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mcfmviyl.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3smlfxkrx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3turvobix.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3xtfmxjbs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tjlytasi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3smbkxjwf.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ullvzwvk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bemcmnim.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3ooaamufq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3chzqyhui.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ivhbbdlm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwczaeoi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3pivmatba.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yvexpmzn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zuswmmml.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gfzpvhyy.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3oimeeqeh.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wwkqzaox.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tpsscwrr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3hpogwgsq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hllklebt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3odpqzrrq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3esqrjybi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3npswnawd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dlyfzfty.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3zvsvszse.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3noovglgi.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3kwwmypms.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ppwnruxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3foxhdmze.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaqmixce.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ktryvtry.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3bxxfaekl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pdteysoj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3nemjwmic.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ajqqeknv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3psirsdmw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfkntrek.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yrdaqdpe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3amtqambl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ceurdbhf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3glrtamhu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcbvtuk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjzexqyv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kfaadozv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zifwnnme.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gcpofthm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3phtcvbax.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3wvrjcjfx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pxygtizr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wdkubupm.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3invpzpqk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mttsknoj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3idsahbtj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3xuktckzc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dtjswumo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3metsywcw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pmbcepcl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3bgipmkmu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3oztpnypn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ikegfxxd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qmkizwnp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3edfqcbcd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rlulykoq.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3oziunklc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ocxeyplz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3zwpoamfn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jkcnswdg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nvpofhme.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gzjwlort.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qenoarnr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zcaizrfi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ikgygmqj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aongrnpe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjirnkz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3hdukgyfn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ckqlcdng.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdknvum.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ayunujny.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3exwnuxuy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3cmorlgrh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzawhhuf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dxgrpdrk.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ytuvzinx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3capjcdqc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3iuueehkw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3rzvnqahh.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3vtivixfx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tkrlaaeb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lnlspebx.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3tsucuttc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3apblzphm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tjylkcrc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wyivmill.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lyckhdqo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qmahlqrz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mrvnjuib.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3mwrsnuqv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3xmfsxeqa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rqqxneza.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3mzwgxjca.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3feeublfb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqptir.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3uayqtpuq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwhhtcxe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3sbgckfcs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3odfltpdb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhbpgosb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txrwflsm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3hnznoghb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jwlquoif.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fwydtoeb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3bakjsmmg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3mgesusvs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cwsjpptw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jjwnxpir.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3qkylmole.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3joomaafn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yaztnhcl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3igyxhbwi.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qowzlnlk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3akvcnzvg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3quftemyp.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3eozbbkgu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3uqjnquib.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3haqtfbmn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3spndwkmw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3hwfjvwos.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bdggneiq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3yxzorqky.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3muyxdzpx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3giznmltt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3sdcydkfh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3chqgowin.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vijjurkp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3suorwwsf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbqclxdh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jtpikmvu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ujzabpyo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ksklogen.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vygwtiwq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3wyhpskyt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3spdiytay.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rkzxkdnn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3jlvwrwmm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuxdlts.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3kxrbrlqa.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3uiutdzwc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wzrsmytk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3crfgzjvd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pbwxpqsj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3anebzpny.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3aalfjmfb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3yeievwkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qrlguiue.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mcxzhexm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jvghbapi.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3bjfjoyyk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nagudwkw.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbvsiwdb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ratkyzco.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3kqwvrsqf.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ekiolvjb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3gflacysj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zuhgxzqu.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3mvwqxsor.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rohiqugm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hjblrubp.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cxawyycr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zuxysnmv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3shnehoqk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3kshoaewx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qqheprnr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kjsolmor.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bqrpfltd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3eimhovlc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ntbilxys.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ullaxsry.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3esmorebb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yznxfget.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jxcukcya.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jywtypou.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rtoigxni.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ggrkolme.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3bagrkewu.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3pnauyrrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ilyvhryo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3hfgumvbr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3ieklklwm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3kuoodzcr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mizwiraa.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3nhvbzmat.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3zjjjpsuo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3sogjporr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdxfogyk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eomiwopd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pxfgrqsw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3owtbimyi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3aylcqecr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hkonbfyy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3iofazbgs.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3psdagkst.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dtfiygqx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ffansrvk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3dwnqqihi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3efxsezdl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ldxjlwew.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlddmqdw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kisymkha.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yhdmncug.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rxrpyisa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3idhrkped.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3flzerujr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tsnajhsz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3upyldsuh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3lpsilncg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jcvzopts.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mjcvvrdh.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nnvhkaho.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3thkvybbg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3alkaskon.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3qpjpxbst.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3qzyzpbbh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tbbwhpfp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3xxhunfio.html


<!-- 参考信息 -->