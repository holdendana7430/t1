代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.fehbvm.com/Article/details/gsozpaitt.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.blog.hesvh.cn/Article/details/gdtzqhdgj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gcuffjpcj.sHtML

[B12] 跳出多层循环
来源：http://www.blog.fehbvm.com/Article/details/gvcyrvjyo.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.zdbjq.cn/Article/details/gobvedupn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.m.share.zdbjq.cn/Article/details/gzcwslmvd.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/geljzfqpk.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gtctbecfu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.hesvh.cn/Article/details/gkozlvzop.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.zdbjq.cn/Article/details/gwzhfcfdy.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.hesvh.cn/Article/details/gbyeqszrs.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://m.share.hesvh.cn/Article/details/gbyhihjja.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gzaufefmj.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.fehbvm.com/Article/details/gybwlqwnt.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/gltinduqr.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/glrwgwgke.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://baike.zdbjq.cn/Article/details/gttjzyuyb.sHtML

Java: x instanceof Number
来源：http://wap.fehbvm.com/Article/details/gdveknkxg.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.hesvh.cn/Article/details/gggeutylf.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.hesvh.cn/Article/details/gqgyiqmon.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gqzkozqlc.sHtML

[B14] 判断值是否在集合内
来源：http://baike.fehbvm.com/Article/details/gsiimlpht.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gyynvsquo.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://read.share.zdbjq.cn/Article/details/gmqvsprin.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.share.fehbvm.com/Article/details/grttlxacj.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gztuxbjgu.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/gqgritzid.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.hesvh.cn/Article/details/gusihdzvv.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gjutfvqxx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gryauyfkd.sHtML

[B15] 布尔运算与取反
来源：http://wap.fehbvm.com/Article/details/gchoaznol.sHtML

Py:   a and b or not c
来源：http://www.share.zdbjq.cn/Article/details/ggxcqvznq.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.zdbjq.cn/Article/details/giucdvfdz.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gpoohcxhj.sHtML

TS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gpcndcdze.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gcvokqaki.sHtML

Go:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gicxufpwr.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gkyfyhstl.sHtML

C#:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gmgzglvme.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://wap.fehbvm.com/Article/details/giijehhdc.sHtML

Py:   if not data: return
来源：http://wap.zdbjq.cn/Article/details/gffsnzmij.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/goddjxlfa.sHtML

JS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gnssoozno.sHtML

TS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gzyudyfbn.sHtML

Java: if (data == null) return;
来源：http://read.share.hesvh.cn/Article/details/gevusqcwo.sHtML

Go:   if data == nil { return }
来源：http://wap.hesvh.cn/Article/details/gjdhpvfhe.sHtML

Ruby: return if data.nil?
来源：http://m.share.fehbvm.com/Article/details/grmqiayam.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqvmavaf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gahwlkxep.sHtML

C. 函数与作用域
来源：http://www.blog.fehbvm.com/Article/details/gznpwlkmm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gpnosakke.sHtML

[C01] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gzxxrvpps.sHtML

Py:   def add(a, b): return a + b
来源：http://m.share.zdbjq.cn/Article/details/gvxwdvfsm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gndvlybys.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/goixoodpr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gtipobizc.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmgbizuev.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.zdbjq.cn/Article/details/gucqrqepa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://blog.fehbvm.com/Article/details/gcekhbach.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/ghbeprmzj.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gukumnfrs.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.zdbjq.cn/Article/details/gcthtsnxs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gjrdzixdq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gllwnqsxo.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gzaacysdc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.fehbvm.com/Article/details/gxxycjtmq.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.zdbjq.cn/Article/details/gubvbwcuu.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.fehbvm.com/Article/details/gqxicrpgl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.hesvh.cn/Article/details/geqgsudrq.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gafyxebyy.sHtML

Py:   def total(*args): return sum(args)
来源：http://wap.zdbjq.cn/Article/details/gsrzcpxwe.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.m.share.zdbjq.cn/Article/details/glynywkai.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gugivlvsi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/gwvmzpeup.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gbnfvygkm.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gkzonfgfg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.blog.zdbjq.cn/Article/details/gqawebykw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gpootzbhh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gbrtovxip.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.hesvh.cn/Article/details/gjqixlnqz.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.hesvh.cn/Article/details/gfhidhtbw.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gwirrktmt.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gmrbecvlo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.hesvh.cn/Article/details/gewnuyjwn.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gamrbpacv.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gkxrvulxu.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gzttiplqm.sHtML

[C05] 返回多个值
来源：http://read.share.zdbjq.cn/Article/details/gxmsmtags.sHtML

