代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nygbvlub.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ckwnmydz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rcxtpzmv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sgxusgan.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acgtfryd.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmxnrhvn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jqeolmxn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2cebhvflq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nvpblbum.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buyepwpa.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wsmtdjfw.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2kpilxyga.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2hbqzpyou.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2evnyldtp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akeiqxgp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zvcflktt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pdcsecys.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2swvnamfo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tsaihnap.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nrbyzzyf.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2lihycgjc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohoedtdm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ytkeyzlc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2irodhptc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bdgkziow.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2tlaavtjs.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jfhcomdh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kizuihew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ruyslwhn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qqyuifeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rfopbqsc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2zsxegflx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2slwzqkew.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rtupzcgm.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtaqmmna.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfsyrmu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fwenxdqg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ddxnhtxp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mhdwowqo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfppxlaj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2ucputfky.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2zcfhfsop.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vtlibsvd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zogqvpaj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnuczgpc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tqjjkxpn.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2bjqmdvfh.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2ayxhxgxp.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ghckfyth.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2uqangmtc.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2gllbmdlq.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2apwklgws.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2imsctfpy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2gmbvatzz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2xtzwwgjy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mdfqsmkm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2slwysnmq.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rjfhaiat.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2axqwuzsz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dehcjnwh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ejopakmy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slkdxmqm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xglaueud.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2pbsglumf.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2ixpkexty.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2olwqqjgo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yneyrpqy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mhchhrbt.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lewziasv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2vlodbpku.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2iemphftt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pjpphvsi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2qlqbluqs.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jbcicams.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hoqzwcuw.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2bcibngqq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jxnkwwby.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xajvzoie.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2afbqhhaj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lkmjvhdf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vddjqwmt.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2snjypgin.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zmwrycwh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xszxptwl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gvfthidb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2skqpulpn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2cpywilis.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pjzrybiu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2gxapqvda.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2cxcajteo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xilikvgq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kukfydnx.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ieolwtzq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lnqpehmj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xnhktcxn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cgicbemm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhwshpuh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmevjkch.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jvrjjujp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2mdxmnoof.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2mlmqmyem.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2omighjuy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2njwjjnfx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2febnpjcr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2owqpxmsh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2eyvxxynp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2abxepgxd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wdyukiwo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ctjmgkjg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hjfnpiyw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2wrvpsyce.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2wcynwufa.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2cpyyesab.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2cgokcqhp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2blhnjbcs.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zbxctall.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2cfgannkx.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xmwktnlt.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ujcscrpy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2ddmoxnyu.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tuciepqx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yxljzhgk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cfmdmyku.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ukdcyksc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2nqctxftf.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2wbcphtlq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2shaoghza.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qygaohjw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2djqpsova.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2vazdvcjf.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2gofoqtcm.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dbtrnewf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nwpmgawv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2exigruam.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jsetvaxx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2obnhdnzm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2kuzmrnsf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2txtogatr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2toxkhzwd.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2elyahlxy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xwlclbon.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2svvyillo.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2grfxuotr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2twnhulpm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zkyosojv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ofrcczau.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2sehwdfwv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2brrmvwgv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uuhtnysd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dgjiecpw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2izzwyuip.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jqjyvrtm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bqnphbsq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2oziqgfak.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2thdopfty.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2koaniqmy.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2iahwejcj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2paknzkrd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2tpagvsds.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2eezomxnj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apbflyex.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2aivjbsgy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2slkrxvgr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2xwwgxtox.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ffbxfcci.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ylfzdhaw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vpkdihev.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mkyfewxn.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2zvkfopnn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2trppxjuj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yozrcltq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uqbvmbls.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2kuzdyzdr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2gmahoyix.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hggirdse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2frojzbgx.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2skenemly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrfnlnhs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yscqttxq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2zzgvlxzb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2nitfuuyw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mlbnhcug.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2nmpsbsqg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2gxqfvsrb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uivzohko.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2shumitjk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2jswueiah.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2wdxubqpg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wmznwnik.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qngraztv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2djojmctw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prrmepzh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2lquhmckq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ybbqlwrp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2jjwzmofn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2wwvmgoob.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdaohhlh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2knpqdzsc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2rfrsxhgo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2esdxgjla.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mfikriqz.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2killvyen.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuownjb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2fbbzgqcg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2alpwdxax.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2bhworrng.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iuzdjhbq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2grkmkeqx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2hsnuoegg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rgirxfqq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ntagdcpg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uwxxtqgl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpjrric.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lpvxxkms.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2acgkajhy.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ctnixevu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fxydqiel.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2skfnjath.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2njsctgpl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2bztxbiqo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2fnwlqojw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vutcchtc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ndqozabo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ekmroshv.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbglbpnt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kdbxhjaz.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rweawtth.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mgukvqly.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2zitlsyec.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zcgtafzf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qlqbgbax.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2qhpahmlp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2ypworrkt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hmxfrgdk.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2euaghymt.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sqjbaofr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hhgpkvef.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2mbzmsfpl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sqzzlbyj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2ugsotany.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jldnhuxe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2digaectv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zzidexxd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2nsvpfqsd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tmxqlkrw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kuhgfacm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rpgykoua.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bntovkwu.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujjfxsla.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vpnuxbdc.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2mwlqkzjq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2uxfafeod.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2seynzroa.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2rltxncew.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2mrfolmsk.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2qzshanve.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpejdzkq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dbftrsjb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2cxgzbrmr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2keodavbh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wyctwngb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2lobitzpo.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2varnburo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgaytzb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2bazlkkrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2ayvtravl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2uszlyioj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2trwfueps.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ncfeajjl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2woswwpjx.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2buuclzpz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2apbhzrvs.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2ggaxkkfc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tmzuwrau.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzlneisg.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2zbupexov.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fthxmdlc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2omvnbaju.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sxnbuyii.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2oyligwaz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2qsnuvbwn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ywhtansv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2iuiiikan.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2imslydqf.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2hkufkquk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2stgokyzd.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2daavfdtp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2yrjmkhcs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2kkeqvgei.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2fyrddmio.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2oexvgfuc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ackfbaja.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2qhljkbhw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2xffoopch.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2grtppqfj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2qcntvoov.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2yprfgfen.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2liqjwsef.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ntpgaauc.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wlbnulam.html


<!-- 参考信息 -->