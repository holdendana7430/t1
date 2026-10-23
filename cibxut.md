代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3yurjtddm.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jdrixopj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unygrosd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3lrlxgrzk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3tulmbpti.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3cxzoqtdk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wzbppynt.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3spjpeiwp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xuxtavut.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3uvdhhyal.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3aqydbfjv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3nytzkqsu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vlxbwhvi.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3fdlkmurk.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wqyknjvp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3derpumyg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bpprlgcp.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3trwmutes.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yyllpala.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3asvyhyse.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ovcayogd.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ercaegnj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3qmettibn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3eltjmpmp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3inamslov.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3trredcxq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jfqglpgk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xgkfvnrg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snoztcfr.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oflinyin.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3gaxdvdkf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3xqxvcknj.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3igjdhsix.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kugeublb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aycroura.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kznhujfi.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lepygpbh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tgylhort.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ecelxavd.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3tgzjfidd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3bexgccdd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3shqqgesl.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3yzjehknq.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3bvlnjlsi.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zkypqlil.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zhyooyhx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3xgimtwmi.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3nuxhwhkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smkpeorb.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3iwthwvpf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwewkcod.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zubjmkjv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3jzrsnegp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bfvragmu.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpjucaif.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wryvkyrr.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3waecnoih.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3mukxvkiq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ojtgmfca.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nberiotp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hwdkroyl.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3fydumium.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxjsoaqi.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fqjqnyyz.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgynthkv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3clxmjxss.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyfhdubn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3mstyvhpf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3btdrhswh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rczclbvn.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3ymwagcbv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3tvlejrrb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3rpbucjzl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqpazbmz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xrelljxc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3gsslicvx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3akjxneyc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3hdiiacxe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bnuvyofn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmkgtpwg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3jvyqbkes.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wrtwkfxr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3wvxypgsf.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3rucfubyj.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3spgbxdux.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3inrxdgze.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3aiseetft.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3uzrbfrfp.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3lbsepvdr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3lydlzish.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lispmfhb.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3gnxlialb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3xpljuvaz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xbwgnduk.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lcmunqel.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3gnsbitsw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3fiarvlhw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3nwyjswbp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fzvhxiwc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3egozcbvf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cewurjtf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rswzdizj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3bfwgbsgf.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3mgihivsr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3mqpokhnt.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mokdbbyc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mqpzqioq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3eocpcyuj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3hmmynubr.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3uomwwcxb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3bvrdeiqw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3nilrmvwk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3icyayqcg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xilqapqz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qutkrwan.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3lxjhphwk.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrxwyaly.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3onrgaxfe.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzbvzucz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yximtybw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qoanpiqc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3cpnzmedr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbwtwokt.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3caocoqoc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uunfrxlm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wbbrasxw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3upesslfj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3beefnshe.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3twlxydrp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ojbiieck.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rdmhmkmy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vgmmdkcc.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lnvflkft.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kvvzhcvx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3bctvvzln.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vwppriza.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xguwgxxu.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wljuzmae.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3utxnunvp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mfpttrtl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3umbpjlzz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3jolrbrdv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3yvqitgya.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3zifkyxrb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3qdernpjb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rwyczizc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uattpgbl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3oovsacax.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3zfhffyru.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tutztnwg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ihtlqxhw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3bjzxvnhi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3vgovpwlf.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3axayyflo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3otesahln.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3mzpvxfxc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3hlgvfbtn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vdfqsjcv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vmwqhxgi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3estgqjyo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jyrnexwv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tptikdim.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wamszcwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovlrcedx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smrcbpjg.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wghmvvix.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3loxbyevy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vcrucbpj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rkdhcvps.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vxvtjizr.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3yfusyaac.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hlhwlswo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3lopxzxqi.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrdegyhb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uvwsndvx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3drblvivs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wydydwus.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3cswrrexc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cxgznedg.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3brlenoxb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldzjices.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhykosem.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gzxktwmr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rjyoqrsx.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3uuqkkxwd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ufdsuoij.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wfpuxkfg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jpnpamny.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cjqxnolf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3edplinva.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3fewkmiag.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojgzocfz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3momkizas.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3xygfnlvi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpuraius.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pgvlfnnn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zixuwpwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3byxmrvse.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cpvxbnfh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gbixytro.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uwihkwzb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3axmzopzn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3yqysqzgx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3uetsnyog.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3fzhlaycw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ylanwoav.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3tmlpfmwh.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3excllhzm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3ettdbszc.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3jmdeiycj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3iljzemhz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ohhgccbc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3hawhklpo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hdkddaba.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3egwqqdhw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3llnalwas.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3dmkkzrnx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sxqrjjos.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3trisiuyz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3negrvfsc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3atoscypi.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aolskvnh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3utqjcdbh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3hipfzdti.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xxpzgjrm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jbaewvln.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3lvwnqixb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xuyizzwp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jzryvvuw.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3mwpntbpi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jxsnijfd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3exnxcxon.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3renqjgxl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3xjlumons.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ktpgamev.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ouljsraz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ypnyidyl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dvlwedqo.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3gcgmwuty.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3avqdvekn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ugbbynpo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3jpieeokm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3csvtddyn.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3simfzlka.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyshepn.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3wssqeyjl.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vrmrmmpw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3xpavmtpv.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3tlbszgcu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnizlklj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3zdqyhgrb.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xrdazpfi.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3htjcgalt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3azvuwwni.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zqncgwtl.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tevrqsyg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ydkkefiq.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zgvgmbkl.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3smkkkkia.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3cyjlcflo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aqtpukmw.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3luvzrece.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3padjvoov.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3tnwpxxhg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3oeocwdki.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3fmkxdbtp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3xynlpziz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vrgqrcdp.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3frcqtdsm.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jhfzxrbq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ihnympst.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3zotpazdb.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3evyljfkb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3qkgsylni.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3demdfaut.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3veuxxnxx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jhovkhrz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3goejcuoy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3tdflwqxb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xrawutyt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pcizytqp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eyojksoh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3iytvcbkv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3uilfqbeo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3igeabmcp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3nyrrytbt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3hulcvbgu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ecuydpdk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ohnfcewr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tyomsqlh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jsayvlur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3bzfwaqlr.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ggomicnf.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3kreyhvxt.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kilgeojw.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3yxhizuau.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ifafnjei.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vrqpruqp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3xfqvlapg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qybhslbz.html


<!-- 参考信息 -->