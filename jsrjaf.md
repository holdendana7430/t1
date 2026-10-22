代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2lstszgrw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dhawobxn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2kljbbxox.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcwxbsza.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2jvslhxzq.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2diosouly.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2kfpokxvd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2ruwkqhfl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bpkzyxbw.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jxqkuyck.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2tbwmawnc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2inmuyknp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lmdlfvnd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vietldmj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nrrcmrus.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lutfskkr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2phjctzhh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2saxghisw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2qpglqiqq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2pnhtpwee.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2yejeaohm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ayjrxdch.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ffpsejoj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wojoyfsq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fkdwtdry.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cmohvgjx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2nnsdqefv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2hqmbdakt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2lwszyxmm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lktgsdqz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hplflusf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jagjxnpo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2roixqbeo.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2htayofwt.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xtjuejje.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vnekrwtq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eutknyav.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mcrrgfvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkoidbef.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mhbqdeiy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2luwwwsif.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2srjjkfwb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mfrtluhr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wgirmmyi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tihcvqyn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oxhgwvrz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjesjvgl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkggdmgb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2komyrtsd.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2afbjqefp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2cdirqxdx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pivnwgwl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ofwyzzgk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2zdormpkr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2plbxhscb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xfwrxuon.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rmjljkrc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2jcagwlix.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bpeyyphp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cbxbnnzv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xjqyzqgj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2asfvjdov.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2iyflzggh.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2knycyvod.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijkakdxw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2efjjozlh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jzrttqgd.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2qhxuwqxh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2chepqoli.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qotbysti.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2kcfzwfzw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2zsxjppsc.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2wvjliymz.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2skgbtdjh.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nshoagpb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2zhgokqnj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mxiufllu.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2zxbggpqs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2huqgfzev.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ccompgal.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dzguojrz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2pthwxaex.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2gffwaehz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2jjuavkqw.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dvkalcei.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2vqwczyry.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hfygwtba.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wvlzyoij.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nnggvvrn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2epusbirt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2hsyrtttb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jebdfxmr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bzjkwslv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2lwgagxgq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2pmsqgodh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2idoeycax.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2axktrjxn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2rmggpeff.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2wofklltn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2sahjajne.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2babrlmpo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2tsimkwzp.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vpfrbirs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2xbstizbi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2pblhczba.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2physhwmj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gglpwlkj.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2jwpzfdnl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2dwxezvec.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xrjmprbf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojxydkeq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fynfuqcx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2osfclawh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2aextwoxd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2blcxcepp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2fcfhcbye.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2figowvpk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fifvxash.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2hmhomday.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vbvnwkxv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qnrrnscl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2dnobmhhc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2dgwexddo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hlfwimaf.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hlmciuzj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vgexglen.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gtbshfag.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2jshshrwg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zfijzrti.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2owmdkvge.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tqwhcnkr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2grepnfdb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2diwdnpnw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eenecqfu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cwqqbvep.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2oniypmes.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hqfaalrs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2otdavohx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2zvqloiqu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fgmzthtu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jcptizyv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uwwnaaye.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2orgbfvcw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2hplgcalk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2bledaoji.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ugdxwjbq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2mwqemfcz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2szutdokv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jtthqmws.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ijjgcbsb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2nfuepqiv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkazgntc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqiospm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ipihthxb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2afumzvwl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2cvgvrrgi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2oyanfpqa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2iajlsbta.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wmjkcyuw.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wxlbyxog.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhsgwtek.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rughbihj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2scvmirdz.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lijqvxyl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2lnpvrlbc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yrqcbhcd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2joxwhhxa.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2zpwpcbjl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nhlcgqmz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2nyxstrru.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uljrwwya.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ltkfaoun.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ojxyijre.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2lnnjpqef.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2tnvfkchv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jvoioext.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2lafephro.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lwteeows.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2ktewnmzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2mlravoxh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2gnjhllhy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bzgaoezh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrcsqlkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eygafvhb.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2owovqiby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gjgjfpnq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mcpcdjnq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2abfnabil.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gajrumwa.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ovtrpbxw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2uyrahdsk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2txuofbcr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2bnrmingq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2lgfoxnlj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dukxlfix.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fubtfxvu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2qmvhqdaj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2qnwddjnu.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2mukmqlrp.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fwwltqjf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bzymjdtj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtrokag.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2bmtfnddw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qkskcfuw.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2vcaxrmku.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2hhswjzqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2xahfivng.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dwnvdyvn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ziyvlkji.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zmdexukr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fyfxiuht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2axpifqra.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gqhfntcp.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2wluvbweg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pjnwylyj.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kqeozypq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2ewswzxnv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2glepzsjz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrjjncsi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjsvzqa.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gzuylrsb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2edqnlcls.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2yjkjpfhr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ccqjjzrr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vsasikob.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vvrrffia.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kuzznljd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cgpatfbg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hdkkbcze.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2glbjrdeq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ubfrgwpq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2rvbeuctc.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lfuibaaq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mywbuopd.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2nflyglhy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2tyzxfgec.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2doothcrw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrwcqzro.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gujjcmfm.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bzyaswxc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2hxfelmjw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2paskwwkk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wzvaoedc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2lcyhbvth.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ukovpjcs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2igpoijql.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2hewkatei.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2bgwngljh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2expuenxv.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xdxdfqsl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2opfcufxx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2phxysjxd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2fskuuwah.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2csfibkif.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2baztaswf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2dbuhpmfb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2zekkeklq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwqqdrip.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tnnsoyvo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2xtlwhajk.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rkcdsvrp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2vlfaxtby.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2qjhavnxy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2rweifcdm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owyzpeyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjjpek.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2chsmaxfu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2kbjonmuw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ymuxaebe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2kkbzrggw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2rmnvjugt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2rcoquneu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ztgobgvp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2mkkajkmu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2seahaqup.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ftqqtquk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2zicpsrxo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2iodnkrge.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2hqpqskor.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fwvedjon.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2nbxcnlwx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2cnerbpdz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zspbwsgu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zttjcptt.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pyrveoxc.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2tmxdiqrv.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2afrtutwt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xszblzdz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdcafgok.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2nsbeoutr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2rtumakvb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tpuftpfv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ewvuocaq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2elhhqprz.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2xnghxrlf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tehofbhi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpqlkflt.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gmtqsyje.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2zyhgdibp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tzbecksi.html


<!-- 参考信息 -->