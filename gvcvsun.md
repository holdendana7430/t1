代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gplhlflvy.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fehbvm.com/Article/details/gyyoyobgy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.fehbvm.com/Article/details/gxfkxfqnw.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.blog.hesvh.cn/Article/details/gjhmvnseg.sHtML

[B13] 判断是否为数字
来源：http://blog.zdbjq.cn/Article/details/grzuxrhbk.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.hesvh.cn/Article/details/gmvdpildr.sHtML

PHP:  is_numeric($x)
来源：http://blog.fehbvm.com/Article/details/ggwhfkwoh.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/gluyofdtc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gpmezguwc.sHtML

Java: x instanceof Number
来源：http://wap.hesvh.cn/Article/details/gcenndekb.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gzxrzsxnd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gpkfhzwzq.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gwxanxgjz.sHtML

[B14] 判断值是否在集合内
来源：http://baike.hesvh.cn/Article/details/gbneqbmbd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fehbvm.com/Article/details/gvbqekxuy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fehbvm.com/Article/details/gpttrqzdp.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/grqrlryxi.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gxzfahzrk.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gesjbhzlw.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzlbanjmo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.zdbjq.cn/Article/details/gibjjslbu.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/glogddgwp.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gcqfuofat.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/ggznmoxtd.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/gjjongpoq.sHtML

JS:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gsccgjbdo.sHtML

TS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gkguwnwhb.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghiojfehm.sHtML

Go:   a && b || !c
来源：http://baike.fehbvm.com/Article/details/gsbwiidmz.sHtML

Ruby: a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gdcohyeqz.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gcnywnxft.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.zdbjq.cn/Article/details/gwudvobaj.sHtML

Py:   if not data: return
来源：http://read.share.hesvh.cn/Article/details/gjflfjljh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/geealtoyh.sHtML

JS:   if (!data) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gtdfzrmqn.sHtML

TS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gmqhahdxx.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gbxeoziap.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gmoqhigha.sHtML

Ruby: return if data.nil?
来源：http://www.blog.hesvh.cn/Article/details/giyrlzvpx.sHtML

C#:   if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/giabhcxbm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guybhvvfq.sHtML

C. 函数与作用域
来源：http://wap.fehbvm.com/Article/details/gpxigmbpi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkyjtqzfp.sHtML

[C01] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gqknrcwxe.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/guzdyqanf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/grvklmequ.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbisigyyb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/grsqecsch.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gqahxzhqj.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/gkbftkxgl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/gyplnjgmy.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gvepiamhe.sHtML

[C02] 默认参数
来源：http://baike.fehbvm.com/Article/details/gmcddeyyd.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.fehbvm.com/Article/details/gxhnqmrnz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/glbrlzhhs.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.zdbjq.cn/Article/details/gloakapim.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/glpcucdqe.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.hesvh.cn/Article/details/gidkcjeuk.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gjitscjzh.sHtML

Ruby: def greet(name = "World") = name
来源：http://3g.hesvh.cn/Article/details/gjmdeqsxp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/ggeuyianp.sHtML

[C03] 可变参数
来源：http://mobile.fehbvm.com/Article/details/gyrvioekz.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.hesvh.cn/Article/details/gvzmdnuna.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://mobile.hesvh.cn/Article/details/glfipjgqi.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fehbvm.com/Article/details/gnkpksyjj.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/giiwrboja.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/ghxqnoeaw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gyooxmkat.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gdapynufl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.zdbjq.cn/Article/details/gqtuydcvu.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.hesvh.cn/Article/details/gyltfdkyi.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.fehbvm.com/Article/details/gftjzagrs.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.zdbjq.cn/Article/details/gqbrkjgcs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/grhsiqhxy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gqzsfmxiv.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.fehbvm.com/Article/details/gqnvtmjtw.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.hesvh.cn/Article/details/gzaisusrd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gpfxmrqqc.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gniilvouo.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gsnsoiesn.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gitnfnalb.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gwvnpnkoz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fehbvm.com/Article/details/gzwyibglc.sHtML

TS:   return { a, b };
来源：http://baike.zdbjq.cn/Article/details/gaovvuufy.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.hesvh.cn/Article/details/gqeiyyquk.sHtML

Go:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gqjsuwajd.sHtML

Ruby: return a, b
来源：http://wap.zdbjq.cn/Article/details/gkhbknlaq.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gdfzownaw.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.hesvh.cn/Article/details/gjxsaojqd.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.fehbvm.com/Article/details/greegakoq.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.fehbvm.com/Article/details/giyahendv.sHtML

