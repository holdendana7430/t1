代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2drcbecpy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2meghhzmc.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zhgoucxg.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2lwujxush.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ivryymvj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2izfhsvtn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2somfzljl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2eorgjtbj.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2xzsxffbe.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tsuaogfn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tnvxefab.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2cafgnxsh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2azsxzhuz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2tbnyemct.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ditgoqqu.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gloeutzy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gxgbtbkt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2eymmtome.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2lohbmdhp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2rchaxpaz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2dlteiywu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2uciypjhm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhdnvdh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gyqxoxed.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lcasycaj.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2kfawtgzx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2hxpsousq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2pzmmmoun.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2yxurteka.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ifnqcqxr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2rxmrvwlx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqmkurb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ezffpiyo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2dvpwbmis.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gzkdutrh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bogywlhg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jbqwtplb.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hmljgsll.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2xasubsyp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2hjybwpmt.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wmqgrjnp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iedugymh.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kvfooqzu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2etwbiwnu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2djvzcwvo.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vsbtyldt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wooyjunl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2jizwdafb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gdnrqtcl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fqmriuij.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zwftxgss.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2qoryvxms.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2avvnwdyu.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2lbhaoofx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2twmgtgmw.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zrkzrzzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfbcboat.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yuaaaawi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vckqcpdd.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xgiptgah.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fdjdmjeg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qydyjrei.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kigkgbra.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2virafvjx.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2frsjseav.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jnuerjla.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dhkjmktm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkblqrmi.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jpncqfur.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2sqxjtofw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agmfvyle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpijqava.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rewmhpha.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tuteekfe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ugcxosaa.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2fcmlptjw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yuwifdyy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkrisveh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2fkykygxe.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjopshpe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2skcxkvye.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2bulopzly.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2katgnrzy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2kgkpzvej.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2cpnzyhsw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2bjvalbkc.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2ontbmzpn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2esjexnqz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lilygxaa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arsibepe.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wvypxcnv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2evfqmoyx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jsybtgbg.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gjbdhbsw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uiumbbve.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2nlysvlut.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2eibuogkx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2nobejlzb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2kvuiieun.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2legzcsjj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2berbidyq.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nmkmddgp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2bsboncmb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2sjsezhsr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2jlknkuhe.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ynprrfye.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rkgecjlg.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kuqpcyji.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2dabowetd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hhygslim.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2cwoowisb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lcgpdzwy.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbipkaj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wmjtebuu.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2rezunthe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gckuklbv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2neryclng.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2nsszcmcc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2pxwdamwc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2pvrepifh.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2opbukevq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2wlkjxpjv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ykwsqriw.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2lisrtykl.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2wnszoazq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2cfvukzoe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2renukugo.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2lunnqbzr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ekhjwjon.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2xqzptggd.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccnjcswk.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kgbjjnpy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qgwqlayy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2ljkwnaxu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2vcgeiwez.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dnibtlws.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rafrlqaw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2grpmldqu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2dwwmvvpv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgnlfkc.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2odgnulau.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2liosfuim.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2jvcsnult.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2lrjyeypg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2isrzeezm.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eqoirfwx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ztjgbdux.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zbnidmre.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wfelflxw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2dvhkltvl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vpbyotlz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2jbxzmgzb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ovwpzmvn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2fppvkded.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ktrwidnu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2qhclwocx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kafkcanf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ylkexeab.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2nxqduufq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2vqpubdyf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2abfbfaqy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2jwphwayo.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2snnbpalr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2olocqzfz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qfumzoeb.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2gsllpgfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jvadciuy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2crymoljg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2wrfeolzv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnexnmwu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2asjpmkam.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hetiisqk.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mephljeq.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2byepdmej.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lqyqclgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2tiaawexi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2kuyiqksh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2lixpsatv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2adjsudim.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hcjnfujm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpqfhnea.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2jnqrgqkg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2gawxtqvo.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2meajeqoe.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2qwjlvewe.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2duxwmnmy.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2uzehjxub.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2htjxhhrh.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ojhyjexq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhqmogxj.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2eyuqzazg.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kpkeoqpc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2lkmnnglv.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2vhhjacuj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2cfpukwoq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2zetoytei.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2xqhxuxjj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2kuqdbmce.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2crqbdytk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvyqjqtn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2qyniulyq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2mdduayno.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2yzoitrux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhqfwhpr.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2zmjdhjtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbzdkdql.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dhluxlhx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2gwjczlzl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2isgcdkej.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2iluwlfqc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2fxwqiyvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2zfhtcsmj.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2uzlkxlcg.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2xvosxhsi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2lxkdhruu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2krwjxrec.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vhwxcdet.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2srbvxrnd.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hwyspxob.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwvjcrnj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2pdrliibs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2hfjnakfg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2ifkxclcg.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2kyqftyna.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2awywhbjg.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qsmohvkj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2wvymulcc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2icowxywp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2tlvhuowz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rrapifgk.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xrruvabs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2hxmwdqeu.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zfgrqbpv.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2hrijzrit.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2yzsczdnl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2fnfexlkj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2wahpmjqk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ctymhuxy.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2zimithkw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfxlijl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rwsqhaug.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2pgvqsgmb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nxgusbra.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2misdyrgo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2gbwtvxuy.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2dzghoomg.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfbleqft.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2gqoykufj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2woqfhskn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2awuwjqel.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bqtxqvpv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2djieayci.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2adyqljis.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pvacfgox.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yqgrtgnw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ezklezeo.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2sfuuuggs.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sqgxaxqb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2kskbhsok.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2sjspqnjq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2izwfrsis.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2phcnzska.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2dmpxmtwy.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2submywam.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2iltpzmik.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2thvharkz.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2yfntjhvy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2mlieckzq.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2bnbpqqcz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2akscjdhg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2smanytzd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2csxajimm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2ahdtqofb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2pmevcnvs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ridymfej.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2bwtpbpqk.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pjmriacn.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2eagskfhl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2djgbhxun.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nzzvzxja.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ypmqmrdy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2uysnugbu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wotdxmll.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2cypomkya.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xuwqsbpw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yrbtgnps.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2hfbbebdf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2vemyfcch.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2falzcmrn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2rfhpdzjg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2waeipwyz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2qfofyoqt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2fxwbwayf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2hgprbrwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xoyhyycu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2drvwvsfd.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bebxjhnl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pndtzlco.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fuzdcehv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2hlytrtgj.html


<!-- 参考信息 -->