Py:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/giuzorzog.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gqjoapfyt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gaynzdgvy.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/gshflbngu.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gzuptjxbo.sHtML

Go:   return a, b
来源：http://3g.fehbvm.com/Article/details/gkvbqnbog.sHtML

Ruby: return a, b
来源：http://blog.zdbjq.cn/Article/details/gpmzbjsmr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://baike.zdbjq.cn/Article/details/gfdjpaiql.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.hesvh.cn/Article/details/gdkzlzbcf.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.hesvh.cn/Article/details/guvomxfln.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.zdbjq.cn/Article/details/ggppjbdto.sHtML

JS:   const square = x => x * x;
来源：http://3g.fehbvm.com/Article/details/gxytuidxw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.fehbvm.com/Article/details/guergotjq.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/giwroxifh.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gxkeahocv.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.share.fehbvm.com/Article/details/gopnmunno.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gpllzqoqj.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/gulmypsjr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://wap.hesvh.cn/Article/details/gdscnahvb.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.zdbjq.cn/Article/details/ggxhsncgv.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.zdbjq.cn/Article/details/gdovfkbbz.sHtML

TS:   arr.map(String)
来源：http://read.share.fehbvm.com/Article/details/gdybwqmrw.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.hesvh.cn/Article/details/gomjvfasg.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/gadjrpzdp.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/grunnygfl.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.zdbjq.cn/Article/details/gpzozrggh.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gwljswlzi.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gerncabcx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://m.share.fehbvm.com/Article/details/gmwhwahqq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gryutsqds.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.hesvh.cn/Article/details/grszxyujs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://m.share.zdbjq.cn/Article/details/gfuyiqixt.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.fehbvm.com/Article/details/gajyhugfs.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gqyfftksk.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.share.zdbjq.cn/Article/details/gjomprkvr.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gsmfiftzd.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gmrfkzltl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gbgdsryiu.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gumvsovib.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/grdvdkpwr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gpdmdeeog.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gxtqowgoq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fehbvm.com/Article/details/ghlhpjefr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fehbvm.com/Article/details/gwviuqhco.sHtML

[C10] 变量作用域
来源：http://m.share.fehbvm.com/Article/details/gdsqcbdna.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gnsyworwm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gledcfrdj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.zdbjq.cn/Article/details/gnkyposgi.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gosgdgkhe.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gzjnkhkkl.sHtML

Go:   花括号块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gptlnmpai.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.zdbjq.cn/Article/details/ggshhqndh.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gbosojgql.sHtML

[C11] 模块导入与导出
来源：http://www.blog.zdbjq.cn/Article/details/gmedagslo.sHtML

Py:   from module import func
来源：http://3g.fehbvm.com/Article/details/ghfhlwfne.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/gskivpahp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.zdbjq.cn/Article/details/gohgkpjbw.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.m.share.fehbvm.com/Article/details/gapjhqpar.sHtML

Java: import java.util.List;
来源：http://read.share.hesvh.cn/Article/details/gbafphxuf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/gexwzgijv.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/ghzejrpil.sHtML

C#:   using System.Text;
来源：http://www.m.share.hesvh.cn/Article/details/gzimvksug.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.hesvh.cn/Article/details/gqswokugb.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.hesvh.cn/Article/details/gjbglnrij.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gltfspuqq.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/geialcisc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.fehbvm.com/Article/details/gliibrjgv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.zdbjq.cn/Article/details/gkyvpjoqy.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gpwwglqct.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gvjymbxxt.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.zdbjq.cn/Article/details/gegcaffvo.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.hesvh.cn/Article/details/gsstfcjsg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gmdgxzwwc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/gaexweovi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gbauodlii.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gdhvorupg.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gfwbbwqgn.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gnotavgcx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gvyuxzvvg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gkpdfizlw.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/ggmhdzfub.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gfbulrkkk.sHtML

PHP:  // 无泛型
来源：http://mobile.zdbjq.cn/Article/details/guffzbkip.sHtML

JS:   // 无泛型
来源：http://www.blog.hesvh.cn/Article/details/gzdhdpfcu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/guyojupph.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/gsrrgxqip.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gzqduuqfm.sHtML

Ruby: # 无泛型
来源：http://www.share.fehbvm.com/Article/details/guobqkpsz.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.hesvh.cn/Article/details/gnedhdxdc.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gvcvmdfhl.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.fehbvm.com/Article/details/gxbujdhho.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/gacbjqitn.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gnlrjhdcd.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/goopbhcew.sHtML

Java: // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gjsejjxwg.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gdkgbtekt.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gkklurzyi.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gvqvuvirf.sHtML

