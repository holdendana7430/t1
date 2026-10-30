代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijqfshtx.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fanxiaobao.xyz/Article/details/gynghztax.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gkrqtdqxn.sHtML

[B12] 跳出多层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdpflpad.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.fanxiaobao.xyz/Article/details/gryeoosfr.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoazaymy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdhbgiww.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://3g.fanxiaobao.xyz/Article/details/gssupmqqh.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoxftykb.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqcwgihd.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://m.share.fanxiaobao.xyz/Article/details/gygzqsqud.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrgdobzs.sHtML

[B13] 判断是否为数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaewwcuu.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gornspfgy.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjipbjpe.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fanxiaobao.xyz/Article/details/guqiffeez.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwnotpad.sHtML

Java: x instanceof Number
来源：http://baike.fanxiaobao.xyz/Article/details/gbfgswvcm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.fanxiaobao.xyz/Article/details/grprymksn.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/gznoegvpi.sHtML

C#:   x is int or double or decimal
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhmyseze.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fanxiaobao.xyz/Article/details/gruspyvmv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwrvsiug.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvtyrgdu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedqqgwda.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvnoaujm.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwmjcklf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpttpfsia.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gqtbrtdwv.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glbltehrx.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fanxiaobao.xyz/Article/details/gpnjcklup.sHtML

Py:   a and b or not c
来源：http://m.share.fanxiaobao.xyz/Article/details/gtaqrconm.sHtML

PHP:  $a && $b || !$c
来源：http://3g.fanxiaobao.xyz/Article/details/gbsnhbgfq.sHtML

JS:   a && b || !c
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpdbgdjk.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/giykobesp.sHtML

Java: a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmoqoxytb.sHtML

Go:   a && b || !c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbbwhznv.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gewydboek.sHtML

C#:   a && b || !c
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyneinfz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpemdjbu.sHtML

Py:   if not data: return
来源：http://wap.fanxiaobao.xyz/Article/details/gvoshkmjv.sHtML

PHP:  if (!$data) { return; }
来源：http://3g.fanxiaobao.xyz/Article/details/giyvxiily.sHtML

JS:   if (!data) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmirhvdja.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gjskwjqxf.sHtML

Java: if (data == null) return;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcitvjdve.sHtML

