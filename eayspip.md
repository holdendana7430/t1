代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fehbvm.com/Article/details/gkfvvqugu.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.zdbjq.cn/Article/details/ghyxqwjou.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.fehbvm.com/Article/details/gijdpsbvr.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/guwqaorvy.sHtML

[B13] 判断是否为数字
来源：http://3g.fehbvm.com/Article/details/gycjtorem.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.hesvh.cn/Article/details/gqrxsrodp.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.hesvh.cn/Article/details/gcajwcnoi.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gwfmxforc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.zdbjq.cn/Article/details/gthzxpebg.sHtML

Java: x instanceof Number
来源：http://www.blog.fehbvm.com/Article/details/ggfjnmbyd.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gxcsauzsw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gmkhdayth.sHtML

C#:   x is int or double or decimal
来源：http://m.share.zdbjq.cn/Article/details/gpzxfapoo.sHtML

[B14] 判断值是否在集合内
来源：http://baike.zdbjq.cn/Article/details/gtunhcfra.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.fehbvm.com/Article/details/gvofgwowk.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/genxprjuh.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.zdbjq.cn/Article/details/gnicnqfqr.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gkcpfrxvp.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/goysxsvoa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkkqzakla.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fehbvm.com/Article/details/gzcqklbfd.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gbfpwfqkj.sHtML

[B15] 布尔运算与取反
来源：http://baike.zdbjq.cn/Article/details/glgdtxwze.sHtML

Py:   a and b or not c
来源：http://baike.zdbjq.cn/Article/details/gagqtubul.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gyxvwpzui.sHtML

JS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gryjiyzqu.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gytnxvrrh.sHtML

Java: a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gyowagnxk.sHtML

Go:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gtzkydvhj.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/grlponkag.sHtML

C#:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/giwbyztyf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/guuqbdsrv.sHtML

Py:   if not data: return
来源：http://www.blog.zdbjq.cn/Article/details/gyjbsdfql.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fehbvm.com/Article/details/gqgrrhixo.sHtML

JS:   if (!data) return;
来源：http://www.m.share.fehbvm.com/Article/details/gucjrknfa.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gxnbllmbl.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gepejukot.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gmbuavavm.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/gkqoewrir.sHtML

C#:   if (data == null) return;
来源：http://www.share.fehbvm.com/Article/details/geswkgtiy.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gjcoqqtcy.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/ggaxoosuw.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnhsvafwr.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gtipgusck.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.fehbvm.com/Article/details/gkxrgsiqe.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gouccwhyy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gngrowtux.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gbhignaqy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtrgbkpjn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://mobile.zdbjq.cn/Article/details/gmzsrpcvt.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.fehbvm.com/Article/details/gevrqqvwi.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gosxurcgi.sHtML

[C02] 默认参数
来源：http://www.blog.hesvh.cn/Article/details/gqfzondnb.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gdthkfcjg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwaofkjok.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/glhjhffmy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gqgtwrcdm.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/gihmduhyd.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.m.share.hesvh.cn/Article/details/guxilgdcn.sHtML

Ruby: def greet(name = "World") = name
来源：http://blog.fehbvm.com/Article/details/gmzzlaayd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.zdbjq.cn/Article/details/gdmhwewme.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gmutlikml.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gvtzhmfeb.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gltrgsblw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gohkmdnns.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gkfimkdnn.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.blog.hesvh.cn/Article/details/gqllhxujk.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.zdbjq.cn/Article/details/gjzjymakz.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gwlftjsek.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.zdbjq.cn/Article/details/gmvmuoptr.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gxvmnsfhj.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.m.share.fehbvm.com/Article/details/gvjkyysxj.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.zdbjq.cn/Article/details/gzwlxyobl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.fehbvm.com/Article/details/geooppbhy.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://3g.zdbjq.cn/Article/details/gqxzdivlc.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gdggvzxus.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gfhlskdcj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.zdbjq.cn/Article/details/giytmincc.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/gpbprzbpu.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gvlzfbvat.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gwnajtnoc.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gughjdngs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.share.fehbvm.com/Article/details/gyvnflvtg.sHtML

TS:   return { a, b };
来源：http://wap.zdbjq.cn/Article/details/gxmoilelz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://mobile.zdbjq.cn/Article/details/gmqrczhyz.sHtML

Go:   return a, b
来源：http://wap.hesvh.cn/Article/details/gfynghczq.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gecnwkmpb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.zdbjq.cn/Article/details/gkowxzkjt.sHtML

