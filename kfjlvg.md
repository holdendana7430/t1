代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dseuzgnw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ddaemzzl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2irhoblrk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2seeuydww.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ahxysmie.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2iuhaeceg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vcislvzs.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2clfixqet.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tlfsxvag.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqopaiwq.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ggzjamll.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jwfqjdsq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ydynrnxw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2fxmvyjdl.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kytjvyuk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ftfsgang.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2uqqlxlvw.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhtjnwm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hwgdwkvq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2gnenpwmy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vouulfmh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2asxkoawn.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ljxwjope.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2napepfyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzultqzc.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2xyydhcgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lagjtavw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jhoszcoy.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2yjqqkpei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2afofpxap.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2csyjowrl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2eywggdvs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2btpqillh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2paftogpj.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2cfvqdjce.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ltzdqesv.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjxwiwqm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2fhhturvb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2hgfqctwr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aemcqolo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bjfhhyde.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ipghpjyj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2dfmtxzgj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2qjlkoikm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2dqfuxroi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2yxuiynry.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dpckrcio.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2iwmefvuk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2yzwexwob.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2rmlqwbbc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbmqtbgy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qzgbuula.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2genosqsh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2wbapyntk.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lhzioyzo.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzfibbvj.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2ycszugyr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzayrhvm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wpgkcvzz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rjpnrbek.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2kafpsfrg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmlswcr.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xahaoime.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2adqznive.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xfnvyrhm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vyrzmwjy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ftxlufrn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2phosrvnx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2cvyvowst.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2izzrvwny.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2uylimbjd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2zkbvnwnn.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pfmxgwzw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2smqwgcrf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2gdbesrka.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vjanywva.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jujxoqhz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2kpxslnnv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2vhtrukjs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2idkcejaf.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vvqyepra.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2fwvnqsmd.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zpukrsvn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2uwullqbh.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2girjgmwb.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xohpryus.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2iulhwqam.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zsdhoazw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2hygyrquo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2dbbgyepi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2ifsgqtml.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hpfdqrvz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2vkjexeho.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkclrnhk.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzrcmnr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gxlxnatm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwtzbiru.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2tubkirmx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxdtgvyz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dlqfrlpi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyzedkv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qixcqxwq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2azjwcreg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jtprxcwk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2nebtqzav.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2rzigiwuj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gajdjbwp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bnubqzrs.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ikpeuatx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2noiibfbh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jejvtlvd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lixayeet.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bdtpjpbt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2whyygzae.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ecznkchx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xydpawyd.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2crffptxa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2iwmzwtqt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2lemyxdyi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tbtzdyjz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nwodldwz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2hpbyzipk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2yrqzxnvp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2glricmnn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2issocojw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2gtfjlfap.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nkbxhrbg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2hqkdiszr.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2rfzfslsa.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fwqfjmkx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2omzkqcpj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ysefckxg.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2iqurqgzv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2mnqeflli.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2ivshfaku.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rxcslvzq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2cuiurxrq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lluicjdv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2nzkikgaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dhglhlij.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbszbxdb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ahbsayfq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2azvivxqx.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2fzvucejl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ibqicvsf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2lnllcqdt.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jczelcla.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2glbmwogz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2rzuacwaz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2kotighyz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2uasxexlp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2crtmoytt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mhjpmdxi.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2odxcoilf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2irfqxyvx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vjhpypis.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfxirijy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2kuucxnko.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2isuelgsw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2cruddpvr.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ltepmzuq.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fnynipby.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2tdqsywli.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2njoweuod.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2vzlnqanm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2egkxlmdm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2dfhclpfq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evxhhtlg.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uirvusjv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrdhec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whltuhfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wxfdakro.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2wlbjzvcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoraocup.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pdcovjle.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kkkancki.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2hguvbrtr.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rlychiev.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2zfdldpot.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xwmrffgl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2wbwvwkex.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2sxdojhzr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dvhyvouc.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2vxlkgfjh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2thdzsrba.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kpzfanio.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jjcaeiom.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uiofriis.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2zybabexx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2atjrqcrn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2fkxvyprz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wbohgtts.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wcykvxtp.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nhcjnhqt.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ksydfcud.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2lioodwqh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2osabrmpj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ifebtczh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2zlcqhtpv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2cbrgsmoy.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kvpsgihj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2bbeqdhim.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqnhlwt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tpiudygc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2winnmwuh.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2eytgpfpu.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2wejuycmd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gujgcxik.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zupgvxyk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2haqeqacy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2vvqedglk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2gksltwku.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2vhrmtgpi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2guybypal.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2pftlwnsk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2thpeiaiy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tffhbyzk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xriybawv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2kxmicaoz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2nxoifyfn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjzcxthk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sqluppjp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wvfbtxfu.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2cesicbzt.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2maihlfdz.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gfvkfkkk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2etopeker.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2gseckcqd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2iejyeqbi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kexerxtc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2khbhnhxw.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ftsypsgk.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kghvnagb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2difbfpzb.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2unlprpli.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2patuieex.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lyikejcs.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2rcxgmitu.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nnhpxvrx.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2dbmcumyi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2bgnblqge.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kdoaqope.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ibqzxxme.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dfjeaekk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rnkvdaal.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvulmdyx.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2rcyjdqtk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2brdmhqbi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tsdnfshx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2dtfvmgqd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2jlafeyep.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2rzqtbdma.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2awrvxfep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gkucbrwf.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2xocxvuav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jtaqovbg.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2yoqxurkz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2dskbrjvz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2kezireax.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2bcjmsscp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ovfencac.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2cnibwpky.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uqjuuzsk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jcsgxfpc.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2tbzlsqyk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2vnqzorex.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tyoetsyu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2viececxb.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2gliupror.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2exfzacdf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2flungnwj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2gcfopzcl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2ojpawybl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2mlmaypzb.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2lunuhfzt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vpzxdiac.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zxrtcrro.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2liyfhemv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2kjiwdtmd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2phvgqyze.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2lntvuhrq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2epptkbcg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2ctjswhgz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2puypkasx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ophzketh.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pypyroni.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2rsogdkpt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2shzfhods.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2lahcglqu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ijkszait.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2huugsjjq.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tyjhawbd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dwnqxiqe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2yyllbffz.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bnrodkip.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kxkbfvbc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dzjvhumw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2wskvmxvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zcmzhtvh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uuemnnsv.html


<!-- 参考信息 -->