Go:   if data == nil { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvwgmwdq.sHtML

Ruby: return if data.nil?
来源：http://3g.fanxiaobao.xyz/Article/details/gljzrixzt.sHtML

C#:   if (data == null) return;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdjbhdaa.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzfhgvyvp.sHtML

C. 函数与作用域
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjagiwzi.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/goxeocbqp.sHtML

[C01] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxzmffyv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fanxiaobao.xyz/Article/details/gwdcqpndx.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzkjgcij.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmboidjjp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/grlkgwdky.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/giclozsio.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcdrpntx.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gykvgppyu.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gqprrflry.sHtML

[C02] 默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdtgarzr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpahssbh.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggnkjqehn.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/glbxhqxhh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guksffsxo.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjklzsli.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/goovxjvnz.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.fanxiaobao.xyz/Article/details/glzbfgxnh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgtujkod.sHtML

[C03] 可变参数
来源：http://wap.fanxiaobao.xyz/Article/details/ggystorsl.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqviijss.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.fanxiaobao.xyz/Article/details/geqewemes.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcicxwpaf.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikjrwtpy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtddgocga.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.fanxiaobao.xyz/Article/details/gyiyypunw.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfzoxpdy.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fanxiaobao.xyz/Article/details/gonhqhzsi.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fanxiaobao.xyz/Article/details/gvtazipmz.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fanxiaobao.xyz/Article/details/govxzgmwe.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmawycmpr.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gslssyhva.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gkzwuwrad.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdnstvpd.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhfyvzsi.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gfneuxbgu.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/grzewzjgg.sHtML

[C05] 返回多个值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxfhiapz.sHtML

Py:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/goammayos.sHtML

PHP:  return [$a, $b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gxawdaxpg.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkutxmnw.sHtML

TS:   return { a, b };
来源：http://read.share.fanxiaobao.xyz/Article/details/getrnsfza.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.fanxiaobao.xyz/Article/details/gbxbmqgev.sHtML

Go:   return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzchshbn.sHtML

Ruby: return a, b
来源：http://www.share.fanxiaobao.xyz/Article/details/gidresfvw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://3g.fanxiaobao.xyz/Article/details/goibxaqhe.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gtwaguhke.sHtML

Py:   square = lambda x: x * x
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcyuvuli.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://baike.fanxiaobao.xyz/Article/details/grjjrljfx.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwilyuoz.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fanxiaobao.xyz/Article/details/gykvhycot.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmfpoexw.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqkyzwbw.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghadttjhd.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.fanxiaobao.xyz/Article/details/gufcvfqfh.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fanxiaobao.xyz/Article/details/gtucwyvby.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjqnjmjb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznwllwsc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwburwyq.sHtML

TS:   arr.map(String)
来源：http://read.share.fanxiaobao.xyz/Article/details/gixuyughs.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gitsomfej.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.share.fanxiaobao.xyz/Article/details/glssbpqpg.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gizibnusc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.fanxiaobao.xyz/Article/details/gcpolprkf.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjuwftuv.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/gctfebweb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtomxmupn.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gorsmegha.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glwadfaqm.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbriyubo.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjujzrmd.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fanxiaobao.xyz/Article/details/gqqqokttu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjosjjyei.sHtML

[C09] 递归
来源：http://baike.fanxiaobao.xyz/Article/details/gzxzfewme.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqkdmxnl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gyevqhudv.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoelvtqs.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gvdismpwe.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.fanxiaobao.xyz/Article/details/gwttwehar.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxwqagpb.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvudehtc.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fanxiaobao.xyz/Article/details/gajrinctu.sHtML

[C10] 变量作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqbtvusj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytjbtlv.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fanxiaobao.xyz/Article/details/gxwgoqydt.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsvstxly.sHtML

TS:   同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaswgawwd.sHtML

Java: 方法内为块级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/gamvtvljz.sHtML

Go:   花括号块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gyoevbspo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fanxiaobao.xyz/Article/details/guoqinlef.sHtML

C#:   块级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyfidcvu.sHtML

[C11] 模块导入与导出
来源：http://3g.fanxiaobao.xyz/Article/details/gzcsyxueh.sHtML

Py:   from module import func
来源：http://wap.fanxiaobao.xyz/Article/details/gtqmayixf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/givzqwmnh.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.fanxiaobao.xyz/Article/details/gnyhtrrdq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsiwuqnzu.sHtML

Java: import java.util.List;
来源：http://3g.fanxiaobao.xyz/Article/details/glbtyjbud.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxfevdji.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gsmlysvtg.sHtML

C#:   using System.Text;
来源：http://wap.fanxiaobao.xyz/Article/details/gjbuzlcww.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.fanxiaobao.xyz/Article/details/gfnpzfjlx.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeaxckbg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.fanxiaobao.xyz/Article/details/ghphkcmhe.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbitenip.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.fanxiaobao.xyz/Article/details/geqzhxxyz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgufjrlv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giydwesjj.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqrnlahz.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdtrsknsj.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fanxiaobao.xyz/Article/details/goxhuqdoq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fanxiaobao.xyz/Article/details/gqbvqptlt.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwzlmjodz.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gmwbvhldi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gimjqcdgn.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxwcojng.sHtML

Go:   func add(a, b int) int
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktmedcbg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhoclony.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxlehvi.sHtML

[C14] 泛型函数
来源：http://wap.fanxiaobao.xyz/Article/details/gxsbrnyst.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmodblodq.sHtML

PHP:  // 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajbhooax.sHtML

JS:   // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gwckiliut.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/giliyfyal.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fanxiaobao.xyz/Article/details/gtpwbviij.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/glyzhwfkj.sHtML

Ruby: # 无泛型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmyioxdps.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gulhhowcq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgelzksf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fanxiaobao.xyz/Article/details/ghvuenlqh.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fanxiaobao.xyz/Article/details/gflwpthhh.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gilreibdt.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gmrmejiwr.sHtML

Java: // 无解构
来源：http://wap.fanxiaobao.xyz/Article/details/gsylnomtv.sHtML

Go:   // 无解构
来源：http://mobile.fanxiaobao.xyz/Article/details/goaykttrz.sHtML

Ruby: a, b = pair
来源：http://blog.fanxiaobao.xyz/Article/details/gvwqlvrws.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fanxiaobao.xyz/Article/details/gplnrjtvy.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecrsohrv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtbuggqx.sHtML

PHP:  // 无重载
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giuandgqm.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrhmvoze.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/gptvjqudc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gzsninviq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlfwqhzv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcdnuoar.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gyoazsbfp.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gvmsukvjo.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fanxiaobao.xyz/Article/details/gtanjavxl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gxsbhvqdm.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdmfycdk.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmzirtbv.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gviskebkn.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.fanxiaobao.xyz/Article/details/ggoclfqir.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskttxkln.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fanxiaobao.xyz/Article/details/ggnjuqdeq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfwdvbll.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzzrqyts.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/gnhhkfspx.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilvhqoto.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fanxiaobao.xyz/Article/details/gdjycdgfh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/grkdkpcxx.sHtML

JS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gclbvtvch.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/guvqteict.sHtML

Java: list.add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/geodjwlof.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqdwmlpm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/grjpuqvvk.sHtML

C#:   list.Add(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gksrqnzud.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvuvrekt.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gwioqlznb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksuheeit.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fanxiaobao.xyz/Article/details/glckalaeu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfhvfkzu.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gmwyywpos.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqfpmdh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fanxiaobao.xyz/Article/details/gvgorilsf.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/ggmcaebon.sHtML

[D04] 删除元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytwdwydj.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/grbwtnxty.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaebdljah.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fanxiaobao.xyz/Article/details/gmfsedvop.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqeptzru.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gczpohgku.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gsfhghubm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzkhmpgej.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gsqicawad.sHtML

[D05] 访问与修改元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gurvdgtdl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqsonxnq.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/ghkkgltqt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/gnkhmngrh.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fanxiaobao.xyz/Article/details/gifolvxgs.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fanxiaobao.xyz/Article/details/grbnjaemw.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gzxeburzz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/ghkhqnlaw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gglznifun.sHtML

[D06] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcclphwgk.sHtML

Py:   len(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gfmucogfh.sHtML

PHP:  count($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gfaeaebzh.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gphvbebss.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaayuoxqz.sHtML

Java: list.size();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkfaxojm.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxnlwctf.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gtzubdzka.sHtML

C#:   list.Count;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxvpljcc.sHtML

[D07] 切片 / 取子数组
来源：http://wap.fanxiaobao.xyz/Article/details/ghsshnjai.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgjzouks.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gptfcnjbh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gamzvbifl.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gxuznucmq.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxwymyks.sHtML

Go:   arr[1:4]
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxsndsz.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gpfdwagmw.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gyvyvkatv.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmjwzucu.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gppvoayck.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fanxiaobao.xyz/Article/details/gpdtaoizz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxohmxen.sHtML

TS:   [...a, ...b];
来源：http://baike.fanxiaobao.xyz/Article/details/gqafhptcy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gvvbdkifq.sHtML

Go:   append(a, b...)
来源：http://blog.fanxiaobao.xyz/Article/details/gjfeepnhm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbosduusj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/glbadfhhx.sHtML

[D09] 排序（升序）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzdpsvqf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvqmwhgq.sHtML

PHP:  sort($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfjpxmwm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fanxiaobao.xyz/Article/details/gcckukulv.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvdxslxe.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/gyjorulkn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyctzvfiv.sHtML

Ruby: arr.sort
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmwxcuzi.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuycthsc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fanxiaobao.xyz/Article/details/gqrguhcow.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsplkyibc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuczpcyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/glkidbiiv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gijitvncn.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.fanxiaobao.xyz/Article/details/gkjfryiib.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnslwmrtl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fanxiaobao.xyz/Article/details/ggdjwveyw.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fanxiaobao.xyz/Article/details/grdclewpd.sHtML

[D11] 反转数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbahqqsd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fanxiaobao.xyz/Article/details/gldfzrids.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzovtywsv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fanxiaobao.xyz/Article/details/gdbyvzfcu.sHtML

TS:   [...arr].reverse();
来源：http://baike.fanxiaobao.xyz/Article/details/gqcnieknt.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjgchywc.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gigayftgz.sHtML

Ruby: arr.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gfiwhqyra.sHtML

C#:   list.Reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/guuhlscjj.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsfotict.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gphcjfcfj.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gokreqoec.sHtML


<!-- 参考信息 -->