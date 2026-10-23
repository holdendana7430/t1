代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kksjlvrn.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3hpnxivlx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3usrrtqrg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvwlihra.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lvkpadbo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hdlvaamb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hfpidlwd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3sccfepcb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3teocxpcr.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qemwowim.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3rogekaie.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3quhkiqdm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gnvfjdrr.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3eiasrhsn.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyvooeu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3osxermdh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3uwgyvocz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3bountdya.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mmxfeays.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3uakzcifd.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rspdvwoe.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3kliuqouk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3pfwsuhbc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3awewzpno.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vghugtvw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wkhkdojn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yinbihvu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3mcainwqb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kknrxueb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdnmskri.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3vnvrsikp.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3wguibggf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3sbeqsjpv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kdnlbalr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ystzuall.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tzbultnd.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmrojxbn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3joyowiwu.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rbwgdjvx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3smwaajct.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3bevtvglb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkdajysf.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qqimhgtk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xmomyjft.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mfxlaags.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eldlvmji.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wmxfhdvd.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3twoyyknh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnbxhhmw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ljxhxcha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbzeaian.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3rnvhtvdr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3lxsrjsqh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpwfckgh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ovaowepf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dveipqys.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fbmkpkhs.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3kalzifxp.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3fvoubttb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsfejbor.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3yblahxer.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3bnvxcouj.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3gzjjypyj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tlcgsipo.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjltpxom.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3okqcjqad.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tstujziz.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zgvlizqk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3zkqurftv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3zkjpchnp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ymfupmcd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3bufcypvl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3elbrvpkg.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bzzggmuc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qjmveyoz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3opdnzdzc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rtdglmyf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3oijrvhyn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3jvyzhvib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3ywngohse.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mpyoradl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pkigmiis.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mumoljgd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ghvyplei.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3sjgzhazh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhpngbzp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3razmnqgg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3dcdxjhsx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3vojlbpfx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sufcxxvt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ihitdsdv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ivhvzqws.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3tngmpsne.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kpguwwtb.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ssougdzz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3pdnvusqh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kzytelnd.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3bjbbcqkn.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jwueadni.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zfrxjsua.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vftvtnji.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3teyqswuw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwkgiqz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3sssdlnov.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3sxcxnpsu.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3rqhqjqtk.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3jwubohss.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbkpegxc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zkxmfnee.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3loituxvl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oivdnliu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3jcgtfehg.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fhaypjqr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3feahduxd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jsgvofyy.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3bxxsifac.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrfrhmnd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zumdaucu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3usjnxpcm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3gafybggt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ctlwtgcn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3achayksr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zefyjhja.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucdqokok.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dgzsrees.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrmqlcdu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jqwmueyv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kjqyeghv.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3vboeaayw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxvzjpw.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmofcydn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xcucglai.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lerzjkcv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jmfvquhe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3qtdxracg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cggilfvt.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3wyqhzmjg.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gytqcptq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hgoaspky.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3dfbcwzof.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmvazise.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3qhgztzbb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3xqsvsveq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dvdjvhga.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3fkebkxkw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3szbhhitf.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3xtryzqgg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3owcvoyrk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3wnfzmywv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xxdiipnm.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3koexlhbr.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3nwucpwph.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3wnzizgwh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qzddydgh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3peeobwhd.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3mhjkwlgb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3eacqctie.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ygplxsta.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svdedciy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mekzpmiv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3rnmmphkc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pihilpwx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3dpeclvui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ubaovywz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lrkrrxam.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3psuuzsvw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jvurfxxd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wkogrhwb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkwsrlwc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3caxtonid.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dgtonaiy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cbgccfic.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zikasrrr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3xghzjylg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3rvdyrmoj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fpcxnjwt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wawxgoze.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mwymrial.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ndxoynyp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ygskjumf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tsueqfcy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zrtlorcw.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pzoxvdki.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ymfhnpfo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3iuuimlpc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mughyrwp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bnrpxgqe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3uaixejwr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3xzewlbzy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zfcjgdyg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tjxjgwjy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwsaxwuk.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3egbdqmon.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jjmyrlsm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ksgthgwe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbcmlvub.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tujjrrna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvgzydcj.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3whlavsou.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3bslmmjve.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3bvnwoeqt.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3illlhqhh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3gppsorgw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uteovrpg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oxajguxf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gppdrivz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3uxzlibps.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3yzcstsgi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3xpsmrpea.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rmrfgizb.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vcecyfan.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ixfujagh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ozvlutnl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qbljqque.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lwcqnuvo.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwmzoewx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3aqbwljbo.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3qrzqfdxx.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ficfygba.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yxtvpnmk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ozdcqxyc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mvibvfzs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lcisyyzd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3prjwqych.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3njdblnxj.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3hwmpcnxx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wkwpljqo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wbcuskll.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3zeyccftr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hdbzwoxa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qwdvfiym.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ddgzrtzg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3umnkjsyf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3auhsgrsf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hgomrrkt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3emeosbsv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fkwcvvjn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wcimrtvn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dfbpyusu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ugheqbib.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tmfxuxjt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tdvxczbi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3aiwwqgor.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3mtoycjum.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3qevujegj.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvupontt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3woqgkgcq.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pxbyrgvc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3akhepicl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qyuzziav.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3fpnyyftp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3vziwifcl.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mbdktrmd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hpnfvjzl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xwmdsbct.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3chjjfwog.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tccqnngd.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3atzmzeer.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3nxhqkvmo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3djsbkjkr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xqluridt.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3efnhxbpy.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3qavkkgqb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3bitrkvfw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3opvmkmxi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wmeadblx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuzvfzzu.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qtobyfsh.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ajddntxz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vsyllkef.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3plisnbzp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qcxnoghh.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ikfqdhyo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nqmgkdij.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ineklgkt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3qblfunuy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xvsqrjmt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qhsffydp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3qxrbjruh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nadtixbd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qnrcuebr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3uivwtsul.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sxtzanxk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3gnpsllmo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3blajfebb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3fhjrpubx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ifpvzhur.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qjhivlxt.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3djdflqzm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hdmysdwi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rfuadftw.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3xhabocxx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3bewutvkl.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3chszuauk.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3folqlanu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hewvcecx.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bmicsxjp.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ytqnufay.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3otequvdg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3surhyvdy.html


<!-- 参考信息 -->