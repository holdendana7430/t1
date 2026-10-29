代发 wailian999

C#:   x is int or double or decimal
来源：http://blog.zdbjq.cn/Article/details/gcelzhmrd.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gbjdpddhw.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://blog.zdbjq.cn/Article/details/gtvydyccs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gyyuavjtw.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.hesvh.cn/Article/details/glhzqluap.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://baike.fehbvm.com/Article/details/gomazatvy.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://mobile.hesvh.cn/Article/details/gnpjpjoxx.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.fehbvm.com/Article/details/gqekprmgl.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://3g.hesvh.cn/Article/details/gzywdggxr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gakduibmr.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gzedoooiz.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/goiyolyjy.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.fehbvm.com/Article/details/gyvfqnskb.sHtML

JS:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/ghrxvgdnq.sHtML

TS:   a && b || !c
来源：http://www.blog.hesvh.cn/Article/details/gfguvnriy.sHtML

Java: a && b || !c
来源：http://m.share.fehbvm.com/Article/details/gjphwdsjo.sHtML

Go:   a && b || !c
来源：http://blog.hesvh.cn/Article/details/gukjtlymx.sHtML

Ruby: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glckqrikj.sHtML

C#:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gpdosjykt.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://baike.zdbjq.cn/Article/details/gspswdqif.sHtML

Py:   if not data: return
来源：http://blog.hesvh.cn/Article/details/gnllbpsgx.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.hesvh.cn/Article/details/gqofjothh.sHtML

JS:   if (!data) return;
来源：http://mobile.zdbjq.cn/Article/details/goujmuxtg.sHtML

TS:   if (!data) return;
来源：http://blog.fehbvm.com/Article/details/ggtnzmeym.sHtML

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/grybcwjtp.sHtML

Go:   if data == nil { return }
来源：http://blog.fehbvm.com/Article/details/goowaxtaf.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gdbowbbyb.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gjwtkuvzt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfctvkmlb.sHtML

C. 函数与作用域
来源：http://www.m.share.fehbvm.com/Article/details/gwfgguzou.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbqhwcrdq.sHtML

[C01] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gniazspns.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.zdbjq.cn/Article/details/gkczhmqbh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gersvodgm.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gywxyrhun.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gzibxlaab.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/ghlcppanh.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gierjogye.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/glwibeftc.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gymjxrdma.sHtML

[C02] 默认参数
来源：http://read.share.zdbjq.cn/Article/details/gvcqwiqxr.sHtML

Py:   def greet(name="World"): return name
来源：http://3g.hesvh.cn/Article/details/ggrssydua.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.hesvh.cn/Article/details/glwthcbfe.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gxbntlbrv.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghvwprxcp.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnruoge.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://baike.fehbvm.com/Article/details/goktwqotx.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gozjalogo.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.zdbjq.cn/Article/details/gyisjsbqu.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gtpdmsjoe.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gliskuhgs.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gjfyalsro.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://m.share.fehbvm.com/Article/details/gwjkctrxr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/glabrwzxh.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gxbymrjzx.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fehbvm.com/Article/details/gtovdznzd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.fehbvm.com/Article/details/gtetxtvhm.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/gsayyreae.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/gifkbnimr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gbznozivc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gehqbxoyf.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gvwgdmiim.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gupjaawsr.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fehbvm.com/Article/details/gnteyyvqn.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.hesvh.cn/Article/details/gojmzbddb.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.hesvh.cn/Article/details/gmofuqcad.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.hesvh.cn/Article/details/ghcjtlkcg.sHtML

[C05] 返回多个值
来源：http://3g.zdbjq.cn/Article/details/gigphvmqc.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/guetiumcq.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.zdbjq.cn/Article/details/gmwhrbwwy.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.blog.fehbvm.com/Article/details/gdsbwtzjz.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gkqgkscpt.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gwjhyohys.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gkacjfaha.sHtML

Ruby: return a, b
来源：http://wap.hesvh.cn/Article/details/gycxvokhr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gigytxyhr.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gobfmwluh.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/gnanyvlsn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gxmqwxoyy.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/ghrgiufxd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.hesvh.cn/Article/details/gxdcsczhq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.fehbvm.com/Article/details/gqednoklp.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.fehbvm.com/Article/details/gpvsvrwbm.sHtML

