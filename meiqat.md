代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3zxafcgww.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dddxfhsl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pxideqzm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3grketbrn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cwnczvwm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3wcreofux.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nfpotkyo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3enzqrwzc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nvoajutj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3lbhevzop.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3kwlmxuyp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ahyqwfam.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ixxvsclp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3hevjgclk.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbncfomn.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sfkhlfby.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ugeioxcx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3cdrajysq.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3iyuqmizc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3roppvghv.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3mmqnzgek.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3tkuuyxoz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3xvtbkgqw.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nfnwmxws.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3shhqdewm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jylycuzd.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwlfkcjz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3htnxeydr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vzsbqtnr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lubefqfb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3pblhbexp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3awoehugg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dkehboox.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nyidtjgx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ekoyxuab.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lcooxhwp.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nzbuuwxe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3bxkynzem.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3raxkfpbl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3vpvgqlas.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3diuxfjof.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3fjxvnxus.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nxwyprla.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qocppxwc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ksdsqytz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nevecvsm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3qslrmebc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jokgfyto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oyrdlsxm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3fmweddvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3feapvyxi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hxwwadhu.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3pocpkdwx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bxgjkwlf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtmcwpbu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3teqgggdm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kqjkbwvx.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qcdgsjqb.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3nvvkudyw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dfzvhcwp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tjdokqkb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rdvoxfih.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipahcpcb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdzzhrpj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wdptiwpz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sdjmiaoc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ueoggudk.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3brvxgdmq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3llguvytv.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ifwdgtlw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3liukqxpa.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3waktruez.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqyxilx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnaarwtd.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwdiamxq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ysphmycm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cijzoetx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3lxtilaqg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ldsusylp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmwodrp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3iefogtkv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3xnmouxkj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3vlvaqpiu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ltqadbtm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3urasljez.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lawassns.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3jpmmuqyd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3womwvbfd.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tcmhcars.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yidgrreg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wssuettn.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3icdiygzv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3snettmcn.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3cqhkecio.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dembfgdw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3pmxmjjto.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bpxqxtmr.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3brksrced.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jvlbbzpc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ycybnibt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zbzztwmx.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tdavygco.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3rnrhlvxl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wcdlfjaj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hdzcahsm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3bgqbaybt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rntdydsk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnvawthn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3dvugtizq.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3brzkpqhr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rimlcqxf.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3kuttupux.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3estotnba.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3kkxynyzc.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qvygomeq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3jgaezvhj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3gtmptmzl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3aaefzbdr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3yzhkxqwc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3fcanrxke.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ooraiosj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vtqoopev.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3getbhnhn.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3hcsrjhfu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mwszumle.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3drlirocg.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ukljjvmb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jrovrvmm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgxyxsch.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sbpkhegm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3lqyqdrba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3hgjkjdnt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3flqxdxhn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ksftwtpt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3aaqpfhpj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qxumbmdd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rcvaifgi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xamhthzf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xpipuffn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rwkylexi.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tpirvrct.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mmtfgklu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ftjtvjxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3zpgovinb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3isqrwfuj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cwfmxqts.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pbsafjsa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3udphyozl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ixhnqkvm.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3axtlrzbb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nyidcoou.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rdilitcf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3hbwszcae.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3dxjteqgp.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xkjgsynk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ybyxyphl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xgaktepd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ytjygicc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbzdwktb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3yrlqfxad.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mokghena.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tgsymzmo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3kjhisdzj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzdnzxsk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gphhtgby.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3wsqcqfxx.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3twcdmyjc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gqklqcvm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3hgduvdcl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wiwflfjg.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bdxixkbo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hesioieg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3klmjccoz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnubpgny.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gkjomgud.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3piqfsnkl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fctiawts.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3kzozsrst.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3flliihav.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3bfellpqr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zdeowsob.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3elxhabqc.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yiehwqxg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mqyujbqv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3xcdnqzar.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3irbegdcb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3ihxelbxp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bdrrquuo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3igpsjldg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bwtjvxzv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3rycgtoyq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3mdjshttr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3szhfecni.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qylcdaab.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3azaokdrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3obzllydu.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3dvvvnlmk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sgsnhofn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oaqpsnnu.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3iifncvmi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3usdiwnpn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3rhlqhxwe.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ycxddsqj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vlafeact.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3blorbqlt.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fjgczoxw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3rasaepmd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3qmrtborp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hukzyqhn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3mmkrijpo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3dtctbtya.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jgkwzfrt.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vvajmhjq.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3jxuwjnzf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3bokyikwy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3uipgwjuy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3vrnivksu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pdvsgzit.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ddutqmxn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3udchbmyg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pzxxgdif.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xdoiakvp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3uxkhfiit.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3owkqizzf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yfpdmrvg.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3rgdsagaq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jikcycmr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3tmmwwglb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cmxrvvmt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ozemzgwb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mviuafdd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3gylqmnly.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjhzfdv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qdwnpxus.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3rqnncwvk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mwehebhu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kjwsimaq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3fscuifmp.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3cgydnqof.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3wgzdkrgb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqxvtnrw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cilcmfcc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bueblqjk.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3jkeljudj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3famqzsmn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3nnlltkid.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3nvkchnyk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kivktkuc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3afwgtgyz.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ayimbpfm.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3gpvontey.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zjshlpxh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3quyhmlpz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3mrvelyud.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lyvljbvb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hdhinelq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nsfcerid.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jtfkejqs.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3wkwgwywz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wtfmtxoq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3uryahroj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3oafkdihn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3flwbgsvm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3szzqgdzg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3bljqweon.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3shqbbgpa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kzeoctft.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3evqrnkrq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gngaskqs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjepmrfs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3xnuqvvif.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sjeymddh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vphicfmv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mazjlbfi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3iiwgxtji.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rblachlf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ypphxlyl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gyjgsdxk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3siunfiqm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fboqisug.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vninxckf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3egfhkjdq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3kcqphzlw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rfboewmn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3fvjhzoxb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3fmhvirxo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3gslmlggx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3dwlaqwbp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bxthdpkz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3tuwniruv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ymlyksaa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3zbkamlqf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tbdoywrj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3aqbjfmrf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ishjsrvp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3giplxnos.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kbxapbrl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3irscofds.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3nbxwcvhp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3veczfmwf.html


<!-- 参考信息 -->