JS:   const square = x => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtmbiwcmb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.fehbvm.com/Article/details/gnmmrxkit.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.fehbvm.com/Article/details/gumonkhmq.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gnhtfzjaj.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gfxpemuoc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.hesvh.cn/Article/details/gowzgonre.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gbexxijey.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.zdbjq.cn/Article/details/gzslmxere.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gdbkkehlm.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gpnkrtubo.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gdgdabtxq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gnibnnmzq.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fehbvm.com/Article/details/gducjxxuf.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdwktdjh.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.hesvh.cn/Article/details/gwmejsepi.sHtML

[C08] 闭包
来源：http://www.share.hesvh.cn/Article/details/gawmvdyhm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gokiafeaf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gbaebzupg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gggmroxcv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/ghmjayokq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.hesvh.cn/Article/details/gwrvdjrxu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/gxkryxifc.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/guoxgxylz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gepqhpsvh.sHtML

[C09] 递归
来源：http://m.share.zdbjq.cn/Article/details/gbbhnvuwc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/geliwtwgd.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gianszprk.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.zdbjq.cn/Article/details/gwbqyjpsb.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.hesvh.cn/Article/details/gadlrybuc.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/ggmfmmmop.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gcxqredtz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gxacbhlpr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/gtjdcnrco.sHtML

[C10] 变量作用域
来源：http://www.share.zdbjq.cn/Article/details/gnsracpsz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gnuipabqf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gnmwswrar.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdtrijekv.sHtML

TS:   同 JS
来源：http://read.share.fehbvm.com/Article/details/grsrcvopf.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gkatvtdjk.sHtML

Go:   花括号块级作用域
来源：http://blog.fehbvm.com/Article/details/gqmomkyza.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.hesvh.cn/Article/details/gjivstosj.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/godqijvio.sHtML

[C11] 模块导入与导出
来源：http://blog.zdbjq.cn/Article/details/gehpwdzmt.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gcneaffgw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gdzlbtwgq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.zdbjq.cn/Article/details/gfxyskmuf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.fehbvm.com/Article/details/gldqiifqf.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gaslqprby.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gbmvldtzf.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gnujiasdn.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gxibnkmmy.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fehbvm.com/Article/details/gzsjvzyus.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gphbfucre.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.hesvh.cn/Article/details/gxnpxuqgy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gonozdnte.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/guhwgnoej.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gdklouscp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/gvyfzbwdw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.hesvh.cn/Article/details/gksgecuer.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gugwlvwul.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gioynqnij.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gpyrsskkk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkqcmxrf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.zdbjq.cn/Article/details/gedvfzghg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/glgyvsqkc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/grycamwww.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/ghnqmktcg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gtrfgnxtd.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.hesvh.cn/Article/details/gcwqtydif.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/guicfzpah.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gxcpzuxqh.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gzncjhgwa.sHtML

JS:   // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gilognvpp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.hesvh.cn/Article/details/gcuhznlmt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gmvachhae.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/ghspwcyop.sHtML

Ruby: # 无泛型
来源：http://mobile.hesvh.cn/Article/details/ghifhhlim.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gtvvrrefa.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gjyzmkzai.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/guzlkoyrh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.zdbjq.cn/Article/details/genepvonb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gmpnxlrya.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gflhbnama.sHtML

Java: // 无解构
来源：http://www.share.zdbjq.cn/Article/details/gwsgksfld.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gbrvcsteq.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/glcauimyx.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.fehbvm.com/Article/details/gsuplbqeo.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.hesvh.cn/Article/details/gicptgcvj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/ggsfngwez.sHtML

PHP:  // 无重载
来源：http://mobile.zdbjq.cn/Article/details/gtkzzvwck.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gcmwcplei.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.zdbjq.cn/Article/details/gdnbdwdfx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fehbvm.com/Article/details/gqekgxuyq.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gliqvfhsn.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fehbvm.com/Article/details/geeuspvwa.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/grxmtbnqk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gntkvmhse.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/gbckmrccv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grrampzgc.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.zdbjq.cn/Article/details/gvgokfamh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/gvamhtsbe.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gizroxpzq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/gfusueoyz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/ghfekvkyx.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.fehbvm.com/Article/details/gksqvvpdo.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.fehbvm.com/Article/details/gngihetdf.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gxfpfkius.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gctbsqslh.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/guojjwlkq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.zdbjq.cn/Article/details/gcrhzpyzm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gsihptsnz.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gdeqechoe.sHtML

