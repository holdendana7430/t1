代发 wailian999

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3irzovtmj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3kldykppj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3keejrwkm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3oiaijdrz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lgmnvfuw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3kbeitdao.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dnqyxzgw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3tvqvjdkg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3uitvuwqt.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3bvzvibat.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3mriicbzn.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xblnxfby.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rwqrrsvt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3gfwwmrxm.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rcepzqyc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ohlfvvhy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3xgsjkkio.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kuokmptr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3bllxuthi.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3mykkeuij.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3cogezicx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3exvtinxp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rvuxjkfy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3znfoezki.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xxihuoud.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3skcietbk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3anyyrqtm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3khudbpss.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3brntvyvw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3tmeszytx.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ekcghlvl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlyatzav.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pcrhhppx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tuwhqucz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vccvydoq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ypzpukxq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qrtsdeky.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kmepxpps.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3jgovnmpo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ooschvpj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jxfzdjmv.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrxuevlj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jmqbtdyz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3abysjwrw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3izcqppcf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ulvqnrug.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3jwcehclj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3asbfdsqz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cfgqlutr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ajkihqwe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ukrmeebp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ouzinhcl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lvfpisae.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hsaqriey.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3niqkzwlo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3zoqgibuw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3mhgmrbzb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhumuxup.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3glyxdogk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3exblvfhs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3txkfkaxm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fqieooae.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3afcocdjs.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rqsbjqcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kiqlyimx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jdhzeffv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3paozuiwu.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ejlpywke.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3ykzrsuok.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nbjwpjts.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyrhpzqq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ccbqdmdg.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wgpwoipq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jdnkvnls.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3emafgguy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wxijxehq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cndybhha.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bobttkoi.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhfpell.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3clhxxhmm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kinkibsn.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ekxzhrxh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3owfoifca.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hseuruao.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3bfevomyv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3subbrvpz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3gmhyfljs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3sfurtmwk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmpvelkk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3aqjshkii.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qkgogqbd.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qpjghkad.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrbzdlsq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3xqtjhrnt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3dfotwtgm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hxagbizx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3isgfnbrp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3niothxpw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3tyjwhuas.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3keeelgeh.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tqlbpcwg.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3uanszhhv.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3imdafbcg.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3flufzqac.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wwegmjce.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fskraxri.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3moxchhsv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lwyogfsr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3spnfpbop.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zafdztbm.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3fpxvugos.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vdomjizz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3buplwmtl.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3hejqfwet.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jyjflund.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lfgxsajm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ivmulyov.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yteoktki.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3gaxhftiv.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3yldfotae.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3idpvqazj.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3aiubrpfa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3lhuqflob.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dxyexjvh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3tlfdswct.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3mzppsgdq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hisynuyp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3msbhykys.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3jpsqimzo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3qnhpufbu.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qhmpsmxj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3mxkczhsg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhjucad.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvgvnpym.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3clxvxikn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3xvymlotk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ibnnphfi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nshmmrvg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jyvszznu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3logrxbpl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3oljocdpk.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bgpoabbw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3sumcllgy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qzdspoiu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hpavcgwy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxapbuxl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajjnbqez.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qkaydoch.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bxkchpvv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3efwdemek.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3pzkuswbr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bjztvhyk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nhmxjwrv.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ouepyjne.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3igdfknlk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3bweektzu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hdaxznor.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3syktpusf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3eenzgimr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zxmimqxi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nzvwmfij.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uejrqqzx.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hjwpxxyl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vboxpujc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3loopvtni.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3mtzswcfr.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3alhyhnri.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xrcqzsso.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3gtlzufrb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wmwgampc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cxjoabgt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vgfcznns.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3sczhzwxn.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3patoeyld.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zhhptvro.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3gkicrqbd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vyyywvaf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3muzbrbrj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oinepbrt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxrikibg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3teuxkjli.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3xhzhhgif.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3gbhvesys.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ustkwscl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3tnncmusi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3xpyzgdqo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hwytlafh.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3abongzhk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3dbgrvkkc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tjbiollb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3lolgebys.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3epllelci.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wvezcsam.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ptdpaerx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pwnvyqqx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3glwdaudu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svxkhrqh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cwqmkjrn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3dryabdcm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ppqmtvyj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3wizndlpy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3rgcwiwnz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3sfirzpuy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ecepaydz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3qropinwf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tbwogazy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ekersrtf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kokmknhd.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3pxgrynlw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxreankr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ukobnzpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cqnyjcsk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hrmcuwba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uxcubvvh.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3asgnswtb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3zoolnpow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3aeqjjwpf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3muwrsyku.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3baixyulg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3xgvumdnp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3aupnphba.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nvweoqrn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3srvzzcku.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vnavkirg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3frnezclx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3taaxdtrf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywmekwph.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3tkxaxear.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rvbimdvv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3amymvvqg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ncalbfjs.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rjbcpfvv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mubeojaf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tdmdzqkk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3cjhgmrkk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mwbjdebu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mgjwcgrb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qafonujb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3evwgvzqq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3mraopkfg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pspgqspz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3zsjcabmr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3epdinxww.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3hykdqsdp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3pltfqkaw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3svncdxfp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ldzivriq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3xnholbrr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fiwxvtqk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vptpzjna.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ghqzfccx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rwhfrizl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uwvwvlhw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3syqtewzw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3eipejbox.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3tblesszt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qpwfgmql.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wrbafxeg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ynipqvya.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pjwftgtb.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3eezqkpef.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3gaxsjtat.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwykkenl.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ixddtanh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3ikedcvys.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jfahmsvm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3bujhaxga.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xdldohtl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3zgxyfmdc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3doambtqq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ndlirwht.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3odpzqnfz.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jxmwgctt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jsauoxtu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nxtkyycl.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vceogmjo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xhyxojqy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3psyyixxt.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgqpkum.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3avraqsku.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3tdhqczsj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3czbmubna.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3axgjhlbn.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ivntbodd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ktbbksif.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tovftyrh.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3iazobbph.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3prawgpxt.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3tpfahnqg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3frnlxiyl.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3qldfpgoq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jskymmpy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dxxedhsk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bpxzrtch.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3eqyvsdpd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3bqzwdcso.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jxmojqtj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kiqejyhv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3eabwreiw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hgtopcpm.html


<!-- 参考信息 -->