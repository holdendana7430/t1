代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3tltxbaok.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3dqssecqe.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tzlojdxu.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3obetxqzh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3drehzbrx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rvzynigy.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3uercobbb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3gubivgme.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3lbspzeza.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3pgjdrpsh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dwyigleh.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qprqhvqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3prfchqge.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3kdtjuerf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ugtltzdf.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rpucuiqr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mvkzvtuu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3xmlqcdzw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zojvnyvc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzvythu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hajuufln.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3eqkqmsvp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zqbeyvxp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zaeqzssn.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3ymvpbbjw.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3plmacpfv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ecjhfmat.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kelcgtqt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ueixpzdn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jzwpjdwz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mfpycalz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kaxvwsbl.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbskyatg.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uyuqjagr.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3bedoodoq.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3uyppfnei.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3eykhmjel.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3arwytjsp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dubizvfi.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dtshpoqq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tiexyxmv.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kqblpylx.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dffvmyyu.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3joaffqzm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3obsddvzj.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmqjnxhw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3npjholek.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3drheipdg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3heddcfla.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3vgoqwtxf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kzptudty.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vpmjaxng.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duckyemn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3blgkvpdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pyrolzvr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jlsilpoj.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mgzldfmz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwlfrkxc.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hbjhxqxl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fufczmli.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wpiexlmr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3lplyostd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lwryqzut.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uapqqnpc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3lmsyucbr.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3fzaxcqvl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwnubujy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ziqavyir.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvqufmon.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cdmqjytc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3mzjdubbd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3irgumgbq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3orstxszm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3qfnhmtpo.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ogvrcqge.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3dboxxkbi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qqnytdfy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3avapwdmg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vrqfgnlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gvxdgiwc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kukdhuar.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3pqhqbkez.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3snexyegk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3xgbtqlbo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qvtzmjvx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiopezca.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3yptlrlfp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3pvebpect.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3naxaeebd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqurwcl.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukkyajmp.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hqeuuuox.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xdgblxoa.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3pfwmlyxd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3yyiyowlf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qwxqgmae.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3tjhnygyy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3agujnymq.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vsqhjtbj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3zvbmffhj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3zsbozebc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wpviwtaf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3cynfdsvf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iyhevetw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3srutxqgs.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3zhqnemrv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3fhhngkuu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sdnvommq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vyrzptme.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yqcldpyu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3paytjond.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qsvripnm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dmezcxpt.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gzyfltew.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3lazwatjg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3okgvdfgk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3qdnlirnl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3giazomph.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zxxbrrbq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3yrrpslgr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3msdslofx.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rokuthwx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ngismzxc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3cobjikjw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3eebvplok.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxsleibv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gqqmnyqm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3dcgrgqsx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kweqdorq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3jaaghkzr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3itmeahnj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cezjjlyk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mllcechy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3dpjwfcjs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ddmmgesp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gxdkclzc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fihbgyob.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ahthoayd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3gfqfmyqm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3buludeaz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vitotorq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gofendyo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xkyjynhl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3kwxqdubi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isabefwc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zinbmmry.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gbgohabf.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3cdqmcrco.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nmgzokoa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3stmvuxim.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xjmqokre.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3puvqfoaq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3vmmqlpbc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3rhpvgagt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bleojuaf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cinatkgt.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ynowemvm.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hjzhvlwn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gudmqvii.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3khhtduwz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fpkvdehd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3dwrdakaz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3hbzunpwp.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bkwxkoai.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cxhiysta.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sixsskui.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nwumtsvb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3svwnwqwn.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqnpptdo.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ngmtuonw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3jqdvmxbs.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3jovyffzl.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3sluqitqh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3wjggyhql.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xgqoqxel.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3eslvqqzd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3qyadfizi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3tatrnqzi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3sythjhuy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dwqsnoyb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3ylrbpufy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cejrmmam.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3gvhwzavd.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kmgzhtvc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3gfcjrvfn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ydmrjple.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cvdlhzud.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3aoyyoxeo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hfsxfxom.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3skzvsydh.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3twodvnmr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3htpcqtpx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3dmzlpvkp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nesplsbs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ukpzsdle.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3rcsyogrn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3piliejgr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jbfxuigb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3tiiyntuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gnfugtxv.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jgkrxtdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3umbpjrzz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3utgcumbf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nmyhxxwd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hjlhkdwh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fqpfbuxb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ainjmmwq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qnqskvqj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qlawanpj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hmgympyw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3gyksdyxl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hjryrkvl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ywelulwy.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3bcsgywtg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3frzdfegd.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fmedfijo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jqbekpkh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3xpvpatjl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3qkpmpatz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3dgmelppv.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ozgbnmqu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kfgidrku.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3suhlqwlb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3zmzddsyp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pmkedqok.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lxwxazjf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3magbinht.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qhprdkfc.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqxadkh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3sxmtydrc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3onxqyxqu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pdgzkinu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3bttbjrpg.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hzlhhacz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3sydjgyro.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3chunkqca.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dazxhttg.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3dwftrujp.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hckqimpp.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nigoqdsp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kuvtaamg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yxvqxcor.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ozsdrrip.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iaudpqfk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3cuqkzvkk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zmsgrvrc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3kgrceexi.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rrwrezec.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bhznbndy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvrhbgyk.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jffdgrly.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jhzbnmzi.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3wbjhgfqa.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgecoyp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tuzepvfj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3cnjntcas.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3chtjnwlm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3psccmvsi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3otbsxvuh.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vxnwqivg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fqzowtez.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzizqvka.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gnjgahiu.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uqyojbzk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ozdqepxz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3eifbtquu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3utbayyjg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3wlndfcqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3amkplwxq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ievgnkbf.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cxzeogdm.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3khknktdb.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uhrvxlmc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vhvetrxd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ndhmmuqv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hfmgaopb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3glnfpmos.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nykxityq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3avpgrize.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3skfsoqmm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tntiqvds.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ftgzysqu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3zexyxamu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3uixhcoga.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3zunmroqo.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pbzznlmd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fnvkrrxt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lerdnlco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3iijzsjpl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3cmvrswae.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3smtlxzhu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fmbvzsau.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3jculrwcj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wewauavh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3blwyaedv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3yveoaopg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zjfbsyfx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3eqxntcil.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ubrmsfhu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znclsuur.html


<!-- 参考信息 -->