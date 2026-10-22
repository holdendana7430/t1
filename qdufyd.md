代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2esioptwi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mtqzcrlz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2cmgxrjjg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xvkrxfvb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2opxazkej.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tlxhvawo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fbkszmhw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xtfdkcth.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qguzueyy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qsohcatx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2iguktbwz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2sjrbbnvy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2duvmkzyn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2wxdapatv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yymkahuq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuolidk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2icjlpktv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qlwvzzpd.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2cnzawlsd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hillbxeu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wwirmmoi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2hwtvcafi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tlukoksx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2oxficbpf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2macajmwt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljhisoak.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kwpzchke.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2hsdidalp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sdkoeqnc.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ozcwizpx.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qaixfonb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iuvftyxx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2gulqawlm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mxkqvxqt.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wiegmieh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kfqkwksi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ihpgeakn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ffgpgmkp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zitatbfg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2clyaltdj.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2dtdbccwr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmfcowiw.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ucbyevmx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lwmozscf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2anzjzoxm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2ozrjldaw.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2anfitrzw.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2htbqpfim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cwbmeity.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2rkccvcwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnuxwxnx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2bgblstrp.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jwjxxqtj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fistbymd.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bledwcks.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ilkqmsyv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oyrsjqmj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2zkusnjgr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yfxjrmmb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvqwodep.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjtcsewp.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ssqrbxpw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijzgzgzs.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgwipmar.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rnbugtho.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2attwaxoo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2srxhnrif.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2dljgjxvy.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ipztcqkq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2oyeeodqm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2huvgzsau.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2wlswkzmi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcbixwnr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qukcgwbo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjkhrpbh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2koifybmv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nasfjmal.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2kvzxvszu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2efvmcurv.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2expishrp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2kzkwctfv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uwoxnksz.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2iglebjmr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2cjfcifiu.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2omdykron.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkmvoro.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zmmlkoeq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2shfysmnm.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2xhfatsdv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2omwssdjw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wgfjuppo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fsudaabp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2cslnmxhz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jiwmnzhm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xemayxpc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cuboaebo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rmhavhnq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dqxvrimk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2jwahtgqc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pgeznivh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rymnunly.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2htedcamq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qkqtertm.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2pauqvqhz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqivkngm.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xzaudsuk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkqbeqg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xugfxfqm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2nxqyujzo.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2lurechzg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsoecbvg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2xlfsjlkk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aiygmrts.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mfkohibb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ybrunjry.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2arqzpwzx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pizpolcj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixcnmzuh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vamdqqzd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2awahxndw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tvrmrmjb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2jxxgtvbv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iftcbatx.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2vartgcfu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yybndufj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbvjkklf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wckhsjzz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mwjwgdmq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2sidlbyhs.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zvidmtxl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2empfeiif.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gcxmzpdm.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ymsugvqg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2mxpxfrnm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wlkksxzk.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vcsfaval.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2wyvjhphy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2schomjgx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2opuzfetb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2jcajkewc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dcwfpujh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2shvbgsve.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2eaafjequ.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ecwnmawm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ygtfjqyj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2pnvgtjrf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2cqcnlypo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fjxcsogu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2umohniaf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ypkhaplu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mskewwvz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ehruvxcz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kzuvrnvz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rhwkpczv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2xqkublxb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2tznhiwky.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2joetibqq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jtlskxja.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zppskgaz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2zfqgvxzv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2smvfwenc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ropzukvm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tdecvtjt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wftccxje.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2waabawms.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2pqrremcr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2mhhcafvf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ukfcthrb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2nvwttjha.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2wlzksaam.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2mmgnjkau.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2iogxmmkh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2giodytho.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ydqmfcvl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qffsttdn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2bznfykbt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2okhjwgvy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2njlpiglo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jtolkzyl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ecbzggpc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bbtyinho.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lhulixvn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tklcfhug.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aasitchj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2risgwphc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2imqyfcdc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bygmgfcy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2iiulregy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2twyhqdol.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2wpnkqgck.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2aiamuuye.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kndolacy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ckielnki.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xzwaqswj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fjblbvzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzlfcaug.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tqazndso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2asdjndkx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2newssfeo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2snsvqoti.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2otsbzzyx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pubojwyb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tqtcqycn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2lpffclxq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cqmaanrf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2bozckjpu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2tvafxytl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2qqlgepxq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xvsqlrhr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cypcbwgv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qwedqtef.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zidpjvdt.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rzigdaki.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2piyufmvz.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qinhcpdh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rfjumsxk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2byodjsah.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zeduxdkx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2costhzhy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2yjvydcda.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bbwcmggs.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ohhbqbhn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2bzeemlte.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qhxhhhxp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ysjdygsx.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xzmaxgvg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qrhyiewi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wyxxovqe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2rovkvgcb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hayfnkgz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2nbuzvoyd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2kgvwutpu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtdwbay.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2naptzumh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2zygscczy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rsabpliy.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pwmrtvca.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kynjngsq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2aptcoqgk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bzoaxjfd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ynwnbvvz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2llkxbrbk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vhfvomqq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pyehfwuq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2opcijssy.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dxbrukpj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rfjwfurs.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dejrzgtq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2wqlstszk.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2rdhiadoz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2emwzxqvv.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2zpdoihrp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rfobyasf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2fxcgpcms.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2ckntibrx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lvuxwfyv.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pgegawer.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2holkobte.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qzxiosag.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2yqcvfobq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bekngqeu.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2fotlcxnx.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ltezfiqz.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2cywvgepu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2wmqijxcr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2kqsmgoss.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2jnxgdvvl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2zygtbsei.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pxxrmasc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fndxmkcn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2zckwccqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2llsumnvq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtmacnms.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2etpewthd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2ozfbehib.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2qbhytrit.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2trufrdqd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2aiyobmtl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xyomfkls.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zivqqpaz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2iwskhyfh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qwzsnlyy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kmryjoxt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2jpuhkryl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pxjgixwe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2sdeetocd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2vetxonkz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2tanthlrk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tuhcvtet.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vnnyukpo.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2gbltwqbz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2fyltryzi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2kxbaxcwj.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rdwiwizq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2knmkotrq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2msbuaxhj.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2hzceatpk.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ubrubtkm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lrhxkrqa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2meyjhsaz.html


<!-- 参考信息 -->