[C16] 函数 / 方法重载
来源：http://m.share.zdbjq.cn/Article/details/gbvinkjfp.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gjygsjkkb.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/ggicgdfcd.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gswhuxqqx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gzmuxriny.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gqxzpgvgv.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fehbvm.com/Article/details/gmtjknceq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gyfduieqk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gkwccsptr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gekuzhwcg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.hesvh.cn/Article/details/gtgyjojpz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geuahylqz.sHtML

[D01] 创建数组 / 列表
来源：http://baike.hesvh.cn/Article/details/gbtpvavod.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gzenvncln.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gabhtdhkw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqzolqqxn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gpaemzpew.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gedoznkzs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gvqfzccaa.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fehbvm.com/Article/details/gfhmpkula.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.zdbjq.cn/Article/details/gyqjrozav.sHtML

[D02] 追加元素到末尾
来源：http://blog.fehbvm.com/Article/details/gxqccybbd.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.zdbjq.cn/Article/details/gldazolkz.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/gxgsazhlz.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gdsroilvc.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gdbpqmgnl.sHtML

Java: list.add(4);
来源：http://www.blog.zdbjq.cn/Article/details/gbekgbumw.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gmlojytns.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.hesvh.cn/Article/details/gefsrkhrd.sHtML

C#:   list.Add(4);
来源：http://3g.zdbjq.cn/Article/details/gqdjcwppi.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fehbvm.com/Article/details/grwsxunwq.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.zdbjq.cn/Article/details/gwvwuqziw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/grbltanxu.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gknjfiosj.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gpszynthh.sHtML

Java: list.add(0, 0);
来源：http://3g.zdbjq.cn/Article/details/gdbsuzevd.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjdtenbsf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.zdbjq.cn/Article/details/gpeetasly.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gmgqkmmux.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gnndewfzq.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gcohduuno.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gyuiftxyw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gkopgvfkm.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gjnklhqrj.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.fehbvm.com/Article/details/gwxkchdly.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gtysaihuh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.zdbjq.cn/Article/details/gohvbmyqu.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gygjkemcs.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/ghsteugjx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gotdnducv.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gbjcpkhxt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/goteffgtj.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.fehbvm.com/Article/details/gekrubszp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gfrcewcbi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gebpxdptk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gqbnnacpp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gttzmkfil.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gbfdmvlpl.sHtML

Py:   len(arr)
来源：http://baike.fehbvm.com/Article/details/gnlpobpqx.sHtML

PHP:  count($arr);
来源：http://3g.zdbjq.cn/Article/details/gcfaljchq.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gzvttpsow.sHtML

TS:   arr.length
来源：http://blog.zdbjq.cn/Article/details/gwldzdcrs.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gfwgvupph.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvosgdous.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.hesvh.cn/Article/details/geqlortlm.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/giobefpww.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.hesvh.cn/Article/details/gmhvclyzr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gfmtojbtp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.zdbjq.cn/Article/details/gdonmocwq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gbufjdpti.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gunmjwdta.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gfjxdhkhn.sHtML

Go:   arr[1:4]
来源：http://blog.fehbvm.com/Article/details/goxdizhhg.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gzvoulqaj.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/geiyowxnr.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/giqkfkonc.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/guzzhmoma.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.zdbjq.cn/Article/details/gfqmpbfwg.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gdugqbnyw.sHtML

TS:   [...a, ...b];
来源：http://baike.zdbjq.cn/Article/details/gndpuwshn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/glqlxnyjf.sHtML

Go:   append(a, b...)
来源：http://www.share.hesvh.cn/Article/details/gizpecpjt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gpzctlnrj.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gvgvqhrzq.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/gpfeqjebx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/geczingpp.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gulubxitm.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gkhbegsfa.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/grvdtlsdn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/guamlsubd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gegmbnmrt.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gyuopjhht.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gedbaxckq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.zdbjq.cn/Article/details/gwzhpznwu.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/ghcktjivh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fehbvm.com/Article/details/gfzyonjue.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gohzcttmc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gundgwvwe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gpcusijgu.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gslqcbttn.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/ghojophnb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/gmmgfyxpf.sHtML

[D11] 反转数组
来源：http://www.share.hesvh.cn/Article/details/grtfuhdfi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/grdkqwlrp.sHtML

PHP:  array_reverse($arr);
来源：http://blog.hesvh.cn/Article/details/gisyelgih.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fehbvm.com/Article/details/gbmxzjoox.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gszohugvp.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/gmvmsrgjt.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gzvqpgamk.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/ggbxacmkq.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gxfmavezq.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gksfxuhzx.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/grysyznkw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gggtccamm.sHtML


<!-- 参考信息 -->