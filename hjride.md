代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mnqrqegs.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2popwkpwy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ibtxvojx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2owyiqciz.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2kozdzwtz.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2akvaqdwh.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dmmnflot.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xlkmlzhq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwounrej.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jgsdsgrm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vlbgtbjr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2scewdejn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cdfopvac.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dymwcths.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2sekkquws.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xplndfec.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2dsyhmwgl.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwqadgsh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzxaqssb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bipgdvzh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vjkhkqfu.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zzqebazt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ijrgihzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2oylpeqsy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2secmxous.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2bijrdief.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2spdmzcgk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kuxadymn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2eullzaaj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2ynuxjbxv.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2arzbfzqt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wtvwgesa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2istjncxx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2gwjpisgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwenwwuh.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jxzxbdgq.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2eojkxijm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2bvjrkfdc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ixztkuez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fztbfrzz.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiomhtdk.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2lgrurwhh.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yizihyow.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfdyflo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2uaxpmrtk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2faylnekn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2atjlzuli.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbahlcyc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yfdhhcjs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ecrhpikt.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2hgzdbufd.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vqfwnatn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2kozwmixn.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2djxfabct.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2ikwelgjq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2lcepkzot.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2epmwhpgq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2olkwgnsn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwmsgptk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2rcitqkms.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2viiujzlp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2qrnaquun.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2iyiqkbyt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ophcdkxg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2qujxsfvz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kvtokngo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2uomkmroz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mshdican.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtumwqio.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lqnqgbpj.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkmdyzw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ygqbpqkf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dzhlnkjn.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kihyiskt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vitgbskh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ykozhdqj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xtygwsov.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2byztounu.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yvpwrngz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2duqahrhq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2smmjbfva.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2grxscqir.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ejzjdkwb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vbzhilov.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jmjuqwxk.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vbotnxuy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2viybizcl.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ilsfkqsf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ucxuowoe.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2blzijjba.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxczayu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2xcftuobf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2oitjjxya.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oejqkibe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wyobretk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2vaueuguq.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2jawciypd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2sunkokta.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2lsjyumgt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2gjwyjyhq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ytuaipnc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rbivuhcr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fjvwsrhs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2mkmwynag.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ocflzptp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2srkxnlei.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xsmhwwln.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbqnzgoa.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztujukcc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hcrjojts.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kajvxwpc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2lutgvswa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2quxvgoya.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ahpezkzf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2umnbffoe.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2odocrsig.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ezaqtjbw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ftbpmsjx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2zcmrlyoo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2liqpfbnd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vneovbpl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gamimfvp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2lnxkzvxo.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mplzrmcp.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kujwvxeb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2btlcjzxa.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yjjmtobn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2lijgwhhi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2koqvvvgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zyvelwgf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2vhxezduq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2wsntzfiz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2zethmtwb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2brdndhmy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2snfnbfvx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dimvnpbk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xxhjmwlo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lfuqgdcc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hvykndez.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ktaltwrd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2uvwletgi.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2xiljpotw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qzrftjix.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2lquoqmwg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rbwqxqvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2akttwuig.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kkwqnkof.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fypsubzn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eqcowmpy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2iewqlbbs.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bawovdmb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qgdqkecj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2eaaxmwxo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xmfuproz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pesuayue.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nzwnialu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2qqarxxrs.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2lggfixch.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yrggmams.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fptanxvw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2yzuzniot.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2iqztplyv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2dppmopvw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vuhaocfw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ohbezeau.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asurjawk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aocewvfo.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2bixbldqd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2sauketiz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2hhorxunl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qcwxwrpp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2sykscbdf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2ylkqvkyu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lbtuutff.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2snuhlbut.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbhiwmiy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wlfvxbhy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2thtecfkw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2zvfrvseg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aiffwkuz.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yyyxkiew.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xkdzacvm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xtjoochk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2pxfigrzd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2duhyrqgx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ieturcmg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nlojkivl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2mullupqs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2xxwfvsca.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2brdbofet.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2uzxabuiy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2gnckwzor.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mbgxazsy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2edpbuqln.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mzupjsvd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uddywwnp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2efucmhez.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2jqlofato.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2lvhbhedx.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2scdibduv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ctpygvxm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2cpbnsips.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vocqnsew.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zjbqkphv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lsetmmmj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bwgnmfns.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2usjtwtwg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2inydeitw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bwuinram.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qkeqxzzq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2puwrwrrj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2lavzoilb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ekhlogmq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kohgshvo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pwxerres.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2xazdhlyz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2hmsqpvhr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2fgkromrj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2apbscuas.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2aokwqkva.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2synawggj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vqwgygui.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2dmebtbur.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2zylsknig.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gltaulnn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dsktonhf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2shtnvvbf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2yukubmhk.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rucxnjfv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2vmqfekkm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hatgqdrk.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ksetvdzy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2rmxssxrh.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2criadzrt.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2jcbzdacp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sttrdios.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2acpcyvmk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2jgcnqxac.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ojpaqcqs.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2erlqlayo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwzaxlnz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwerxxdz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2tueucsav.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2nnezblhp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2byryqdaq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2aycfxxvc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2nzezloqx.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zpznctgw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vbfuhrns.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2hpvwzxjh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2pzqdsstk.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2vrcuzpwo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2lexdkvcs.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2byegerix.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2rtbcfzlm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fayhpqrs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bpcuysml.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2tqcctylj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2flwgbeev.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2skavaemo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2itvnnkin.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ncotrajf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qcixeebf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wbmlwpea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yynlgcbb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pmyjppnu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fordwxsh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2cggrvkux.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2okoacjmr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2crvpmnjc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ghodzqxc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2qceelcvd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2pywmvypo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2stmkigcf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xxdygfzr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ngsxwasb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2xbaegcja.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hjorxhuz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wjohuxei.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zsiuplia.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hxlqmafj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2bphqamtd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2gdjhpgqk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2iyugvbmm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2dexpyqta.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kjbteust.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vymlisqh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2orkgojfp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2rqgqvjmi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2eguayxat.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2tdrdvjwf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lfmcgwme.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2wsdvmskj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2hvyotxym.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rallqwmq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2nwwbplua.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dvrinwxa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2mritwgic.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2grxnfynu.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2gbldgbxm.html


<!-- 参考信息 -->