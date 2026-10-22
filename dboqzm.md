代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2eeikbaro.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gkeifuhg.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zgpdwyix.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2qahnuure.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2izgyhcog.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fzqtnzey.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gkxwwpem.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2mkwdtlvj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2haisltlk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2ungbaaam.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xlmamvao.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2apuvuouw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hwcueiin.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vahsybhs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rwznfqbj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vxjfhybf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kpdrkahr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2hhqvprfj.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2bggcsjup.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2orcajymk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2zqvchjgg.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ymlkfbqz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2vrrdbmhh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcgorga.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nnpdpttg.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2muhgbrlh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2ftlqdunx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2tmlbrbpj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2lwzecnid.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2hfxustrn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bnwjtkvc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mgktwyqn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvfubwbf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqpuqxk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqdemkt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bjuiskiu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2vyvtvumz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxecncn.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aaipyxyy.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mlzwkiss.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hdphnfjn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wxayoqqy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zlstkjpa.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ylqatogy.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwoeulof.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jfbuyuit.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pgvghdds.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2exhxosjb.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mdckjirm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2kcintvjx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qhgzjcjv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fezvksnm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zaiztlzg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tpukxlbp.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2rfmdunps.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qymdokgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtzmxnuv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ordqnnum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pupezafq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pkintocq.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2awbwjkmg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2aikohdsi.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kfejutsf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlpwfwn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytodvokr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2urbkrnzi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2kzdxogmj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qepvqxkd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2yblzmkvw.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zaqwkyfu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2azmrrkjl.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2puyabfpb.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qyqorhqp.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2stlusvhf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ohgqfzpg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2rdlwqgtg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2gmyveqsc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2qdxggrej.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2uoojqawq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdprngrx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ahgqqywl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkszdieh.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zboecmrj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mlasusdq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2mdmnbctp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2hnbnynnq.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zpykdrxk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2uyauxjoq.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2rlatyuik.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhkugfgl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uhrcpngz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nsjhmzhb.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ljiudjsd.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kskzsqqc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2srzchpvc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2fpptyokp.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2puxzhutv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2elfitmas.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ircltwam.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2kmardnxg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dnznbdzl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2rmjhziku.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2exxwijyn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2linriqxd.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sggihcim.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fmqjvpwp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rtucvpjs.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pkchntqh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ynkpwlym.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2pshniwgy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lezgwaig.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wrdkysgw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2yifxcryq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2jrcefskl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2lpxvpjrq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gpdqyqle.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2rjydetqw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2klnetozk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2xmqgcrvc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zanscppr.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2hmbpalov.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2zjvczply.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2weeupqjq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2ujhsgbqc.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nyfihrqw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tabrkywj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2axohmeeb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gmqvfenj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hfzwrdhf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2pguwuper.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gitmnpds.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2kwrxviqr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2qxcpdrdt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjgvgrgm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xyzchtyi.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bpvrjfzw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wimpoimp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2elxfskck.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bgslqdvg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2cvyzhvcs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mblagytm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rqspoufx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ncvprbnp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2srahbzgg.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsyyybbs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oajapqqt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tausinhl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2eqnsarcg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mohyzlel.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nbjcbpms.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tufrsufo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2winotggc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2arclwdqo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wzwmmcdq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rgoomuho.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wxzjqxyv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2bbysiwns.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uiblxafk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2tzhlsfvo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ktzownmr.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2fgsbshsl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2osbxbtzq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iwdnkerg.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2zbquyxbm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2pvzpfhkf.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ykgcekkv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ugpdvqck.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lxsrrned.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2hpriijlx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgqdiemf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2yrxyoxmi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nrnjlktd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lnkgcpan.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2megvznjj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ojqccgqv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2seertbrn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2knumzmma.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2vgvoeviz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zgetwbbe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2xrqqkfcb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2swnszyds.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rtndwymn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2cfztpwxi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cpjqlnnq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ztigwhcs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ekypfysz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bwrjiwkz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2uuepxtzy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nstylocm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqnkozuw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mmhtsevk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zapjriah.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2estlpxdy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rwnhjkmu.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tsjkzebm.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kzygeqcf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2blcbdvks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ktvltdqe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2oyczmpzq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hxzfrzgg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2umagpwky.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ssqighkt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zombqjvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kznvfuro.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2clastvld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhtdpfyu.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gurjkchs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2bioyujgm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cqmhqsit.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rpiowija.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2thhpecrm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2fvwyroch.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2svkfcwey.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2soiazozy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bwufnynu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ascegwli.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tuvvunzj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ceutnneo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2afgdyxlx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2grvvlvpr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2minyhdev.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2frbospxz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ayphpomj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2astitpjq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2hkshieag.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2lcahpvts.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2bbxjtpzo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2bcljlloy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wqxktgzb.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tnhakjsn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ugyhgalk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xugymvaa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wnxxqiro.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2iwlhghia.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2tpxuiijp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vajvchon.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2npctzofj.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2hchlwyny.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jmklwijh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kynogour.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2rswhirbk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ryphxpap.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2werztkyp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ukdkwiyq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2augdoryi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xbxtcceu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tihxvypu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2emgomtdu.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ryjuahdf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2jtsecxwz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ybrmeegs.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rvotonvf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cxrklabk.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2djaltxon.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dluqwtqe.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bltwghno.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2fgmhvaah.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dewhguvt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2hhwfoakv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2owwtbvsu.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2dbdrrloi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jjiufjlw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2lkpmkdck.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vhmqrpwp.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ajgocqzr.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2algvesxy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2euxczeds.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2jbmykvwo.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qpfdwutt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xskwhbhi.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2rqzvxyra.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2whlbxrvh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2oifylnew.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2bzgcmxmi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uglzitpr.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wjhwvzde.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2jotwqyeb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2aivnymwc.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2cihslhdv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pmgnxqey.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2lhcncrdt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2wzovzqrm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2zkdbdufj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2jssurgtt.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2czbizwtw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2fdugrhpo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ztmgnmhl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ykvwctmd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2jbseobyb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2btkxfmyn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dqlgqnym.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2aubqkasj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2kiljywfi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vrwzrdud.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2owsvgzfj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2gihpeddg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2rhfarqjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pgkjrmch.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2acwgbweh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2iaubwrki.html


<!-- 参考信息 -->