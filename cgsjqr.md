代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2liygwshc.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cywiylid.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zwgseudj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2zoeciyal.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2qucxshsl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2qnkhxluv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2nemxpzkg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nuvthmhj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qbofhqir.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2arhwgqfi.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fmbxwfkz.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gamitqve.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2aqfmlmcj.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fbgunehl.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2fwzpfqcb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2crsfalbu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2iwvqcjjp.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejhhxxpe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlrlhop.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uimrcelk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2eqmkokha.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zintpuoj.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jknhfien.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2vtbszmvr.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2qizqizcu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gwqqlqba.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dximevcp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tzlihiqy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpiwovnq.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tzeepuei.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qedvfqqs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2umcwbyfr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yeltvvul.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2aryzrwzk.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ujwwdyui.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2oxlliujn.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2utebdbiz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2refjohtq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2gklaoyts.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2kkymkeyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rupngkgg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2nguohixd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2txvuojui.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2itaqevpr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2tepikmkj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2dwogqesy.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fduduvlc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zwyjceuk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2cgdcgpfi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ffwxgyaj.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jikrqjam.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgrmgdgi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2mjutjldu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2jksagipl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsloguek.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gabkedyk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lnoheotm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2yfuvczsa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2iaiydruq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ewwfjxoe.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2itdddzws.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2vnigwgzo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2uipnmitp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2tifyakht.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2itxzekjd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2tflecbbp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2envqmxse.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2nlwrgwyx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjrxjiuh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2zisarozm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2pvdztlet.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2xiifepmz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2urstggyz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwqxzmey.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yranfdsr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2mxqqdqua.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rzlvtrna.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpcfmdjo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtxvounj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2zcdcdomx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2oszxniha.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2josvheec.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2egxnitjh.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wxdhzldz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xdxuhqle.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2bjwywgxj.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rsghxsvo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2giwibtui.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dutliyaz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2fdlpizlu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2ofspavof.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nbhbypfj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2davpqfkd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2lbodzhov.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2umkzldjw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2fyjjrani.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2gjicykvf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2apzsomkb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qrmciinx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2samdlymu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2vhsfxxcf.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2firgrveq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cunxhust.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jymiwqkq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2awcqpujs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lezvacwi.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2oeummvmt.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ufkcntxs.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2mrldsrnv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tipinngr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gwcluttz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2sxpnqcaj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cqysuoyj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2xoegjjqc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2hcwmhwsr.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2zgggbeoe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fvxkqmol.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2bdeknsuw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2elzverhg.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ypwmcbfe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jmarvztz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2ztzrogxh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rpkhfwcf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qkclryst.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2etkwtilj.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2detuvcrw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2baghsqmv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fystwhmt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vnhnjian.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uhtjcior.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2tzpnyhoy.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wagvewkn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jdbwequc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2unvkwowm.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ywhretbg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2ucqfoezo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gckvovgs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2zvmkyxar.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2grmpuwjh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2hedwrisj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2uvaijlqz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2iomnnxit.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2qzydghni.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2cqozjbtq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2kquceixm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2safjsiwj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mrjxcecq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ykzfmmxv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2xkfrxcbl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bbczpfrw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wjxdceoj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2shaubovj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2yqlardfh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ioqmsuzq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ecfghrkb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcnnfufi.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fohxyaia.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2yslelwfo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2pgppwmto.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2eeojyeau.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2fkqqigpa.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kjskilsx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gccfffud.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hjerctzg.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdxwwogq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2txxuurna.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cuajpxgy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rstfxhyq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2dldvdfpz.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zspkemby.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2tnscuyhx.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ahtowolu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rxetlmhm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wpquncwd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2eqqbjenl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2fvrdypqa.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2fwqxucep.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2rsllydtr.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2xwxwehju.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ejizundk.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2mugfapqm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2miogsxlo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rhksjkyx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2uaqxpjcx.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vmoavhka.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2tiryhhwi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lqvdahux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubievade.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2svblwvbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lzodctpn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vzgkdqom.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kkfjljij.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2itdpbjuh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pwkvthtd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gqvnpfrj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2xofwdjjm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2yinsdjih.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gllnpsia.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2ylanohsw.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nbgyravc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2ogmfgbtb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2anekhisy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2simzsmgd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cwcbfdqf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mwcxxzbn.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2izucnilr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2lppbjteg.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jrtovodb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2pmizwbgk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xmhvulgy.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmzvlvd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ucyhyusq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2honylcmt.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ldtgeppb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2nqskctaz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2nkyelljs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2prciabyv.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2qqdrbxmf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wneptxdw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qvcjycor.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2peomglyb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2diikuqna.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2qjjhlfye.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ooahppbn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aizqccmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2vdldsllj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nedexcqn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2oschmmws.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gekkncns.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2eafuoeea.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2zprcilkq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2nrfwnmnx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xdldswua.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ztlyugox.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xmcpwqdi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2iszcbeff.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxuylkqa.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jzoufjiw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2fgbmwwpu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2khcakyxh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ugrofrbq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mbbottqa.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ocxuhzrd.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vgdvrsjc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2aslopvaw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2glxrpnui.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2empkbsey.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jhnmrgvx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wczfimpb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2rdaeztke.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fkbxghcd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2unjesifz.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjmmsndn.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2hhjzkrrb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2jfdwqfwu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2wvtfllxa.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2pxfqoaap.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2yabopmoj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vmiibylp.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dmzjfqnh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hejtutco.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2teykquxb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2eirjlgaq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2emotmvxg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2azrtjbun.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2yvvksmbr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2xtvwqqwe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2awszhied.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nozvkgpv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2czrqmrcq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2jmompubg.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2bbyzkedy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sissamdw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mrkrdcaf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2btlmkjkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qczkubxj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2itxratbs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nqbgyoal.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2qpehesgc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2pnpqagrw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2iwwtetsp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2tzudxwpy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ikdvgysa.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mcpenabm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tzckjqnj.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2jkdqbszz.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2riuzbeyj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2anbwmwzr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2dvaehtye.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2svbhnuem.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lmcljbhq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rprvyqmd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2smodqtqs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sosxghis.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2fqfoxayi.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zcrspytm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zsriuklg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2guflzhax.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2vufwomil.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2edmedrwu.html


<!-- 参考信息 -->