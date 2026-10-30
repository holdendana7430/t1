代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.hesvh.cn/Article/details/gosryfmqb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.zdbjq.cn/Article/details/grsgbjiwa.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gdlrcqxrg.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gwdkausji.sHtML

[B13] 判断是否为数字
来源：http://mobile.zdbjq.cn/Article/details/gsiaobkdw.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.hesvh.cn/Article/details/gtbxzzlma.sHtML

PHP:  is_numeric($x)
来源：http://www.share.fehbvm.com/Article/details/ghihvfwuu.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/ggigexqrs.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gpitidpcl.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/gkhatzbbb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.hesvh.cn/Article/details/gejjzciua.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.hesvh.cn/Article/details/gqlbvwlam.sHtML

C#:   x is int or double or decimal
来源：http://m.share.hesvh.cn/Article/details/gjtqcobyf.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.hesvh.cn/Article/details/gpjbfyikq.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gnoxybxiv.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/guwllyvom.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/gbztemgno.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gzsdkptgt.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://wap.zdbjq.cn/Article/details/gnxxcvzrv.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/giuqvnfih.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gvtptcnfc.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gldxxnbrx.sHtML

[B15] 布尔运算与取反
来源：http://m.share.hesvh.cn/Article/details/gotwbzozc.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gvshfwtds.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gceknwuwy.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/goschvyhd.sHtML

TS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/ggioflpeu.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gxnozakwo.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gcbewwler.sHtML

Ruby: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gwxybvxsm.sHtML

C#:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gslppnems.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.hesvh.cn/Article/details/gyrqfcnxw.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gntfcyfpq.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.zdbjq.cn/Article/details/gukdxeqza.sHtML

JS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gdzpxpfal.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/ghtrnzscl.sHtML

Java: if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gzfaswskt.sHtML

Go:   if data == nil { return }
来源：http://www.m.share.fehbvm.com/Article/details/gsfhyrjia.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gkwgryurt.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/gpshaweqc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjxjurgss.sHtML

C. 函数与作用域
来源：http://blog.zdbjq.cn/Article/details/gvucrqygo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtzornqgw.sHtML

[C01] 定义函数
来源：http://read.share.fehbvm.com/Article/details/ghhiaarnl.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.hesvh.cn/Article/details/goxpcepua.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.fehbvm.com/Article/details/gjsiiffxq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gnwojoysy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/ghzrvacxh.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gxhjhaaqi.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.fehbvm.com/Article/details/gglpehfox.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.blog.zdbjq.cn/Article/details/gaprqewsr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/ghtlsjkvl.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gexatlztw.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.hesvh.cn/Article/details/gpjxuzssm.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.hesvh.cn/Article/details/gddxtihqs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gauvnbtpg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gnbexjaco.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.fehbvm.com/Article/details/guvexhzfy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fehbvm.com/Article/details/gyutrwkyz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gshjqectw.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.hesvh.cn/Article/details/grcgpkwwu.sHtML

[C03] 可变参数
来源：http://www.share.fehbvm.com/Article/details/gmappsqrx.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvszecnu.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gggcjtdrk.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gdgeukzpx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gibwszycf.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gklsvzawd.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.fehbvm.com/Article/details/gwyycuxxm.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/goygpwxtc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.fehbvm.com/Article/details/grgdorwbc.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gasbfthuu.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.fehbvm.com/Article/details/gudcvgrki.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.fehbvm.com/Article/details/gxoqeitrp.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/geyflvcrv.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gozjbuhwt.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gebfdgskc.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/glxuspuun.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gjeakayve.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gqjcqvhme.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gwhddwvud.sHtML

Py:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gdxwuoypt.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gsweykcfw.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gjxkiorry.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gpscomose.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gxiofbyic.sHtML

