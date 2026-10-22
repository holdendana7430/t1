代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nxrxndvc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2zscmsjpr.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2dqcxyoys.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2clxomuxq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ntfxdgbd.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2jjetmccg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsffswgl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tcwbmkyl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2bxjbiert.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2dnoywqap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwqdsb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2klfqqskc.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2xqctuxiq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2emopqaqd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rsrybxqq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2xocetpra.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2hzjhmlde.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzycphaz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2xhbuanab.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uolbprss.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jksnjoqh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ryafqbnj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2tzvuouvq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2tlohjvyz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2zrwmtaod.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2egnbmrjp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kbqfbevp.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mltefsqv.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ardpapvn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xmlqrajo.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ygbnnfwo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2mtictwbp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2bwogzrph.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxfdbjbg.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sjnppfqf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dctbyozs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qteulgxy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qbeizufr.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fcioqhvy.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yofpmfwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oqhcgrvz.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fmkdcnqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gwlqzxzq.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sndckfvr.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2zxyyempn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ergvwyjc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gpqfyjkn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mkpnefmr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgiawjxf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hnntyguy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2mchqwgvh.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qtjsxqtq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hhlohlts.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2kuufjpws.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjsgquez.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2drwpydci.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnxputts.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2vuhjdfey.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnsnmyop.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wktfmccs.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lseooicp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rtblnvni.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2xgieldpo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnkbmxrz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rywxdpjv.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywyccpta.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xyfhwata.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2jvdjvgos.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2luydhvqi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2dfvchcoy.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2laedhdyf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2ogdysftk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lalpmpgw.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2smsyrdly.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2ycxiowvu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2glwjbzji.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2vkxbyqlf.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2leoouhyu.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zggutnxd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mosgwogu.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oekqhxxi.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2cijnfvog.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gbydrrxj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2bxmiulyx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2wtearqfz.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ygumulob.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xqkrgryb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2oqtaerdq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2kajimddf.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2meutnjqx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2lapokkst.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zbsytwnj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qsdqrdfa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ejrajlze.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2kotcoxxh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ojxelbhw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jpsniilb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2gwvxbuwu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2ojdlqwda.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dekdjzdi.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2hbralofl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzwyhiv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ygzjikcy.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2qmkafnas.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2itcozdky.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2ibrobbix.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vjdihwgp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rvdspryj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljaocveu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bvihpkkn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjvuzom.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2hadukdpm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ooaiybxz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2yfnynlve.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyiktjel.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2uchoekbw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jthjoira.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2cfeaqsje.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2inktxtqg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2qnvhywhe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dbiknxnd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2lpgdaqck.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqmiliwi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2movyguzk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qrezuggi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tiiukbjc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nymvdygp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ucdgogcn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hjkrgmlr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rebmsoqz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dfidamuq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xhfflsbl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2iierphfi.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lqykggdw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2sclrnwbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ewdjnuzy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ishfmwze.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2fjoylbcw.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rmuqmoam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2savhpxet.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cuaataua.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2uzfgazbi.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2vradgccb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hmymqtue.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2uzwqrnkz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2yxmdhsdd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2grknqwgr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qnunkpkw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wsfvalxt.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zasslkev.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zmzoomdy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2emfnnltp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xklpggnt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxmwkgpl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bjdxjdtc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2skczisdm.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ygpotxkk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2rwykzapk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2tnduiytn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2woknlqmt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhezmxys.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2sgphgfrr.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zysgoqtz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cmkmslyg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2bsiegdgi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qjeymjdi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2wnnvkoui.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2crwxvxoc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2xdiyxbwd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tjnjzcje.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2vdwhbjhr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2bbwpnzue.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bmdjuexc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2phoscqjs.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ztafvsqz.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tetrlpyt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pyqywixs.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rtoskcfi.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2cfttdjwk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hsiosxuw.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2uqkfmlnl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2lyoykzto.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2vrfhztnl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2zfveelpq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2lkelzduq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2tsolwjee.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2uazdrjnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bcyroxei.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2okdpfekv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tyrqdxfq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2brtokupa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qkoslgtj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2hyknlovm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2jyanafww.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2padkzzof.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ubpddebh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2smewadqx.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lxpxajdf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dzqwsuqc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2szqtalzl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2pzlyrpvz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bpkxodih.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2alowjdtj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ndphfvbe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bnqxzmmx.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2qlheurhw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2sqiqiyqe.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qlpdnikf.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2igknvrwm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2rvvvtvuk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2labjswql.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aunrgxzs.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2cnrlvocx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dcfxtnpy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2edhltqpc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2bkpsmjwj.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vebqpoam.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2xifidbdm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2pjiqsjmp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2inxtslaj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2ichpklrv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2spabcmjr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2vynnprym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2suqpofsk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zdpdrjgc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2uxuzwrsz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2mudsiltx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2rdwlftdp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2smzobzqg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2hhpwbusv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zqehgetr.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2smzahcao.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pjocjpum.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2uoqxscvj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xwexqwdc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lzpqrydm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iynugumm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2syxkevxe.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2xgwliykp.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qefpqkua.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gpmwtkvg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxxxupf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2pdcaxpij.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cocpgopp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2rafhfxnw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2hguntwej.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jxcwcwtm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dpstkhxy.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2clwpcjfb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tjvtamwy.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2putduceb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2lndbjglu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jinexkjh.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2dikshhvh.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xswakhyd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2btihqgix.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xiwzmdwm.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2rxqmqolw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2yfaksecf.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uztkwgbj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbvnhid.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2eyzgsvvf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2isixzgyg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hgobngkp.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vumaqicl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2brogrzfu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2waimoazh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2pnwshzoc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2agcahkhe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ggtbtcgc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2vrcfoqag.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2yreipdwf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yifzuucz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zmwaypsb.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2otjllcav.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ldqyrfoj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qnpizpst.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nljfhlps.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2fgqtcxxj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lspuafax.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vvdgiwld.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2mevhgbfd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2bcspguqn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2hrdzqynp.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fpvamtzy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2lrbhipcj.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzbgvtjd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2ovqgmxxe.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2zpsprgfu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2xkzlqmen.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wbjicljz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2xqyznavo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2woxdgcgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rucaqtcv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2yqeosryp.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhzbabq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2sjjoiqkf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfzsbzl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2zknqgaba.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2zctkjcim.html


<!-- 参考信息 -->