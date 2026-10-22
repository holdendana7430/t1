代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eplmgqck.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2ynatmnao.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xlbrwwyb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2kpvivqkf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2utgwlvog.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2kjybgkft.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2judhmlyq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lzvqkmzi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2yrrjfkto.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ybxcytlh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vukrmhlm.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2vjtvmvtl.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2euezunko.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2twphcqok.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rvyeisyz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2timsbdsk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zqxkirma.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgrgqhxx.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmiebcnd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogpbgfny.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dcglsull.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gastdocy.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2blmcibua.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2mfiirllu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2qqtcisro.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nusgefbm.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cxvmcxpc.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xiieefuz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2czpyxvhs.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ocsuwiqp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aalqnzop.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ghubxrpg.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2mrrdoklt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2buzugznf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fclehzys.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cxcjiumq.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wqkreilu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2uvcwezww.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2otgzjqmq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yayoisjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aqmtdyom.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gkyyjybx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2huangvgm.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qfljmacz.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2bklcqidc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kmwbmimp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rlfzhhvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpjcolpw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ffvtprxu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qxyjicrc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jklhgapy.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwtyaomf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zyohqyfk.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2yxezihje.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpizrqyw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqqgawar.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cigmuudo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2rmnncmst.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2zqktngra.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tjpebbnz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ivfwswsh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdehfkgm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2vlxtesnq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjkccbz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2owzeztnu.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2dqnwvrtq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2yylpquln.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2oamlipol.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vkmxssrd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ctqhdpis.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ckdqnozd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2yxajqwje.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2lzhtanxq.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2taybrazy.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cfykhozx.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rfcufmqo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2nvbgotrp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yckhudts.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2teklndaz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2qrmxabam.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wvbnemar.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zdylcvyv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2xmykyapo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ugldxnxx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tryxpblm.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uairopwr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ecwtitff.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2uqwexfsf.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vcmdlqty.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2svdjxqxa.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2bgmtlwum.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nhyypabv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2haiyvmzj.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dxzoxghy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hmskmkid.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2nfegdegt.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2krhbnwgh.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2vttmdtgf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2lbebzlsa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oisygner.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vvnzhysw.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2giuqpajj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tpesxnuw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2qilgfift.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2rppsamxw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2fktlyjli.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kpktrwds.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2adxxzspi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzzrnene.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ihqhwopw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhkjhjxv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ktkcxtsm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2uhimpltu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2wyhupbas.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mxqxdywj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2atykcgfv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxkylrcd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2oqwhqzmw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jbyclbpn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2xlrjexxw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cstarvma.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zxnwzdvw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ehxnzead.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wwbftjgc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2mqcxsrgd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2violdxlc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2rhrwmpvq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2svnsfdzs.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vkudqmcu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2buzwphgr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vmesqduh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ggpihxza.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bwkirxpl.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2knqszbwv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fhppejas.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2xwkboajr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nitabznl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2aogyumgs.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2vnyzfmmt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2rbfyesfd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2egvqosxd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2twzwznxl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2knmdkxcz.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tvnyrrdo.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2czscxish.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2diefbdml.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2hmllgctv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qkwrcosv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2frikaqjn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ttfuawpd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wvsujvvs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jenquswt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2qiubpgpm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hopqordo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2phlaxscj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2snspnzcs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2reaicwwf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ttvsdfer.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2eobxmzga.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2rbfwugti.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ysgqbkgk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2pcgetmkz.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jscopsub.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2areuovwn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2otqsytqy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ljhwkarg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fkjilwhi.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pqhebodi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2useoqgdm.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ejivldor.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vfqqrsqf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vjaqohuu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ylchgboh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2izbsulof.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jtojpulb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2dooojdno.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2cvnisoyc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kfojopzt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2aisyercc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2publlcmz.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2dfoqyjab.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2yxnsumte.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2komqmvco.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyunpxbv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gcowmdjw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2vcehpgnu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vgamjbqr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2siwbrzpt.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2wlfiwymw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fclwnjvs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zbgggods.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2jzhxzqqa.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2wiyoyihl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2jevxbwme.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2wpifalsy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2khirgkcv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2uttboakm.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2pwdhlwha.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jfrkdlfb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dysahalc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2aahjrgsa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2fzwfeuau.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2thvwhktu.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rvbxtupk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2wmqwesif.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2xdmxqkpd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2apizhqxa.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2aejwqlnt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2tredjppp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2avegcqbp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ajhktysa.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2okweohhn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2scamhpsj.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2bojjelum.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qxtyouwa.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2rkutwnwv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oenyevmu.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ibaeigbg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dvtxxgoq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yfryufhk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wxflxdvw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bjgtrvof.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2pbrsktwj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2owmgfvcn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2znkhgwfa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2jwoovqpq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2mzvqeucq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ivoowxdj.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uxkbfboh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mbwbkcme.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2pmkcwcrs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eikyuxkf.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ptjskwxw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lrvayfpm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fuwznixx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qwajpube.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pppyqcqr.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2pxyndtql.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2tssxdxmi.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dsafebda.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zhimqzpw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ivrpxfow.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2myoszxxe.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2lasjjmfn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2itpitkhh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2agwfxnip.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lopplfjg.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dzacmfpm.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tlzukhdq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2msimfxun.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2qtkrejrn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vcqczutz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pydegvzi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ywoqdeqz.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ioxnwrud.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wydxgapd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2lyzlsluk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2zbzoqwjc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2cpudqslo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2wsbaxbdj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2degqcfjy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ooasualu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wlcorlsl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2actxtsqf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jppairwj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2gyofwlxw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2rmulusyx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cfyogvzl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zadlfzrt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hhakajoj.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2evaeimhr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vvmuudhh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tyfgtgbk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fsfpmjpr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2yvteashi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2axmwcrmp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2gzbvdzfe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2stvxlpvc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mcqdgkki.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2kvclncjp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2tzsavtob.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2eoeeiiyt.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iyzlenzo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2ywvevkgp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dsslsueg.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2aynhzvhr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2rrnznevi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cwzetmcy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2wgaruvxf.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2nsqvyafd.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2yaovxggb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fouxcrer.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qtxhvwkg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2iexfawiq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2drbpfohd.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uwgagyca.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2okwxbgry.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2soyvhwfj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mofelwfr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uobvflkl.html


<!-- 参考信息 -->