Go:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gqtdcjefk.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gctlaqqmw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gchksvchz.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gvnctsopm.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gqebocmji.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gogtjvtng.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gvfutkmmp.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ggnkqjymc.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.zdbjq.cn/Article/details/gnyvojxwd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gmfeglyiz.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gtavgjiwn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gasojasts.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/guacwwrwf.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://read.share.zdbjq.cn/Article/details/gblqadzld.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.fehbvm.com/Article/details/gnlismosc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/grruxiyfm.sHtML

TS:   arr.map(String)
来源：http://read.share.zdbjq.cn/Article/details/grnmddfox.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gxcysfttw.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/giovtldnn.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gbxrlggun.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gxesoiadx.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gqtjrjmpx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://baike.hesvh.cn/Article/details/gmrvizlyo.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.zdbjq.cn/Article/details/gtkimrxxd.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/genqvlgpm.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fehbvm.com/Article/details/gytmsnztm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gzyqnqrgu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fehbvm.com/Article/details/gtjkerrur.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gjdhbwupq.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://mobile.zdbjq.cn/Article/details/gfkzggavb.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gvafkngcw.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gdgqaectn.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fehbvm.com/Article/details/glyaslwdv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gtbdcmiuf.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gzlwaqbmg.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gvhrtnnfw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.share.zdbjq.cn/Article/details/gmuqfzdjk.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gfbffmzvk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gynspdnrz.sHtML

[C10] 变量作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gbiniebta.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.hesvh.cn/Article/details/goyvgqtvb.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gknfajkhc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gyjtudzxz.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gvhyvixkv.sHtML

Java: 方法内为块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gleoyysof.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gcyrlhfru.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.hesvh.cn/Article/details/gpcuftwek.sHtML

C#:   块级作用域
来源：http://read.share.fehbvm.com/Article/details/ghetzmpaq.sHtML

[C11] 模块导入与导出
来源：http://www.share.zdbjq.cn/Article/details/gjjcsqixb.sHtML

Py:   from module import func
来源：http://wap.zdbjq.cn/Article/details/gjgqsabqw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.hesvh.cn/Article/details/guiignajo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.zdbjq.cn/Article/details/gjkfpkgjt.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gsuxfeeun.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gnfkyejpr.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gkangjedr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.zdbjq.cn/Article/details/gfitysbhm.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/govjylvji.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gpkkhdqtg.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/goqpwkvto.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/ghxaygvrv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/gbayxtmav.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/guzkjxtvk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gogjblqzw.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gybnfinls.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.fehbvm.com/Article/details/gbphfburw.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.hesvh.cn/Article/details/gjumhpqhb.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gxspmjroj.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gbixlahif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwgvagykb.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.hesvh.cn/Article/details/gkvoziyfx.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gguztigmj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/genwpsmrx.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gkeaocyns.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.zdbjq.cn/Article/details/gtzzswank.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gjkjnzmlj.sHtML

[C14] 泛型函数
来源：http://www.m.share.hesvh.cn/Article/details/gpyrbvoqf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://mobile.fehbvm.com/Article/details/grajndipx.sHtML

PHP:  // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gqmklqoqs.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gkmfocbnl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/gmzhbehgs.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.zdbjq.cn/Article/details/gpjwoghtq.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/grrgcjhsb.sHtML

Ruby: # 无泛型
来源：http://wap.fehbvm.com/Article/details/gfnielscp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.zdbjq.cn/Article/details/gekazweez.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.fehbvm.com/Article/details/gapvduozt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gvrvtqrow.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/ggsbawzfy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.hesvh.cn/Article/details/gybqsxfka.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gbxwvzrwz.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/ggqhhavpn.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/guwioywui.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gtqbsnyuc.sHtML

C#:   var (a, b) = pair;
来源：http://wap.hesvh.cn/Article/details/gxonnyfxe.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/girtgavsx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gdencmzyx.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gmxuntwhp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.zdbjq.cn/Article/details/gvkjvzlha.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.zdbjq.cn/Article/details/gbsqrbqyh.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.zdbjq.cn/Article/details/gpdkshkqd.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.hesvh.cn/Article/details/gppxesmxi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gqmdcpugc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gjjiajktn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqkgxhyxe.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gyctezuux.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grmbnizns.sHtML

