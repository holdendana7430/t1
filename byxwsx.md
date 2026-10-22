代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2auodkifp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vjgpcgel.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2uociifpf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2qrhietqv.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2eajqpgfo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2hqestzmu.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2iibsoule.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tguqfgpo.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2cviizemj.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2khqerfca.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2flkiouwf.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2ebklossg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2cggktgvd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2adrsjdsd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kytuydhe.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2yrrmnngs.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2lpxbvijp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxtiommz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2rimotrfb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2blsohvxz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2wcnrpymr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2djbamqgl.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2fkbpqrka.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ovfzkzqi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2omakszxv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mhcrqxpr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwkogrp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2asudazbr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2hpuhpwvk.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2sxplcivd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2nizgqzig.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2arhfddrd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2vctluqvb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tkngqwzy.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2waiglhvk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnfazgo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qlcqecib.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cswqfrhl.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2keoxlmtx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wbphgbwr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zhhfnnrm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ljqgcleo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jyodiwkp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kfayvfte.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tcgxkpyo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tozmptlm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sdwpxipz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nwnyqjjk.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2xxxskzox.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngjgfamw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2mzkoucyw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jxouufas.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2firzvpah.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iagbjzmj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ptitiiiz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hqohxfil.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2obuusftx.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zjwezbwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcuwjfpr.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wwmhosjl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ryezygdu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypmemsnq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzietutn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypfyulrt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2sdsjzgkn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xscefiwf.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2nrpwecak.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rovpsgcy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2qpluzksc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2mbmhdjrr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2ueudsiar.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcffgzzt.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kvzezofm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2udxnelsx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ytcnurdf.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zncfgxpl.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqtxgokt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2nmvanaeg.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2deumqqaf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqshqcda.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2caavlbjz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2oupyljfp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2idsyedae.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2zogtjjkq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2zuckgnjg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2iuxwamrs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2izrndbsd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2trapddxo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pcktcbhr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2anillkcv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cudqtcyj.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2becpzhqj.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2xxrqpbxt.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2cqftgrvq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ughwvjvr.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ukqfaotk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eczvdqjy.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2rzbcsvrt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2izsoachi.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xptyamrr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cawclwif.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2utdgtmly.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2qyyvwkbg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ssgzkljz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2chsprudx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2tccmcpyc.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2fxycbdgu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lamqhbjj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jnidzuyo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hbhjnxuo.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ppxiiemi.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ymtssuxl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nfoutveu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2idfizafg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zjzboywn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2asnpslwk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vkjwgrdp.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oetblzug.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hssypkvw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uzztvqwd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hjxypytx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2guigfhbj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2yqiownsg.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ageqfwln.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrmevjxu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vbtfxjxg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2beukocbp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2luqrzoxl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzywwpx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2fzzzjamt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2amkrjpon.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2epumyotn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gaobvunn.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2repsjetd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2rnvnpldu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dziopqrd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2tqmjzxnb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rmuvzcdy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2btgjvrrb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vmrreeui.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wntcywqp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2jykucfep.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2fmozkzom.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qxcrgkff.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kzjrvuac.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rotzrpqw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mhzyjgfe.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2sstnvgak.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kwbhtalh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wxoiyrbv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2drzcuusx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2dbavhhbc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2gyiszkrt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2qogvjhsw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmctlhi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2werewrin.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2maxnorld.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2octnroyo.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2bwseicmw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2kdmqttda.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ylxoihgn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zsgxslnb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2lumvigrr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dnixsdvi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2unruuckh.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2qwolcoxj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2uylugwun.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qgohndva.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rptfuiqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gkoaxjys.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ykiqrdia.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fbytuqcs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lbnbtcen.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qymzosej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2sffjxicn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2aaxmrlxr.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lyntbdgj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ombawdpe.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2txyfdhie.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2qhgqcsvs.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cilcecub.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mxqamwgz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2zhffpwtm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2awuqjgrg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2hnaqrxlc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjxobvhd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lfdbarsa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nejvzdra.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mrjolwcz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2bkjjschj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uhndhfpn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2hwzbbeje.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2pjcrtajg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2yejbgkoj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dcaqacmg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jdjcohtz.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oktieytd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2enupptuv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2lwpcoqan.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2yijsdmzq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xvmxgvfj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2pysmhmtb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyfcslyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ckbuotgi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wlktszqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntdjxjoi.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2qjrxyylx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2pyqbdkxl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mofdpbfy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iwjpwtxa.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2iyrpzfqu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2bdlufwga.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2spaupder.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2fguwvlrz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lqyjcsgz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2rlgeadxy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2padakpde.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2kmtjcpmj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocffberb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xtrwvrty.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2hsfbpvdp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejuuefnq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzkvnf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2xdyrgzbn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2xszfhgam.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mexmucnp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ctppcbjh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dgjpkvbd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qzpbmekk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hyidpeha.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2igsfknwk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2mozzwxlw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2gdrfcgvz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yizxwiia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2mxpvulhx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lsncffxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2yrvukhcd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2sadadqlo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2mnnghxlf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2fdlkpgzh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2sssfydkm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2nxxmqlcj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ypoabusl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hoccapxy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2qokglimf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ndcnxtty.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2cuejgluw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2qzrzzbiw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sqjljhhk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2pwjlfyyc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tfdqyzar.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gegbkhbb.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hiuoayuc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzrzasrp.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kaypgjxo.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2izbmobpj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gwyijftl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xilgzxwe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2fpimavcq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2xuqzrfae.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2enkoynke.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2tuvknnmm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jrpuhhee.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lawwfsdr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2krjrezft.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qaoudais.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fzxfydcw.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qiixmwkn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2cmcwzqjm.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2jzowqfya.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vsvirxyi.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cgvysetv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vjmwurwc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2imbhjayn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ezmtdqhs.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2stlbrpkn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cdbhrnqv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2xdsxztev.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2otmrwzzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2elemrqqs.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rpfhhexq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2hlvcvolq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2sbaqbjvj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2pwtqfvgm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dgtfrrla.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tuufaqww.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2bbzfddpq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2mvmfrtkz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2arzsejao.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2spueczck.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dhopbkht.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qgelitga.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2pgwvqbdd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ooddtbkc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bysxkpfa.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2jnjoyoul.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2qcndqytv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2chwhanjt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2kexwreic.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2xtqzyxcl.html


<!-- 参考信息 -->