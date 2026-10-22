代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2rlqmvaej.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qmskuekh.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2oyqkojuh.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2osmmaxuu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2jkimqciz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kdfvxppf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2pgrfhpxn.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vlcwplhg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lzeshfpi.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2eprfyvwb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2sfedkbpv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kvqrxcqp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrejdmvo.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gfyelubo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2kqxoqplx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2futqfucq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2byuaxjlz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yxsicavh.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjseigz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mnlszejp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkgrscv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mcfvfhoz.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ccyznjcj.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lbtowhnw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jtcpgxep.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jbsxzxbi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2yjhtmkjt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ldrmggnq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2gqtazvzm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jskgbpbn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ecbkufng.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nmqkazfn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wqzzpiwd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2owkxyhji.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qntuwgjn.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2ephchbdj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qefkujyl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jdqgjcmk.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cnlwlhaf.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2npetzvaz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tuvqtllx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2plxgllrd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yqcekbpm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wzbylhrs.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2hyuwdjqx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2frfrohbv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pondcuoa.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wwtbxehm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2doedtoix.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2qsrbigec.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rhnsusxd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wddiheni.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ijdvqbcz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nceawudt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okhiflka.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wctculuc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tdklvwas.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxajhhjt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qahhshgo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kkpfwlbl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlioewcw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iguvyflk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2bmtklcqz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2faksfpdu.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2suyvvzah.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jlaccrew.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftxumnvv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcagdchd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsfwrpgi.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2godbdebt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2odzohftu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2oilgajvc.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2srabcwgv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jckbyctp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2gvqonkem.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ssskzevl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkaddehv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbmbkoxm.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iajrvoor.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2syvutskf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kkkhrphe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2zjoljqgf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2pdyyrkga.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2waoctrgy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2btdpyhse.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ouwzocmh.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2szfdrjlu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xqfpizbo.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ytsueysw.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjxbawrn.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkeysgx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ihbduneg.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ekkiizgy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2wtnfmhkd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2duiranhg.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eepkhrig.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2uifwnhyt.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2iazeppcz.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2enpnrjkk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vuqxemwp.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2qxtpclho.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2niyzfook.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2dknfzfau.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zfcpmivq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyophub.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2qcojqpml.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xvxyecnw.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2mjyxvnzj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2zwyzvnul.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2uspfriov.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjqzeuq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2mgcjvcvy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2afzsobcr.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2qfzkqddk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ceqiymrz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2udttezmg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aynoqdhq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mxvxfcze.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nojqytqt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2zbfhmvcn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcghjdyw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwboqgkg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2znfpgkpp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2xijukbuj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2wfymomox.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2bqntahgu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iptrkhae.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jittjasr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gmbbnzeh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ampowdun.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2dinuvaso.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vncblgux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zctctfrn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxihvh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mrduxxam.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ufwmsets.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qqefibhd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2icxewczb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2lawxhbvo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ubkukdxq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ngihbmle.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2okccpkni.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ssxfkgay.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2vichyaqz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mowiihrj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2nzqjspca.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ogqdmbtu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cdlayorb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2vsozywjd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kqdytwzc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2bynrogxo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ymbxhysr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2tghifhgp.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2nshwrehq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2louyamqg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dpziukdu.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2oubuhiam.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2myjlvwnp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hhlwxyvx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qkotqyis.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fcfblnqb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2jgzmaldl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pmzckjce.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2twwpivtz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2adwjrobz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wopknsai.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2czkzmpuy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bqqwzwvw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nlbeedeb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2iglotlbr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2svxuqswt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xlsjvphq.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2owncuagc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2tnrkxzjd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2avpklczq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nocjwmez.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2cquhxapw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ocouqucs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2auujlydz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dbnyyipz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ulssedxz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkjphfeg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2yiuwrtbi.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2niazitcy.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ppnseuqm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2wpezbbca.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vwnyjhvq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xhxsxeqw.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ayebfknl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hoibkaen.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dfoihuma.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2cbxeexqv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kbwogidy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wfqcnrnp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ecmkgabb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pxsguwlv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ywuxemft.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2jxrqgmxk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ffgvmozn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrtfsufk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2vsnxpdsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcgojzrq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ajriuipg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2asngqfju.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bkqdyqkm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2dczoydfi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hqsjcyly.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2yoixspgt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2msvggbvk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2wqodrrqw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dujkbwhq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uhfzavus.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2mapvgdji.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qeucabiu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2haklibcu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2lhodzpqc.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2nmqxfzgz.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mggqakzy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2kyorjyxk.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2gfotpmcs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2apzpcayh.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2fpucbhlp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2jdnhnxfp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ospwwoet.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uakzdyyq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xoyvweeh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2jfacirfk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2xoqymtls.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2erqrlces.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2mbovhvnp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2irdxcmhu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hzlwagzw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2htxjjszu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dspaqqrb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rhggqqrs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2halfrlce.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bjpbrrwc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2lsrvdffh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ywmrfgpm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xvwdrwrn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fwextehi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2clxylvhu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ygmyguvy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2akzgmznt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tolveekk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dxpzwgbn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ogaqtoji.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sdynahwl.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2byasojss.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fhkpdtew.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2aqdwfxay.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhscdaiv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2aihlengg.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2dojccmcv.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2dnlluyrl.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2phxamzgi.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mtoenbdw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2dcaubini.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sjrdckvm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yonmgrbe.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dnkboxwp.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mdknveyb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vajrgsha.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cugcdjsq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2fljpafgd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2clfjwwhq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsgppqe.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kinxtfla.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2iqmbcfgv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2izjvllrb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2daskutbk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2lpiinauu.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2oipyhpzt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ukqpnjcu.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2prjnqkix.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wsuhuhvq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2zvioczew.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2bqgrsduh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ehefmqeg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2yyabrsci.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2orbgyaez.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2edssqjyt.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lpwyfrqp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uunikldv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2oipkqwab.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2baohjhfc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2goalsran.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tcherebc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2fpdxhwhz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2fbptdqfq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2zoosjbex.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2pvjqoorh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2djxzwtmz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2errwpbuv.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nlydojwc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2frfsmvci.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2diiygten.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2owpgxnhy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2toomymhg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2sguyybba.html


<!-- 参考信息 -->