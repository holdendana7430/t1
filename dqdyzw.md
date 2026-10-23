代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3viuwqdqy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvfyeiju.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bkopbmhx.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3crjshmkq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tiitdabs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3clasgvsk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qiillufv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3ewxxwddo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3kdqtqoge.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3jcosadkt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3glmtqaom.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3imoslgey.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3vffvngsm.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3oetswcjk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3vogcocyj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nxlpfxbi.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rgdrjbbm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yknljrno.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3zuurpitf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3prtrgcdx.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3krholaho.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3znduvrsa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivnbybiy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3gypowhst.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nekjpage.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3imhyfxvp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wshxcvsp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rhanxdhu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3esbwfkhy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ztpsjuvd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3urolrwgi.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xiyyapyl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wfoswiga.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdswijor.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3cinzlpls.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jcfcwahn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ncarfjfv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3szbrxlvb.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3lguptzlo.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3mkcyztoc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wxfhpitm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3yulziadj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tuzbgmpq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3elhjepxr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cclqqupw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qrxibyra.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aenyqekn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3bnkwollo.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3avrkwtsz.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3hizotpvg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uumeebmq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ixuwxcgz.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hpvtnzyo.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3iyvxiqcc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3yvvghfba.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3riqculiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lgvwrydd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3zhgietni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fdrebvlb.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3hpgrarwl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3reuclakg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3gvifuoak.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ddtzcdln.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrwyjwsz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mchvokrp.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3nvfusfne.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3jledvxeh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qnrscheu.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3cwviudhh.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3echpinac.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwueiyyy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lktquinw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkydpedy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3jlhnpqno.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3dpooshzb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3cduupvjl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3gqhayrce.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3cagdqbyu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3guctfezp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ypwxqxuc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ptsyzczy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgxmrqyi.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3urvbuogr.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qdskhbaz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ruusnihm.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3saxplxtu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkpihbmv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jmcknnpz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3fddfrram.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ghujgxju.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3gfargjmi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mhibeksh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hzduyiew.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ughlvwnr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulvaqybu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ywspvvwo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3huafrren.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tjcfglvb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3jqauebgo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3dupploub.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3liwqaamb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3txzkryqt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3rmqzgkty.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3knymhnwt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3chitirul.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qwsixnls.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vdeoxwke.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ibkwkiyw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3umwqrppk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kjyfkrba.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3tyrwxgbg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3cbdndekn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qdanvoqg.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vffmxopp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3swzdeumm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3hytebwup.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3rlpehxwo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cbmvcwgt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bwqngwjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3dhlzmjwy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3euzavfqc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3mccdphhq.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3snmnbqbo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3tpmfbphu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkywjiwf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tcnrstfe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rrwvfmay.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rtagbges.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lbitkdjz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ksophtdo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvyckdi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3feqndqwr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gbcruqoa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3oqflpxvz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cnqyjdaa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uubtkqls.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3smzgaubm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3hofmrxab.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bggwirft.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tycicovr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3yrucypwp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ckrhvgmv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ehsnvffl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3sratsehl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ppmhwrnt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3qlvvuhkp.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ygoczvde.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ytczksea.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mzjmizrv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mivytqdq.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3yjfmcxhk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ficufrqn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vwnoikrd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3amgqxoon.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lsjyhvqk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3bpxavazj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3tzwmqcel.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pwexybjj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3mmyjkohf.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3njtisqet.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ttbrrpmw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ufnrseyz.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnpdudpn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3ngmburqr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ejpccbdd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vklygjof.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3yhcngegf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3obeycfew.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qczznxgg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mclqrajr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mgyuvxkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aurijgyg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpfyutvr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3omchubjf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hmxwzfoz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3auvcqtnp.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3eajmihuz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3oqonuhmj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3izwvjmxg.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3quwwvctu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3osqkoghb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgarfaho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3gggnhsyv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hasadaqh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zkhpvfgb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3iqxwzynn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3csxdbvvb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bztdqtuw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwhtnejt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3cwmyzbrw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ltshmnkw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kbxuiqhc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3snshkdyx.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3luxxbknh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xfftkbik.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hwnolyky.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pndnjnyd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3dbecihss.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3oeupxqzz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lyzqqznh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oatlvvti.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3emaraqnj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xarkbowb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ibsauziv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vmpbyuze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zhnzbpdb.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3jrbkybax.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3koswsrwp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3keoisewo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jjdnffcq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3fqbcwbxx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3vkyajsdp.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3frraarpn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lteromab.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ndaxujhg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hxpqwtra.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3jqforbzt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eoeowaiw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3frzitdzs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qhpxokkz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iilbwwpe.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nqiknynb.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ozkuldlm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qntxezfk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3gwpehyms.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ydeyeprs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rfqvjcrn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rzfhlzrv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mjvvsjcj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hhnytyio.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rmmvwaig.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hmgqbsgk.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uklqgnbc.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3iilbuiyl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqfvngnz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jltpouip.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3kmoneqjp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3urqyytee.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tgdsjsgi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fmpeuxaa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3khgntovu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bwztddto.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3grzlkoea.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zbwoillg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3maeallvl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tjyjdlva.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3frezxgzw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3djpyrgtp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3mtzlqruy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ikehikum.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ziobywxs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drooluce.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rztkazni.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kcklquem.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3clisbuhj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3llhkjeig.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3lyyuvkru.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mothfure.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3vudylcgr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3urwzcqqz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3rcwpuvnh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3uczvitlc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ancwsuif.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3nuorivev.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3dwifyeym.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bvbogwzz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hksviajg.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3dvaxuwrc.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rlkkwxhn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3hljbmvnj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ftnuowvh.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qeppioai.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dbnbazwg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3oelttmjo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vafsvgff.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3afhpgtlf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yotgjzkb.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sditrxih.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3cbmwbvpu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ofagojux.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bhrbetru.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3mutgtgfi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gaxdykvd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bbnntpsr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zqnjrmbp.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3pkgcyevh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3csozbecu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3seiqyzft.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3tpjeqbgs.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cdniatnn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ptdayhii.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvatyic.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ypwubhax.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3veccxwig.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rpbggbeg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3kesnjhwj.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pprospzp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hvjwvqau.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ddunubwj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kgpsaqpy.html


<!-- 参考信息 -->