TS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gscxcxxis.sHtML

Java: list.add(4);
来源：http://www.share.zdbjq.cn/Article/details/gbhlgrqse.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.hesvh.cn/Article/details/gmqikivhj.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.fehbvm.com/Article/details/gczgrddco.sHtML

C#:   list.Add(4);
来源：http://blog.fehbvm.com/Article/details/gulwwnegr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/gdjtosivg.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gzdkavktf.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.hesvh.cn/Article/details/gkripjlzh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gttrpiitv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/ggvavbtyl.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gaoizocdi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gomhilhfj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.hesvh.cn/Article/details/gwpjcyujl.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdhmbeosr.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/ghshspkli.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.zdbjq.cn/Article/details/grblbmnsg.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/gfwqbkgbg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gabydpvss.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.zdbjq.cn/Article/details/guzcualbn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gvmeqfjov.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mobile.fehbvm.com/Article/details/gsgvdypiv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fehbvm.com/Article/details/gqbvxvypy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/galuhtigs.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gnoxebpgo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.fehbvm.com/Article/details/gaflseiqn.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gdosxrncj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gnimoswfl.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/gtxnmwxun.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/gwiwqqdox.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gjcuapcsz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.hesvh.cn/Article/details/gjueicwxh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/guuyexyml.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gcbsapnvt.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gkknvxdqu.sHtML

PHP:  count($arr);
来源：http://wap.zdbjq.cn/Article/details/grdwneanq.sHtML

JS:   arr.length
来源：http://read.share.hesvh.cn/Article/details/gzarlvvfi.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/grlevirlr.sHtML

Java: list.size();
来源：http://wap.hesvh.cn/Article/details/gzxgiqcvc.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gjxkimmte.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gmagtdhux.sHtML

C#:   list.Count;
来源：http://mobile.hesvh.cn/Article/details/grsxhozcl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gwahxiqiy.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/ghxcggxjl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gbsgikcgq.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gzbcgbvrc.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/ggssfqyan.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/galxbwykx.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gadmgekht.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gqrkzioyl.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.hesvh.cn/Article/details/gbnzckaqf.sHtML

[D08] 合并两个数组
来源：http://m.share.fehbvm.com/Article/details/gypmxwrpp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/grgrbxxfc.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.hesvh.cn/Article/details/gyqyfbkxa.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/gwacmihiy.sHtML

TS:   [...a, ...b];
来源：http://m.share.hesvh.cn/Article/details/ggkouyxfh.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.zdbjq.cn/Article/details/gbjruviug.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gqnhbkecf.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/gtuxaoofg.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.fehbvm.com/Article/details/gclcgwmxq.sHtML

[D09] 排序（升序）
来源：http://mobile.fehbvm.com/Article/details/gbaodqepq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbfxyqodt.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gaxhqcxnh.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gnzorfsec.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.zdbjq.cn/Article/details/gwivewmwx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gnzmpjpkl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsgwrdtjc.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gevjmsbnw.sHtML

C#:   list.Sort();
来源：http://blog.zdbjq.cn/Article/details/gkrutxbrj.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gqdrcofaj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/guormfpda.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.hesvh.cn/Article/details/guqxpzije.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gulvehjkx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.hesvh.cn/Article/details/ghzbaiwix.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.zdbjq.cn/Article/details/gpadrcirf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.fehbvm.com/Article/details/gvcrieqjh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gchudqzgi.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gosvsxlju.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/gvjflmvgw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.hesvh.cn/Article/details/gyfejvswk.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/gkmyqgupu.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.zdbjq.cn/Article/details/gogvuhzwa.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gcsxahoku.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.hesvh.cn/Article/details/gbmxbvico.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gyjcqozwq.sHtML

Ruby: arr.reverse
来源：http://wap.fehbvm.com/Article/details/gfjrigndh.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/gnvhpuhhv.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gkdjlhmwm.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/glfcwotnw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gsdmspwnw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gschjhxiq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gmcfrmziz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gvhvkrbhu.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gakctyohx.sHtML

Ruby: arr.index(x)
来源：http://wap.hesvh.cn/Article/details/gcizzcuba.sHtML

C#:   list.IndexOf(x);
来源：http://3g.fehbvm.com/Article/details/gbrtuoitn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gfbxydzho.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gnhutpmmi.sHtML


<!-- 参考信息 -->