代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3xrokaxur.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uudiwevj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3fesoedvh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3acpzelor.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3joctnwds.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xonmmjuh.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ojfivxiu.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gjsjofgw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3yroaqidb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jqpcikes.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3erylxueh.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ymtwxqde.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3cqtzeinx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qsvbsros.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3akjbstwm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cjiotfyi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wgghhctb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3arhsuqxb.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hlfilzok.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ldjvtrob.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3dvvfkgzw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3jkwhjavy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xlgxtiar.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3zfuuijcj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3ocrnibar.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3afywjfrl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3teujwzzl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dtrqqeoe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aibbavfs.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3lrldufng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkwdzeil.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3psjgguwb.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3xtngmhny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhtnzels.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykiziizg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbihujhw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xowbschz.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lvbthgbn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnbdevsq.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3awhbqwbd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3trdxikoa.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3icnvjvht.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3rwenyznm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wqylwgsn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zittvxvl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3ktwijzpj.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pczdssre.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3uthewqck.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3oziwtcwq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtjezgry.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3ngonrkwf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3qqkkntwl.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybecfzpk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nshavogf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3tfuqiqoq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3sgbodbne.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3bqzvckth.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3engqpsgb.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rqiqajbj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsprqtn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3czjmtwwg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lrysxoaj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3ftrjomgs.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3rhgdjbta.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3purebere.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3yxjrvyvf.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ipsbtquz.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3xkymrjht.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lbifvhgm.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tkgzioqt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3sysmxksz.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hnulzbtu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3etrjheso.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3jaqvdtcc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3snzmoztl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tweucwbm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3xdnjnull.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3uujkqiux.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ciezmcdn.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fvxholzt.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3uankkhrg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3qsivgjsk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hpfpipjy.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tjquhexd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jdmbwbip.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yqbpbxde.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3spfqeasw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zkmbuttk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3nxbvepcd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hyarwolo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3chitvucg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3nueujaow.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wnvmouzg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3gtrjznin.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3wooubvos.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3legpjvfa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mjjxfwbd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhkfwqhd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fyzvjyxo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3sqiymyyh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3cegbizea.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rfsqvggu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bfeqtkng.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3msswabty.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxzmbsbu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lqughbij.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vztbewhu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jpokilwt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3nfwyjuzf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3qhhixgmx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3binubicu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xsguksli.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wcwpqopg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3tsojyqfy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wpfmraxn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3knefqeey.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3tugcpnlp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fftayoxr.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jenvdvvp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mldjiutk.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bilataiv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dxuibubc.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3fhoxwtiv.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3oexohycu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3iofkbkzu.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3jjwsfipm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wnnmsamk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3erlakcai.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uyvecauz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3auuagkmj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zkisncxy.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3arsqildi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kfvrfkmq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3nbmxilyr.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gyelmalu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tllikndo.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qrbrnaos.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hbxbtqju.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bhzbriaf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tnjkkfyl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zljnndhp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkhwpxfx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3wguikhpu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zumxawjc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fbdbbfcy.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3vsdltasy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3mzhorgjz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3amwvrddn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3qaywynqb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sikrmcvs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hljcysqp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ppwytmdp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3zimourii.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vumcmpyp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3slzldxfl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cuwgyyep.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3shskkviq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3kfmllcoc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3mzsdpbrh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kabyrxol.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwkcljqk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lrgzywjk.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3btbtuuth.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3drkbiack.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3bqselenc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rawgqqpw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3lapxamme.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3kbrvbitk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3svdnkmec.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xqtkcvsz.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3jjdvjuzq.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhwduzmo.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zmbixsto.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zckbdclr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdkbnzoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lmxgdxke.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wcusudkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flsidgla.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qsacozba.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3sigljvnu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kqtzjvyc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ydniwasq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3dzrsckse.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3aqkpmakq.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3bldsqkgq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3bgzydjmc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3orbwvnwz.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xrapsevf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3avlgzsnp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3vbeabsjz.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gjpssyan.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zaunnxhr.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ixomaiml.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3shzuiyld.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3armbkrom.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3okfwtdue.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3isjlsmww.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zzhuczpr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3iouttoss.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3mxexwzyz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jbrunbzx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3unjmbpvi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gbgwxvbn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgxwkcp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hemaiweb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3fvwyudtu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nhfzvyfv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3syktdivs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3mixzouya.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3oxsxekdk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ietlrejb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3tcykjerh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3huvegfij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3lvqjmqrj.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3qikdnifq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lkgrlbdm.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rzinotts.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kvfvjjea.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3ewotdgmi.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3jlwyvamh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jlokgorj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ajltcqtr.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hbyqjeit.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tdxoozka.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3frkzrchn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ypijdlrc.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3sezkxeog.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dpltnakj.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3phhiiari.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tbhdtvhl.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3pabawxwj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cpuvinxn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3abhmkqhy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3kwyvbgfd.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mlnjlpyy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3guawuigi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nrrogzax.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wexoqgzx.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3hyhojaos.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3eephjtze.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3klpcdibq.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zulgpylc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vabfampv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3gmuvknqy.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ijoosqpn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3afnwslrs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mfckrpye.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3mswcheds.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3jmwmvkah.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fahmebts.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3lfsfzgap.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eaqpmhve.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yiadsupd.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3wwstihwn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3brhpeclw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3dreikrgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pndljgry.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cywsqqdb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3dgeqbqev.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3upvszoka.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3rrcxznvp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3afxssrpa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lszulskz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hjhefviu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3tskodkan.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3adkwcamp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3evulxurl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rhhiqwmz.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3llfmsqhw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3hpjpugov.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lwnmpiyz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3kgskmteh.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wkruliyv.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vdhdxfiu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cgmzogkq.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ppexknri.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3bximicqs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nchxjcye.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uaudqdqt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3yiskorbi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xthxrlir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3eewwfgfc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3tzfyhyvb.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3umukwzly.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhkbezhq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3arypmmit.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dlcgicmt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3pyyyvxko.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ylgdigfl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rufvyvde.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3nacqtkpl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zzldhhgt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3bqzotgkm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3bxncpfub.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vxhxqkqv.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3aqshgyzi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3wknmwgxn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3wshjdest.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3cvrxzlxj.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tqchcljd.html


<!-- 参考信息 -->