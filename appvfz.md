代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hhtxuluw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lzwirtdm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2yzztljmi.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nxovfdew.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rfuomqax.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2wzuptphq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yhiysuvr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2ohpcfzzi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2faqxbzmp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vilqnxaw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tjaomwbu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2igmmcfkv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2knprrdoi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2rshsbmpf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2puhcuxxt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2jnobsndv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ixbgerpo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ihujvgos.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2taqbakqw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ndadrtuu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqohusgr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pjadzidx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2kxtweadq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zhbcahls.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2jsadevqv.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2folkffju.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlpdrjni.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kzsmptew.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2gdctkgdc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2klihkojr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tgxajkbj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2sdldrywm.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lptyrilo.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2lxuparrt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mrhktpyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2unxwzcnq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ejhozncq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vuixmwfz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2eyvhcksw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxduoku.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2quhsweup.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlawgsel.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gxrigjtk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gmfcluiv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xyvgtiuy.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gssjrvep.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ggdzpaik.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rhogdsbv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dbowlkbe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hkurgxzd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kpcdvggs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yzhxgabx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2izbmsbld.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2nqwvcsin.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fhypaifl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fwkqrmhw.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ocyisegj.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sqmiemvp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2idjvsjny.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2lqudzqfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xucnsory.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fflwtkee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhizezaq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gmtugfzy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sfthrwta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipuzvoge.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gorrsiww.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lntzxeal.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iqdpkkqq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zqgwngla.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2arrutssq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzsbihyn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hpirvsqr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2tqjwklza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwprvevs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2izuvcuii.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzyjrclw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2envteztd.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wzhujceh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rmimjkpd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2tgmybuyw.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xmmdzpgh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zpnoqteq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2xoflnvfr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xgypyfbe.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ebwnflkg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2twzagyzr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2iezbnvqx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mvgxyyrn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2tcedfopn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2qiutkrfm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hjkmgobm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tpzsqiie.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfpnxybl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2grzzpnpw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2fiotawvw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ysdrfejl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wsvjdkot.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2namhwjol.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kvgzbnju.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vschhtfi.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2juooehxl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pmcjciqo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2rqvxbkqy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2bqxvbabl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xhizfekz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ecuswhja.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2minfyuwz.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pjqtjums.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2styqwcuw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xpfsrvhj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ybkuaraq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2atjnsijr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rlnqunzg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2jsgbsbgx.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hmxwhhlz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ivylpdhf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2iyoylfgu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2nfxywlxi.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bapjcaal.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2edgamvce.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2ricyfmfu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wxihgyvr.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xkygrrqn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2arghwglm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2maedkuge.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hxfpkovv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2dtpsuzgo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfiobfsw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcuesfxi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dqottqll.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ncqiatym.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ehueyhvm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2sqzrpbgj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pttclmau.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2qilnacae.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2slvdofgi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2rkmmonlk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2yfbmonka.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ahfonzes.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2tftbflay.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2cignguuu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2zhpxasry.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yytueqtu.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bbwggyuo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2eigmhcta.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nishglux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sdlguszo.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2jtofifho.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qzvfubbr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2kckqtvfr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2qslrlvdl.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2clluhpbx.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2xkkfeqre.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2yybthmfy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2fypnaxhn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2mwknopsm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2ugfevvev.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2jknlijjd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2mwahshyh.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kkhkvdza.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2yrzbfeih.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2jtqpctib.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2aodmsvvs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2gwmynzor.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2crigplpb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mcrcmkjp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2mjamqczb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bmtfidnb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ljevwzqf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gaaaakvi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2rjdwirct.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2sapnyfoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lewyymen.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bukfbqgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rutkictk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiibrmol.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2djkqbsjm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2lvzvacnb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lxaqqzjm.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2efbvtkxk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cibrpzie.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qzdeceyd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hndbtvuc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvirgwiy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uicupzgm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2blwynbwt.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tvvjplpq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qldraaqq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2aafvhwey.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2warmttsp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kfixrkgs.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvjyvxtr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpnqmvbw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2akoomhrx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2hsgbqjyh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2wvrcmqgm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vguawliy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ktzxelsy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2eymhxchw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2httbqmoh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bsdrofkx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ipjgcoqi.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2jbrlxsaa.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2fhqasglr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vlirjamp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2giqnlapb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcaxcjfm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kfcggozt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2secqejkx.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qvfepzok.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2xqiuvvsj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2uvymyssp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zoburvar.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zpqydnue.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hwnhaugw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2czdpehfr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cgwuomkk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qtebqtmb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vnzioutd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wjurwamp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2utxovctm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2cpmgpjtg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2leskpedb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ujuvjjzo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bpkvkdkc.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2tjnueyjq.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nwnlaqea.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2tfrrsxwv.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vgjwpesp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gnlczyyj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wfnmmzpq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vonottdw.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2okayzbwr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2rfbvvfcx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jklbwtmd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bihtweok.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2ladglipe.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pxudcjph.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lsgnxdcz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2bjgjftqp.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2angdqfxx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fqrovadh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oqbpkpnm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2chcutgan.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2edgevkrj.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2kwqpltae.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nbgaelua.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2iynlywnm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2awnznriu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2zanhohqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hrdaomdd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2uiojgvyf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rmqvogea.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zugqxtae.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2yrkqgxmp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ieimbugx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yqveboci.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rfxkjyba.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzvylyjq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2khsvhoex.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxqeqps.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2cddcgikg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ykgsdwzv.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2vlzkebuh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qesoncil.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2melhuvam.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2fjxwaxub.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ctmytixl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ucfkayug.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2etqrqzvt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2eaulcbzg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jnodljzm.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2yfzmkgbx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mgxhltbv.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2rvjzojhc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2atfshjqr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2xprsxpao.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ccyjbltq.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xrywdiez.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2qjalxchz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tyjhajwr.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2peqsjvkh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wvyupflp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aglhqynt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vdmmwhly.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2omtquufi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2unqmlsmx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gtxxonaj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2iurjqgxi.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2jfqspcbw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2rnvqwyrs.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vpdiadwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2cgcnzwbj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcjisvj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xywxfsux.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2gkqerevo.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2jsluapqc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2usyowtaa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2mqpmsoha.html


<!-- 参考信息 -->