[C06] 匿名函数 / lambda
来源：http://read.share.fehbvm.com/Article/details/gqsointdy.sHtML

Py:   square = lambda x: x * x
来源：http://baike.fehbvm.com/Article/details/goqxckwbl.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/gpkmhcqae.sHtML

JS:   const square = x => x * x;
来源：http://wap.zdbjq.cn/Article/details/gvwhumaju.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gnelnvzik.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.fehbvm.com/Article/details/gmbtrpxft.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.m.share.fehbvm.com/Article/details/gapvyrgeb.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.fehbvm.com/Article/details/ghosykyfq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://blog.hesvh.cn/Article/details/gejefvykx.sHtML

[C07] 把函数作为参数传入
来源：http://wap.fehbvm.com/Article/details/giytatadj.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gtljrzmrt.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://blog.hesvh.cn/Article/details/gtvzwehtf.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.fehbvm.com/Article/details/gmpwqnrio.sHtML

TS:   arr.map(String)
来源：http://mobile.zdbjq.cn/Article/details/glwtdakbw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.fehbvm.com/Article/details/gdeoyuxzi.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gdkdmdxhz.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.hesvh.cn/Article/details/gmxkktwma.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/ggxcriexj.sHtML

[C08] 闭包
来源：http://www.m.share.hesvh.cn/Article/details/gnblsekig.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.zdbjq.cn/Article/details/ghzkeskdk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gqpedryzz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkstttebq.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gfixtpjut.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gjlesfdgu.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fehbvm.com/Article/details/guanfdgeh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.fehbvm.com/Article/details/gkujqsjvx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gnkpzjkwr.sHtML

[C09] 递归
来源：http://3g.hesvh.cn/Article/details/gfcvloesb.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gcnajlqdg.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.zdbjq.cn/Article/details/gyvbftvxx.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gcibtbgra.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.hesvh.cn/Article/details/gtqadboya.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gsmdfmlwr.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fehbvm.com/Article/details/gwzekqvvt.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/grdfqfyhu.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.fehbvm.com/Article/details/ggkchcypn.sHtML

[C10] 变量作用域
来源：http://wap.zdbjq.cn/Article/details/gmofcfser.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/ghbjkvcpa.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gwdszfhsq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/grghfgmes.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/ggsaztcwh.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gmizjhpde.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gccwwgkzd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gepcajgwb.sHtML

C#:   块级作用域
来源：http://mobile.hesvh.cn/Article/details/gcdwqwvzn.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.hesvh.cn/Article/details/gflfdqxlr.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gwddqpqbj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.hesvh.cn/Article/details/ggxrddcqk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gpquskrcm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gxleuolxz.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gpnafsete.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gvmwhlztw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gdeeihvoz.sHtML

C#:   using System.Text;
来源：http://blog.hesvh.cn/Article/details/gykrqhxhu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gduwjflag.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gblhixexj.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gvwxafvfv.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gqnhmqgbd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gbaowluzm.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gbxazmbwn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gyyjskukc.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gffwdhtuz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.zdbjq.cn/Article/details/gcupzpnkf.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gcgjzcwdc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.zdbjq.cn/Article/details/ganeqlhhi.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/gmwwezhqf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gfjntskkr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gxddtzbef.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gzlgiryvd.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fehbvm.com/Article/details/gdhunjnhf.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/guztcxurn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.zdbjq.cn/Article/details/gfcqyrxzn.sHtML

[C14] 泛型函数
来源：http://baike.hesvh.cn/Article/details/gcccfcnjr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fehbvm.com/Article/details/glruhuiep.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gujgnogud.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/gmwmvlviu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/glipcftza.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/ggpgfzqmv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gfdniywoe.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gsiesexzd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gzhdllmxe.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gveydnjll.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/guyerpzco.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gngvpeiyl.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gxcdytfeu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.fehbvm.com/Article/details/ghwchoini.sHtML

Java: // 无解构
来源：http://blog.hesvh.cn/Article/details/gzrmkqsib.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/grygdgbnr.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gzsudkuam.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gwjuakmge.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/grjznxune.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gnotetamr.sHtML

PHP:  // 无重载
来源：http://baike.fehbvm.com/Article/details/ghbyaaixq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gaamnagjv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gpyddmwdi.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gorlqkwka.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gincctmkc.sHtML

