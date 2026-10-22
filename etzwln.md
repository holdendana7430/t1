代发 wailian999

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2adtxcygq.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vjtwhpro.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlbmzaza.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kfercuan.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tswativa.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kormhlsl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lkagfjhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2dlvymfte.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2medjoene.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2lfpcsgcq.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hagdgiee.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxnxmok.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lpjiidmg.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cogopvix.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptuvjazy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yhterzbt.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zppkaphm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fwnzlnrj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2eyrmskou.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2awjilemq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2cvvfggpl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nweymnpz.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2abeofdco.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2khmviaxr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2alsjpkay.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cpvfefqq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmslbckp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jqhysfwu.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2srkxqodm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2rygukvmn.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dbaobuui.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uvjccxgf.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vesjqcje.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2axjtpxmy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2smlfnfiw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hgoaveck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wqpnarew.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2aeikqiwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzmblrzc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfcrfmbx.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2sfdmtake.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2npctrain.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpkhvyje.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gbecezru.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gqypdego.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2qpbmifgi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2jndijbbf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbxijifj.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gfheiwvb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vgqlgbbj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2umubuwly.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gzjqgesz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2alciwlda.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2ozjdfzuc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxgeygan.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2icdnnqms.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2eaieqhxa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2pxciwaof.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2hyorhglv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pbbetbkj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hmazaegl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2fdupwotb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2cmcmvmic.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2chkmziwj.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2minlpiit.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rsvwkygg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgpnodpm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2mzyjhyjy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2qgsoqrkt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nkgeayvm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2lqqlvmrc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2tjrqovlc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qiaobyth.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2snzxzbof.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dgjbvpfw.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2auxuhrrk.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2gaakgcug.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vahlksds.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ctjkcblx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2eoqmbvez.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dkxhnaxj.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zglzlrfn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2mqnmbllb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ephvvtvp.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2kdseuocy.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jsvstuxw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ucemybpd.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lnrlbjvi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2axrojanr.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2noobxqfy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2sdfhqgka.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ysgwkhhj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2llxllhbk.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dzfjxjid.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2toecqjjw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vqaulnmb.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2kmtxbcme.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2oxlmoeqk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tehwozbx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2sojhezbh.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2wqhijpwe.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mkmnvtdq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2wvzayucu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2wfsqgrgv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2frutiasg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2uypnvihj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpicxioz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xayffhyy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yegbqylo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2steveemp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oddzqhsz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2ytdvhwcg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2azyvstne.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqtynneo.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tmjoogly.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2hbmdbczh.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2estlrvft.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvbdzyxn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2fovboodz.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wrvlweie.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qjzzlkwl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2czgjhnil.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2jxihjcle.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uaxcgfcd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2bzvjsbqj.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jubcjyfr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2okpcuoqb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2imgxxvgj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ogpkurvs.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2swnsulij.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2iqhxoyst.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2cnaneleh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2idvcgmrr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2iypamkab.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2uvahzvbe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vvqpoyon.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ktpcfgkn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ilklcgbk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2esmmkijb.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ywebsvpf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kddqzvdm.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mhhcvlyi.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2aqcustpt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dgqkcqee.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2jzlnxzgv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2ggyhnllv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zhhhauuf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2rxjgferu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2skuduizx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zsowujqn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ilgxnmez.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bjxvoldi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gkfxpmvt.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2dpmwmuib.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xjmahqrq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xeewkoye.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2askqomyb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ajdlesyq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zcandipc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2fmcfeqdr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2opkfujxz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2pujbxmoi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2tveoxgqp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2avzgxvcn.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2jwkuzoul.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2cncprjdn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2nwbhaugk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2senckvnc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ytmyzrso.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fqxwkrqw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zvbtapuq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jdgmtkqb.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2fdnsxcnd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rxybdptd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2kisqhqax.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ysqxnbdb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2rdccnbge.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2fxspriua.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vkczjphp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2eosgdntx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xylhkzod.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xsxhymwe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2wyxogcwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtjyrtrd.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gkibfdfz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovggntof.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jhuuolne.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2byufkvbi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2xrigiwvt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2chipkali.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2yronmebv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jxqshlkt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2vcthhrfj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2sasxmldz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lvpnnvyz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2hhmontdq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2fdqrfppy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2rasfdhuf.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2xpdpxlct.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qxwurqvd.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2duiwxxlm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2njkpmreq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ceamhhxf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwenqkbt.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2qsblpehw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sojlrner.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fgrlcftr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rdftgbxv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2lxneaeqi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xnhztgly.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2fehpsoif.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2schlzurp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dltwlrjy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xmvnipcr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hhgfaswk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fhmuusmx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2arxkftls.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2nztqfiys.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ckhhnszt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2enyrxxja.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2toxfqlnn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vzhwesff.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2xtmuavur.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2dfygvgoq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2breisxxo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2waeutdiz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2eaoutqin.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wjdqcqpo.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pirsbmyu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vlstffcc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2codiywmb.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2cfjjegvn.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbtjklk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mslngdyi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ysxlhetx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2wmsoiqdf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2prrqkbaa.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ucekbeif.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2qveiarwb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2celkajeb.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2qkplrnrf.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2skzniwwe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2anrqjqze.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2yqmqujad.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfmqcdy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2kzslihie.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2jpmtecjf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kqqgugtg.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2naovqaqn.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2wfmmbryw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2satobolz.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2pupbqhlm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2fhgyefqx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2ztlokuda.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrmgpwwe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2yjnmmqjt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhrqepcj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2asbklgwe.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2yfmufncv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pwfcylth.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xecfbnfp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nuywqkrd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2tjomgtjb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2owijqxez.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxndwupx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qqrzovsf.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2lzqrlpck.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zuxctnow.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fubordzv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2bcbnynde.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sskjfnkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zzsbqyhi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2pitpotzn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2iwyiybhv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2plhqxvnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2auqtxsqu.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dmjuptff.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2miraippq.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ndovxand.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2gstsxhje.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ergnreyy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdbwoiy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2ajlbztih.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jfjafksu.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2jmeujegm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2wpsvnydl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rshlvzcw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2yacnofkt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iicdnpjy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nypvsrcs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2dqnrhjnr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vbuodsel.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kqnklwch.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ymzsiubl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rctlmtif.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2jnxfqusb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hxiumkix.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2gvuzqrnu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2scrvixur.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2wqpchqkz.html


<!-- 参考信息 -->