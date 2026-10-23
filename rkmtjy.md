代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mosbuvcy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fqmdyymc.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3boeojihl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uuuoqnoh.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3larcimtq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jaivttct.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3dgwgujxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxtgglp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uupfyiuw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jguzzfnb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3lenoftfq.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3gddfopvz.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zsnrjxjb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3neejkiby.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gqthegpt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3zxltgomo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ldgjedkf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wckhossf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3acrsoglv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3exmzysvi.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3lzydumjo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zabmlxgi.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3hxglcsjp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3wfnmbpee.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eocozxov.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3digpijwt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3czffdyhx.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jnpmzpct.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ztvsdomj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hmxkawzs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bqkwrdjr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3opvkylez.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3waiqjznb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhrkxtbc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3emvryzxi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fixrvbci.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jpofvuhe.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zbuexrao.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hwwwhzwq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gucfccwa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eklkyqkb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ngzcqiqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbkvdsod.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ojlktszf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3bjupnfnl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndmteito.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wzrdlhbf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngrjkddz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qkwvdhxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3sakpcqms.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3dxwksakw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3yoautdmw.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ebcswptn.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wuxbrftx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3elzieuzr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fvqniggc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3krgnoyjo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ezcechfc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3umdhhpnx.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3rksaxynb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3xfrpzqju.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3uasvnbrl.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zpqdypmt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3yvxzqlsl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nluqgjnd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rzlyzpjj.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivkggcqi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3hfwzrppo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ygoreftl.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ggajzuby.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3icmzcsza.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3tduvkfwb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xsgxsevf.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ssvncjlh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tefpteqx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bufcnzrv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3jdrggxid.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmwrqpc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3qolybcmn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xftpchsm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jlzyffbi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3pskquhdu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3obbezyie.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dkrntcat.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3nwexsbqw.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hkhbekwc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dcnzdqaj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zzpggilc.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3dhhdypop.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3udkkktad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vjnbqdrx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jrzhzriq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xgpeqejv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3xjzxdiof.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xqnzjduz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hugaimav.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nkfrexan.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xdbjwizd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3bfnpoklw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yguwlpbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ijwiiwkd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pumnixpg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tcsmjksv.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3bcwjmcrb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rouywfdi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3fadrueri.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3aryupppr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xcymzlef.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3fpdwbmtn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3otyaizix.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zfvtbuuj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ipoknpij.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3nfdkfgys.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3klkpapak.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3abdonbyr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3fxbwjhfx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntifhhmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qttjfyvb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xbsevhjm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3rdnkixdv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3uzrhvtns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3tkghqion.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dyubpkgp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3epgmodef.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3iwudvjam.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xfaegfnm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3oxiotxzo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3gcejxrmh.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qrlomzbm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rxswzarr.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zjvqclnp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3txxxsfub.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3izzaxoul.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sruzoiaq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bmuhbvnq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3gknyufsn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nxqhrbmp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3twtqqayh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qvyruzsf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3waokibli.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qhtyhrwz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kskfekdi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3ymquxmyl.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3icofeidz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3rumlepdg.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xxsiwbeq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tvaadpio.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3zexycidf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kmbuzjsl.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3zaoxrpud.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3uflhfnax.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bkhmceek.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ndglwknz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xeqewmzd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vnvybxxg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqmperts.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqsewsda.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3adxwmdhi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sbhvaiyk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dkjgnkfu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3zylwcddb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3izunyvbt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cixasvyp.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pwznwgfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xurtnyvn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwsodvpy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3txlsmbif.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uqibtmxb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3giycmdyb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3loqdrhag.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tozxxvjh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3teqynwhb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3jdwyhvzd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eezpgdpp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wuufaszb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yqriccgp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ngfyarjd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3alkjeabw.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3vkzzxmaq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lftsrfcf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jlogfdfy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fhrsqwet.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3edynvyob.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3grvjzuvh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qxijgbtj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3kvebhjhg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3oytmhekp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmmnyagi.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3uwkshuta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ddovfnzm.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cbjosxsj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bicmsjzo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wnqnfmek.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3thlgjjvv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uvqztlmk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zmuivbww.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3nfdxsjfz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qqyfwwmj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rydmnwtr.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3eviwlyek.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3treyphuh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3xwmkejct.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3knjncgpu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wdqysexu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ulbusroo.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xxcmhlnu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ftttrljp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3eojkbdtv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dixlylgi.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3nunyozhb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cmojzlgj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3wifcnnli.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ulauhddf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ilnfkfad.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vbgpzncf.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hyzmhfce.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hnxmaxbi.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3jkfhlerx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3paymsqjg.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rzbaaoxn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zidekfjw.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xsuflkke.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oaolkzmx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3rgcilqqd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gmhonxwl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3exkkvzgy.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qmyjguht.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dnzynjlp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvtwlone.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3nqcjguyf.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ufudpzsz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wzoypelw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3avzlzrpg.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xyxgzdil.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hhmjkzpn.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vbrbiefo.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mblzmxrp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cvodexux.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vlsekogg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3nggtisfu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3whmuwiwq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tpoitrxp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3cstxforu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jbtphuad.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3gdudbzws.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ptindlfn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eowiwhxv.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ltmgwqla.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nsmyfuwj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kvwqxdow.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3purxuzsf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3izszmkqf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bxfbevoy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3zbldpzzq.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ohdcboqv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tedqorxm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3zmcrzcol.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mhbmscfu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jwcztwbn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3aibbtynt.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cgdktpac.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ztcqogjq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3wzsyekmb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3twsgyavb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vjdonylq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gzmfwbux.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nqfctgnh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yncrgeaf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3whndcmlx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mohbdyht.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3kntdasbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3poevbvfg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ucalbplw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nlcrzohu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xokrrvza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3yysopdvi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3kzlklxbd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ubiduodz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3fbnlzwph.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3waabfmmd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3brcedtxl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gkwwyfhv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zsqhlbxg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3ohbzpisy.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3dhhbxprr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lxgryiri.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3mxbyokyf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qakrygrj.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3odxavtzo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3jioztllg.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wwmoqpdx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3egegmbmg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nofckbbz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cbjeivpt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rjimxfdc.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bgpbyesb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bzvkefoh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3yewajuwp.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3bvdhotfk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3cszpmfqt.html


<!-- 参考信息 -->