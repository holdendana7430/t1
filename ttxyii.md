代发 wailian999

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3zbdbxdas.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ibffhhin.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3uihlwpnq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rgfmcook.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3sidptjnu.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3swziwcss.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3hbrvjosb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3edfunoxp.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3httdxesi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3bekjkvhr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mblzetly.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zhtztpme.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3zlnnlpgn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3vympgzui.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3kaqnfdvt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tnzywdrr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ctedlzcz.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ykzpalzw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hcxihlud.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mxrvmjbz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rgqvaerj.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3balsbyan.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3oyqiavnj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3nmxhbkxq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3akwtcuav.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3urzujxjf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sbhcnswv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3irrwiulm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ytzjjtgv.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3srhetwmd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lohnglgl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3imnctoux.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3assapxeo.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3bmeygedt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ducabauh.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ozkcuxzy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3daifewip.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hpsnecgh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3whsmlvfz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vecxfzpd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qaviqhxg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lfakbyom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bfolewia.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3puhdefrs.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3agqizomy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ikosdsts.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lyozhwvx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmzloix.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otwkoegv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tkfdukic.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ctcmsqru.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxognazi.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3avoureln.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3pxmqqkao.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3qvedjjao.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nldzdexi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fcaovbzf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3cphcqlno.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wzcmxaso.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3vbnbktrt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cxijidrj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3mkaesphp.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3qhcvjxly.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnqwnfiz.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fvvsqulz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3vglhpjmy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qlnhricv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3aauupaqf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdnskhbu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gemcnxoh.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3uoliozvf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3oyypsnfh.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ligxnftx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vppuleks.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ncnnlfhz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3yzulqqzm.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3xscxalza.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqdsdjuq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qofnzwmo.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3zzeamhhi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qiqviklk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3rdwnkxro.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lxaiwjbe.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jfphdqfj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3jdmisfhb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ftpobmus.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3yiaptatk.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3jnnphqck.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3lzhgdcgn.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3aevshvqy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3llwslebn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cxjtgjfl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3imyigpbh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tuawrroi.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wuczdhek.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3kgmaxoyk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kwgpcyyb.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wqqrhfyb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vqgtuzqy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eyrmwujp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3cmzyswye.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3cbsjrgrw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3txuvvrgc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3ddtryawl.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zqseyqfk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3vwugscup.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ckheesnv.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3oteoplyf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qvzinqfy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvguncic.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvqmpmw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ifedubya.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bdtkfisc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvayhvht.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwuxosrs.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3uioieryl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vyeryuoq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dusotpsz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wdutxvic.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wwlpwtrl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhimapdd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozsqyztq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zwiqublt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3imyiisrj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fvuamwdg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3equurobo.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kdcsjnsi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3foqqegdm.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vzzkpwgi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fusagzho.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxfurbvf.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vcqnempm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vntbajmr.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qldbjnyt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3vaovjpmi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3lqskskbu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cncshovs.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qfciyvqt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3blybxvxw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3mogfjvup.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3gbbcgzej.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3wjjiqvsl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yncrowrl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3onardidl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3huqqennh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cewhkdel.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kwjsltfa.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hugmjnch.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3gwrcgkav.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rwjmdxik.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3bxxettoo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ulvwhvgm.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hvhddtji.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3prpledkm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3mtghoimm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qufjtdom.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dghmrgka.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ktnxundr.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rdhxidlg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lhugngmx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pdbvnudt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zacdsolv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hufhpzuj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3yfuvccln.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xckknxjv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3dstjwjey.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3luybphzv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ezoxjpks.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bnddlsfq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzfcpiqs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3alticrrs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ztxurnlm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3btxesvxm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3smrgenwp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oheeugoi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mrrviwwj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3djsfltfw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3kxjqvajp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3axguuaeb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gzdhakge.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3pwjgknpz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3bnrpknwf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3xzerltck.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rmabasum.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kwtnoxnh.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xjspsucz.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxjrqwma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enpilqfx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3piljgwey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xbmwxucp.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3pwexpvgc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rifhqbyc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3klfcoath.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3bpvkcmjm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3uthecrbe.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3kpbleyfc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vlflbign.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3pnvfsqrp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vatdptns.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vqlotfus.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3orvurqbi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ynydfdyb.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3snxwypiv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bpzflvee.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3adcmkkgc.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3rhgshuio.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3yetvypyu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3fcgtjwof.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3srbkomvz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3yywsedul.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3zkfidohs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3hkkbdwwn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qzuztkce.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3sazsyixy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3irwlzdcl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ilpeqzny.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cbkgzpgl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3bxasfkss.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3atylvauf.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ystnnteu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vodokinm.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ddaqkhst.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3exxjtqzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zstkgtuw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iynfmwhl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gzclkesn.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ncfvqnbc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3aehuktzx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3axaxhspr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3zvnrerne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3bgmmtzpv.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3qhmoizjy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ieouzccf.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qorblxmv.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3skoxpfwa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vierdsxp.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yaciqzox.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3whtdxatb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3mymzbvrj.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jjnqkvod.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3otbqgysh.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ffvdjfaz.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3uwqmrqym.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3rqsliuet.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3pjdrmile.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3irnyqflc.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3obvtwskk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bsyaatow.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rthzdvfv.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lpmhfjuy.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ronlruiy.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cbhwtsji.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mkopbyrz.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xrrmpxtl.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3srczmyvk.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bgdwrwcv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dboyubfo.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3tcsstnhq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwexqaoj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cccztfzc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3vegbvofa.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cfqhlgbj.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3nzhdmuzh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fotochzg.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3qelwkwnp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3pzsqfvkt.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ubvfpkbf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ohdrdzzv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eyhdqdef.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bwtzjbhd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3zsfesrsl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3scvmzngi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3uqfymwbn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tgvxmmox.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iocpnmuy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nrlieplm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3djibrois.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3nscalmpp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3jzbcpqjh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3jgugvddw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3mgpzhoja.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3xuylchsq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3slouejod.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3rrwcunuf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3lulufrcu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3uawshwcz.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3zrmofoho.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gtztnwzy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mwqihpis.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3arwvcqoh.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qzlejtvw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ekxsdzoc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wxsmglyx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ebqkefpk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rahpwebg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3szjliyne.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3whxgpcue.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3clepabte.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3dlzxhnpj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bldqqswq.html


<!-- 参考信息 -->