Ruby: square = ->(x) { x * x }
来源：http://baike.fehbvm.com/Article/details/gylzeyzrk.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gbnnrybnw.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gyzqgjcwl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.hesvh.cn/Article/details/giiutjndi.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.fehbvm.com/Article/details/gxbjvvvnt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/ggknhtfkr.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gmcipqcaw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdfoweyqc.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.fehbvm.com/Article/details/gkxweyuzl.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.hesvh.cn/Article/details/gmfqsagwo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.fehbvm.com/Article/details/gcswqtzhr.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gdjpfvram.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.hesvh.cn/Article/details/gftdrqrek.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/ghxkjfkhs.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/gqgwqkkow.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gfmjeojwa.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.zdbjq.cn/Article/details/gddkmqjvr.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/glpdfmawn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.hesvh.cn/Article/details/ganomwtkx.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gilsfhxcg.sHtML

[C09] 递归
来源：http://www.share.fehbvm.com/Article/details/gsqhrhfrp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gbsxteuvc.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fehbvm.com/Article/details/gdffeeafo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.zdbjq.cn/Article/details/gcyjclusd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.fehbvm.com/Article/details/gkshnzwfd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gimbjimve.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://m.share.zdbjq.cn/Article/details/goxtbtakf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.zdbjq.cn/Article/details/goerpcqch.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.zdbjq.cn/Article/details/gasfgfmlc.sHtML

[C10] 变量作用域
来源：http://m.share.zdbjq.cn/Article/details/gssxueslz.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://baike.zdbjq.cn/Article/details/gtwvbqdmd.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.hesvh.cn/Article/details/geirhczdf.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.fehbvm.com/Article/details/gshinovkj.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gxnoohizo.sHtML

Java: 方法内为块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gdkvhzeen.sHtML

Go:   花括号块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gdyccecyf.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.share.zdbjq.cn/Article/details/gpmynrcla.sHtML

C#:   块级作用域
来源：http://wap.zdbjq.cn/Article/details/gxmpswqzd.sHtML

[C11] 模块导入与导出
来源：http://blog.fehbvm.com/Article/details/gbraojlsw.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gakzamgof.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gbjghlhdq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gzuyjpgko.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.hesvh.cn/Article/details/gxtipiyya.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/geioneppg.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/guinqlgwr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/gcrymsyfv.sHtML

C#:   using System.Text;
来源：http://m.share.hesvh.cn/Article/details/gmshtkjxd.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.zdbjq.cn/Article/details/gjjlvewqk.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gccltgvzf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gjtvirlcs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gjwnxyxex.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gflwyvmun.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.zdbjq.cn/Article/details/ghxzodmhv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.fehbvm.com/Article/details/gzyqdoftm.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gacrjcaqf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.hesvh.cn/Article/details/gvqsttkhn.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/glxkkkdjv.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gusopbwoh.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gbbkvkebq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gsbybxwrk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gjznpdfcb.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gydzilbhy.sHtML

Go:   func add(a, b int) int
来源：http://wap.fehbvm.com/Article/details/gfihbbewk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.hesvh.cn/Article/details/gtznesfgj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gvbuiurrd.sHtML

[C14] 泛型函数
来源：http://www.blog.fehbvm.com/Article/details/gpnywzdee.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.zdbjq.cn/Article/details/gdvwpvmmm.sHtML

PHP:  // 无泛型
来源：http://www.share.zdbjq.cn/Article/details/gvwjhzkpz.sHtML

JS:   // 无泛型
来源：http://baike.zdbjq.cn/Article/details/guwtrqbfj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.hesvh.cn/Article/details/gdmbrtvhe.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gdtampoyc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gyohhyrvo.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gpckhfkak.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gheczsipe.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gfgevldnl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.zdbjq.cn/Article/details/gxucmxjkj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gcrxpdmkk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gkhvvpbzd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gxwyiyjcm.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gzelbcimg.sHtML

Go:   // 无解构
来源：http://read.share.fehbvm.com/Article/details/grmrhwvif.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gdaszwjlr.sHtML

C#:   var (a, b) = pair;
来源：http://wap.zdbjq.cn/Article/details/gctaroxmx.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gqnfutatn.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.zdbjq.cn/Article/details/gvcsbnghy.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gqzkjjyve.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gtifhsloo.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.hesvh.cn/Article/details/gcpizmdax.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtbdxxgwx.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/glmirrota.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gvzcjvbrt.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gucbhlepb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggontirii.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gixmayfgk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdhpbrrts.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gflhkgljb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gtrsdjmgj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.zdbjq.cn/Article/details/gpyvmungq.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.zdbjq.cn/Article/details/gntkidkvi.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gtysysqzq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gpvdvecet.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gevzmvgry.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.zdbjq.cn/Article/details/gcdmarrjc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.zdbjq.cn/Article/details/gywwbsnwh.sHtML

[D02] 追加元素到末尾
来源：http://read.share.fehbvm.com/Article/details/gochytikn.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gvgszydfj.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.hesvh.cn/Article/details/gjtejhydq.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gwaimhkbo.sHtML

