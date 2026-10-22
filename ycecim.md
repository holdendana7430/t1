代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2iazcvakx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2pjthcuvi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qpawnvtm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jrpjogtj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2hqydkwei.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jnchykpo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mvtqepfh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2nlusllye.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2aqyovnlw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2otuzmbyz.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2mtuweazh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2qouuquyg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2uhpzrsxv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2tyzottjl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2fwfvjzzd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2aaizczto.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2wpfoakqt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yqgybknb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2jhzecrde.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2thbbrwkn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2umheosky.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qwujrfof.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ycjlwpie.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hukfsecf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bihphyis.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bviqqidy.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gblkcplr.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xehciiij.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2vrhdjgmn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ugquptck.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2klimpyqs.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hazdcoef.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2evojxqja.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eqmyokxe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2geopydjh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2voltvlpl.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2zreksazw.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2bhwlhuop.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dpidhtlt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnyhsyp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2louzjcsf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2qvkhqrdq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fqexjvgi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ygygqykv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bhpjdgqw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2pkskrmhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqdnnbtk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2aoggjzdo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vgmcbfmt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lyvkvjuw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcxnroue.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zapfjgmn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vtbakwkf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2eypcyqey.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2veenvqnv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vlmcvtbx.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2akdulwqb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2jgecbafy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2vpdasqai.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgldqczd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wlzlqdgy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2aohezujl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfhelzbs.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2mqnpiakg.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2ryeypldn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yfbjynsu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nsosbjgd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2aolzkozh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qzeldtxb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vxjyrgiu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2eeojxxof.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2dvbdifne.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2xxskdpdu.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2hczqqwek.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ubujtqey.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2upwxcwbx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2tgrmcwvz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xtsvqahq.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2vjdiqvqp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2homxktnm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2flfwkpil.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nlarlepo.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfpljysd.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2twflnmao.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2lzllsawg.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2dqowggya.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ravcknbt.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2aphwluvp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2dhgcjlkd.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tmsbojuu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2agxziibl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2okbxuluj.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2wltnqurh.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2hrpmnfrp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2igmvjynq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bcplbbjs.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2oigmymlv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2spghmlde.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ffqzylsb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2dpowsfsi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wubargck.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ekyalegp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2zxntapaw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wdpmveid.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2kcsywror.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jxhkokyg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mcfehkfh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2jozmcdwd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2kyqomzkd.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jledhquo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2fiphlqus.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2elxfdqgk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2oszbhltr.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mndvqqxp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2pvhynsgx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2xovwwxpm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2rqfamxyx.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2gghccntj.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2boslkeux.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2togetmhz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hlrwpddc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2kebnfenc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gowoxgye.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2iruzeqnq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2bwiytwfi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wlndtvzs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jxapvzin.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2tkbqxdnk.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2oimzrxcn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2irfslfjt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fubtaets.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2opmttynm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2adckvzps.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cfguxgtu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mwnmvbsa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2dxzhqkaq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2mpgwzzgd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zvwtvgjt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2opqidkca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dedmyutn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2picpolxm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cvmpjkfu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2smgvlqvm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2fxiogcyp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mzbsmyux.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2jqdodhgk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2ezvnnbzd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2wvaoferi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jxqgzbmk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sksmioyf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2iajcnkcw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hrubqmfb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vkcadcbg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2uvtdjdlb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2svrfjygy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wweezmqy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2rfgxkmlc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2fubfnqws.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2txglrsyq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahmdtyok.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmhfchzj.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lpfnnesc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rimrwiet.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2xycmaanw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2phbyshtj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qztpevgz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gnilhrnu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cqndtndn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ptzzojtv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mxqpwbpc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2gyoulelv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2oelejgou.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2qovehmap.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2chycbqug.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ifsdwqkb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qdameuxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ysljkapd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtleocht.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zwjeyzek.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2cejpugme.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xjjwrlqk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2fnjxqrwz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ergboika.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2uhskpdpg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2ajhigtxc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2asskkvvy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2sxhltnge.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iegheyzn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2uuointle.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ixcmmlhb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2btmrwdyx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhvhszxs.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yhwiuehp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gcqfzxfa.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2oxueyyka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qkdfthsp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2yrrkbwhb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zikfqaii.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2aeenawxg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2hngxmrnd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2icxghejf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ciestozg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2hnhxgjdq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2rayshwfj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2wdadvvpl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2gpxezadh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fgkpzorc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ysgmfdmi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2dobfwako.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2huvhkghk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qdryesiu.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wakarpib.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2isoflvjb.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ubfgnxht.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2sbhoswin.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2rvbcrrcp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2essnydkf.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2mplzdxqo.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2znuzyhqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mueybttn.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2dnlmaiuk.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2dfokkzte.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2dpvbizgr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2tpogoymy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dqevpbfq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2wsexccao.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2rxajugpn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2gadepdtn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wevwiemu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2prdkzges.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2fasraahe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bzadtoqg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2xdyvsgve.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2olcndhhe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2okfskfrs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ybkqdfyp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2whrfjsxp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wcfiriyy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2suokjftf.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qfjwebzm.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuuzpzwk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vniqbole.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2wltvbflj.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2dxesjvcf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2iujhxaug.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sohkcpwd.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jdkfkyso.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2jngizykz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2qvcxepce.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2aniefyte.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2oimlnjgw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rngvgzsr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2evsctrhy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pzxisgbj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nejxqzel.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2rmbzyqcr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2sxtpphfo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2oqdrjarw.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2lafqtgdd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qkjqppoe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2awvrcyrm.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2xcmrgtom.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2atulyhiy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nhbdspaz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhyvrwh.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qmcenlkp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2pchsrapu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2gprsvzby.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2ygvcmbyj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dmsjdnuw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2thmoemmu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2xvbqmnth.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sjjlleew.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nfofvnhq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2pggbjdgb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2zealksos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2barihubv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2jegqbttu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2ngifphtg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2mikethjs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2byiojugl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2onaoluct.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kihweqca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2uldekgzd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ypefttxg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2dqrrxtcd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2stmbsnpi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2piehtimy.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2qiywydtz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fgyucypg.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2epadblux.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2woxpmrak.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rzttysnn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2cdttnvyy.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2vrezrhga.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tydxyzib.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyeparb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rnhjyqjw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2lmbqqhnf.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jzrjfvpj.html


<!-- 参考信息 -->