[D01] 创建数组 / 列表
来源：http://blog.zdbjq.cn/Article/details/gbbtusknr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.hesvh.cn/Article/details/goetuhqtb.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.zdbjq.cn/Article/details/gnhczcmxg.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.hesvh.cn/Article/details/goflomuht.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/goghuttip.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.fehbvm.com/Article/details/gsseysoqf.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.hesvh.cn/Article/details/glifbokkv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gsidvxcyy.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/ghhzzwcbn.sHtML

[D02] 追加元素到末尾
来源：http://blog.hesvh.cn/Article/details/gbdvbnjze.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gmazrohlo.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.hesvh.cn/Article/details/gqwbhwhcn.sHtML

JS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/gixhoouuv.sHtML

TS:   arr.push(4);
来源：http://www.m.share.hesvh.cn/Article/details/gqtkihygg.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gfcyrqpwa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fehbvm.com/Article/details/gidjhewbd.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/glraoumnq.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/gphwksqos.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/gxbmgrfif.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/gpngdsjpf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gvjcefzkv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gbbnutjdk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/ggdhjsiqi.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gqqwndbej.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gkeptgkmk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.zdbjq.cn/Article/details/gsexsfxko.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gxlwhcvul.sHtML

[D04] 删除元素
来源：http://read.share.fehbvm.com/Article/details/glddyolle.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gjmfqxmyp.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/ggiitjxel.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/ghheeamdt.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/glfcokumu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.zdbjq.cn/Article/details/glssfponn.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/gzwdhrojq.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.hesvh.cn/Article/details/grttzxleu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/ghxxfddix.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gmmqqtwyl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gjylenyio.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gftxuphts.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gzmkpimto.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gahhkmcic.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/ggbyunjdw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gyvcjhezf.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gjfruinxb.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gkgsrexxn.sHtML

[D06] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/gjpylmwbm.sHtML

Py:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gvmpshnbe.sHtML

PHP:  count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gfdivcybc.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gkpbljpdj.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gsqqpoxvi.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/ghwvavcka.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/ghahzakve.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/gcibpqnpw.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/gricnnsqv.sHtML

[D07] 切片 / 取子数组
来源：http://baike.hesvh.cn/Article/details/gebksujho.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gbtngzhjx.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.fehbvm.com/Article/details/gsfudajpp.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gaxdkfceu.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/groeknkmd.sHtML

Java: list.subList(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gvvqkdwkq.sHtML

Go:   arr[1:4]
来源：http://m.share.fehbvm.com/Article/details/gojyppady.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gzfczmnca.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.hesvh.cn/Article/details/glyvprezb.sHtML

[D08] 合并两个数组
来源：http://blog.zdbjq.cn/Article/details/gsysqabvb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/giemxyndk.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ghovwvlna.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gauxvhkei.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gwnqcbisb.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gtmdakihn.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/ggjkoifec.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/ganenbttn.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gbrvmxuum.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/gzmhdkzdr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxtfjncop.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/ggrrujces.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/guispefre.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdexgwuyf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.fehbvm.com/Article/details/ggbobljlp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gklemwvmm.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gilipigkr.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gzrisiufe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gsazsozid.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gngpepagy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gybopacze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gqysomffi.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gvqmaymjo.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gdyqiytej.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/guuiibbho.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gafqptoev.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gcbrbfaqr.sHtML

[D11] 反转数组
来源：http://read.share.hesvh.cn/Article/details/giancymzd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/grjpfxtrc.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gmzgwdmsa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gdzbrdqvd.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gpaxdtlij.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gffkwwctw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gmjxfkkhx.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gbbqrhcqy.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gsluvohnb.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gowqmeves.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gzcmnehee.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghjndbhbe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxvpgtfwy.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gzrinufpp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gseqovzco.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gxctscizu.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gjvswbhmr.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gltknegjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gkdkshweb.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gerxlthks.sHtML


<!-- 参考信息 -->