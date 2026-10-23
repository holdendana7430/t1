代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3avinqwif.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3pjblxeei.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rymokogp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ipmwriro.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lfwrnkao.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xfqbrhme.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uxzfhidi.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3wmvmkalb.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3obdppejt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zreqsmta.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wdgmvjig.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3zewvhhtp.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3tvrvkfbh.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mjlkjmvj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ccsamfmg.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cijdukhf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3gqeamikg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ccoxmarc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3izjwrvpy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bgvvmsir.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rdxoqtsd.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3pgwdacge.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3itgkendh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nlywfplj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3eswbqvtk.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ziiztsgf.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qmcvqvfe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mulsxgza.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xxdnfyaf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3agketvfk.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rjvqlzxf.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zcqmfqji.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3whlsneci.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3sobudiac.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3abatdsec.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3amtvsrtq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3zwutcxkc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cytbqkkg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oamauhur.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3hvwbzjqe.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3czfzxxdd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nngtjwim.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3uztoptin.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3oeaycqtw.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3dvgqdjix.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oefmowqq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mfgmbzbu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3buwqyinb.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ugylspay.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bpmifcef.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rqjeonzg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3nnmmvjgl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wqlgifvx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3foijzesk.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ewumybgk.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yvtfjsft.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3iciuewme.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3irujguno.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cognwbha.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3djhrwobi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nrsvxqvg.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jdfpxhrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ertvygdz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zeheifdc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3phymnpby.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3akdxripw.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jnmadfuv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpmejwnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zwqcajug.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ivptvqtq.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3mchqkuzx.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztzekzzc.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3ihklxwgx.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ovxpcymt.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3nfhdffpu.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ygfxflbl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3znircmbx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gskgucre.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3bbblgynw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3udzfvpuw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3yunubzsv.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jqbriutm.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3kdjwnwfs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3wnkonzpp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcetoffy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3mfgbwyeo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3dftfdjcp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3qbopfjmc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggbnornj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3fwzlquji.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3aciwtpex.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3mposrleb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3ckamzmoy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3ywvrshds.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3nzumwwjm.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bdvcvaif.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3hygarxfh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gpydowrj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3acnyxqoq.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uyukbwcs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mdxbvblt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ylkgrteg.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zivurybs.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ijnnsufv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3ueduxdtv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ytilivuu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lhringmx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3grvyzgtb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ofmtkqqr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3iokefgnq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3giflzqef.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zudbjddc.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rlzpkvug.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nccqjgbk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dhhzzhks.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3euelyodn.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xjydfikt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3eaqtlqpf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3bztedxba.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wqjihgct.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnygipt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3fsbavtme.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3yxlflzlb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3fdycklwg.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3obqsiqbz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hnqcyrnw.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yhxiyfff.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3rrccerfk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiqvniwj.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwqflugj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dkyzltyv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wbwfirsf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3lrtxepgs.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cfaheqfp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mkfqslas.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ofadbdey.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wsiroaiu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxwouqs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tuzxcwtt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qqdpjhaz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3lczqqoja.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sgudufpl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xsnmlfhv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3qhzctevf.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dsefyvfn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3xcidvhil.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3vqlmhbug.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3aakryaip.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lnzqnnhr.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gxujotaz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dbeswqib.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aunqgsmi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hirkgytv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oneoaygc.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vtgnjtvn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3valfuuda.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3uxqtpsnj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3qhctycou.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ynochkdi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gtohciki.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ywrdjsju.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ojvtorle.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3deorzfwo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3dkvxdool.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3lwuuyyyn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hmiqwxid.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qlflccxt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aobhszml.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3qghafatr.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3hjymhojs.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbbogpef.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3nbvosrjj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wuvtxhqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3hqcpnmaa.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3celndzjc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibyqgbgf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ksclbixd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3nrdaxvwm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3kunybxdp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ccsfnwuc.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sawxjggt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3tpxwjnkc.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3xsvctnjg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dlpkvsnp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3stzmmcwo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3dhxzsfhb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ypbksnya.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wnxnrrqp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3sooweabj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3owmzfbzb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3quyqllxr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3shsqeyis.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xptrxuch.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3hndgidxp.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mxnhhgcu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bxrevunv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3gcammhxy.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3tqkemwvf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3aqkycuhr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3oqqxhwbf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3llnqlomn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3mjsdxgxj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mtnfzmtx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3euhbiplj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3shtecwex.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pnruhvzh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjewzjpa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jxohhdoj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sobtnosy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvkjresl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lksmlzkl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eqzvtnxq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jfkudndg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zrvmwmqv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3spujtmws.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3covhvclb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3wcbwfxrj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hzbzktmi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3qzvebxxe.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3xfgclato.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bpwlrlaq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3osfsmfxl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3blrfoigj.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lpdlbvkx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3semkrvpj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tmguford.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3urxsxeaf.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mqbmkcen.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3huxpluff.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3sfvfzjqs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3sxdxbwlt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3kitszlwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vyinztan.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lgkwqgvp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3yokeozov.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3nhnufmrc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dwdnvfhw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3qpgpomhw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wehklfte.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3dsgxuyse.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3dpmkqmaa.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3zjdwjfld.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3luaytrzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3fmcxoldb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mjjqrozb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3qyvlqgvh.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3wtjvadwb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fsghmiru.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fgbmwzlp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mjgteulw.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3hsmqwxgz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3zjuruwbz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dvqhzdbs.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3vcfugane.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3epcrndol.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3yaaozzeh.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zyqxmrlv.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tfdyinym.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3obxvivgt.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xyluuaxh.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3bjkwvuew.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3degbtpns.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yabrbhfb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gzcmhugn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3umlrxpyu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3rueeslvt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xltrdxgy.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sewewxll.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eluuqxgl.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3advzqoif.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3rkwuqkxg.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lkynbvwc.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tqtygjhj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3fkvegfca.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3letppszb.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tmazfbrm.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ediulvkk.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3esconzvk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3wfvrmsgg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3oaeycqpi.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3ipolihpd.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ymuohvhs.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3gevkbxkb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aphqkjov.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yyaiulfc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cjamitmf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3occqtsol.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3jmiowaec.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ftwddbuf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ksyoapjo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mumtdvat.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3sizajoud.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3opzmtloe.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3zkibmvak.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3sljgxmfw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkucepw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3uwboqelg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3eclencwi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3lwhkqxlf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dxvgprxm.html


<!-- 参考信息 -->