TS:   arr.push(4);
来源：http://wap.hesvh.cn/Article/details/gpqxjbbhw.sHtML

Java: list.add(4);
来源：http://baike.fehbvm.com/Article/details/gazxwnhwq.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.zdbjq.cn/Article/details/gpysdghnm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fehbvm.com/Article/details/ggttpudmr.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gremytfrv.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.zdbjq.cn/Article/details/gilqpnexb.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fehbvm.com/Article/details/gflycazcc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.hesvh.cn/Article/details/gtcsaerpg.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gpogerjaq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/giandkwfb.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gyvanggwy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/guqpyebvh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/gdrlgdcej.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gvkbsbjtn.sHtML

[D04] 删除元素
来源：http://blog.hesvh.cn/Article/details/ggfkigeax.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gyahclrga.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gacwemjhr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fehbvm.com/Article/details/ggdgfapja.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/gbvtavqqv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.hesvh.cn/Article/details/ghwmxjfug.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gbhsjdgfy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.fehbvm.com/Article/details/gmzjgzfly.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gegmqxsgn.sHtML

[D05] 访问与修改元素
来源：http://www.share.fehbvm.com/Article/details/gohxfmwjs.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/grugesrpe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/ghnerwadw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gbiwinhat.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://m.share.zdbjq.cn/Article/details/gyazpztxl.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.share.hesvh.cn/Article/details/glrualoej.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gfnprkjsp.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gaspczrvj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fehbvm.com/Article/details/gfafrlhxl.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gqxqkeyhp.sHtML

Py:   len(arr)
来源：http://wap.hesvh.cn/Article/details/glagzxkhc.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gbjaxuugq.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gpzraoapt.sHtML

TS:   arr.length
来源：http://www.m.share.zdbjq.cn/Article/details/gpvdymwyw.sHtML

Java: list.size();
来源：http://m.share.hesvh.cn/Article/details/gmbdconpy.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gatjribif.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gfajnfvmu.sHtML

C#:   list.Count;
来源：http://blog.fehbvm.com/Article/details/gknrbuvvm.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnfbxtfga.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.zdbjq.cn/Article/details/gidaecczs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.hesvh.cn/Article/details/gpmwiwqku.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/grdfndgvj.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gwjjtikyr.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gnmrrugas.sHtML

Go:   arr[1:4]
来源：http://wap.fehbvm.com/Article/details/gnmwuphaj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gftyfzbuv.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/ghlfanajf.sHtML

[D08] 合并两个数组
来源：http://mobile.zdbjq.cn/Article/details/gybmkmhxg.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.zdbjq.cn/Article/details/gntzpppra.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gtqtjtufw.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ggtnaaakl.sHtML

TS:   [...a, ...b];
来源：http://3g.zdbjq.cn/Article/details/gxtixxwjp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gajvcjtma.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gxmiprgvy.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fehbvm.com/Article/details/gpcwgkcop.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpjstjtan.sHtML

[D09] 排序（升序）
来源：http://read.share.hesvh.cn/Article/details/gdbjcdkls.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gjfyaxiwl.sHtML

PHP:  sort($arr);
来源：http://blog.hesvh.cn/Article/details/gwciqvyyz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/geezhbnkw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gyfchkvep.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fehbvm.com/Article/details/gstmtwnsg.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gzrhzhchr.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gxrbsijjb.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gecwoewhp.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.hesvh.cn/Article/details/gdimkcwad.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gzfphexwa.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gpyalbcyr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/ghvtjyrdc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gsytkzwtd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/gdqoiclxp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gcyuuhmwm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/gmfkpooqn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gllpnukyv.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/gyaenrmfc.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gonajgwhx.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gadwvfevy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gkxijrodl.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/glsjtsujm.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/ghllhrljp.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtksusjzx.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gvtsorhkc.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gjqimmlti.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/giddcnqnd.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gxinjbrqa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gmszmrwvd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/gtlghcjbj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gygyjogxg.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.zdbjq.cn/Article/details/gkftbsegh.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gqaihvaii.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gorhfypvm.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gcwsomvar.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/gqhyfpbik.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/ggikbqlrt.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/ghqseshdf.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gfnmuckrj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gkdfkxxge.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gazxmwdxu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.zdbjq.cn/Article/details/gxmrublij.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.hesvh.cn/Article/details/gvhytizrq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqtkkyenz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gpaurzdpp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.zdbjq.cn/Article/details/gdseqzsja.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gpfsruqpo.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gxexwxzme.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/grlutyjti.sHtML


<!-- 参考信息 -->