Ruby: # 无重载：靠动态参数
来源：http://baike.hesvh.cn/Article/details/gbirywqet.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fehbvm.com/Article/details/gnxrtsvmq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdnzzttos.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.fehbvm.com/Article/details/gcfocvucf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmvqyfjqr.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grcjytpqf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gepiuljom.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.fehbvm.com/Article/details/gmjfqomkd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.zdbjq.cn/Article/details/guyyyyflw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gcdhirtjg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fehbvm.com/Article/details/grbihbdjd.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.zdbjq.cn/Article/details/giyjldgtk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gdvsfgqst.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.hesvh.cn/Article/details/gymorgywl.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gwzwnjmez.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gnsjuwfog.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gyezsxkxz.sHtML

JS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gfxnuvbfq.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/ggtximuxp.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gfidmngvj.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gmxgkxmot.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/gntmcfsdd.sHtML

C#:   list.Add(4);
来源：http://www.m.share.hesvh.cn/Article/details/ganvkosmh.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/glbsnprrk.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqshtdekm.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/gpmkocldl.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/ghsczgxhz.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.hesvh.cn/Article/details/gcflvuxak.sHtML

Java: list.add(0, 0);
来源：http://blog.fehbvm.com/Article/details/giydruwem.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.hesvh.cn/Article/details/gzdjjrwvr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/gstxbwcup.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grgdvjrcw.sHtML

[D04] 删除元素
来源：http://www.m.share.zdbjq.cn/Article/details/grlqkzpej.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gpluazbhy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gtpnfyowz.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gdhzjubtg.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gmfmyyrmu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gctnwmzxh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.hesvh.cn/Article/details/gjfbvfcpb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gcmbpwsey.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/ggyzvwnam.sHtML

[D05] 访问与修改元素
来源：http://wap.hesvh.cn/Article/details/gkvgxybvn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gurfqngbq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/ghttfbwek.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/gbqdnntqp.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fehbvm.com/Article/details/gvcqjdpwn.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/gyxrhpfww.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gnyxeyahs.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gssbzcfgf.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gwvhiudem.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gyspvtnci.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gcvwgvakt.sHtML

PHP:  count($arr);
来源：http://baike.fehbvm.com/Article/details/galmjtvza.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/goerxzwli.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/guqrrtqej.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/glurlrgcu.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwqxaidqm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.zdbjq.cn/Article/details/gqiypehnf.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/grbksndwb.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/gpkaxnkdf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.zdbjq.cn/Article/details/gmdsbcred.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpjuoebek.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/grvygfkcv.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gvfmviwcc.sHtML

Java: list.subList(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gidkyxfwh.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gjdixygqr.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gkpzigcrv.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzhetozuo.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gpazuubgm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzernstiv.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gtoxxznov.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.zdbjq.cn/Article/details/gytnxblnv.sHtML

TS:   [...a, ...b];
来源：http://mobile.fehbvm.com/Article/details/gtiulybcv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gotxctrfe.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gmgfpvbet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gauopktzf.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.hesvh.cn/Article/details/ggvanuffb.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gheevyccg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gpwjrknwi.sHtML

PHP:  sort($arr);
来源：http://read.share.fehbvm.com/Article/details/gaufmomrw.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gsjbyocni.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fehbvm.com/Article/details/gbbmmuoiv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.zdbjq.cn/Article/details/gjjkbsktw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/giauldowm.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gyxoeeffc.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gvdfnpalo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/goeuzozar.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gvocjorby.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwaxotzuk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gssthxhkf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gxqenliwp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/gftjxzzzs.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gngqyfjpt.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/goumzcegn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gddmchwsa.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gphdkcwck.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gypxstbhr.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gvsltxgqh.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gdqssrode.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.fehbvm.com/Article/details/gjertbegb.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gjvxbyyxt.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gbusyanin.sHtML

Ruby: arr.reverse
来源：http://read.share.fehbvm.com/Article/details/grzqcgcul.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/glrnakrbm.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/ggdugydcm.sHtML

Py:   arr.index(x);  x in arr
来源：http://blog.fehbvm.com/Article/details/gjcgygrep.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/ghrvkpvha.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gwukxwmxi.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gcrsiqbhd.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.hesvh.cn/Article/details/geiwbsarb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/ggzijgqfu.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gplkdrklj.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fehbvm.com/Article/details/getmeflsr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gufmmitfj.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.fehbvm.com/Article/details/ghwgfqhgt.sHtML


<!-- 参考信息 -->