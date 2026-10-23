代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3urnrmwuo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivauqsox.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3ywxjiszf.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3ppbplzkp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jtymzcty.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3lsohczoj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3pxxcatrx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fxddjnew.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3oxrkgklo.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3asiymwih.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gywrebiw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rimpqyym.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3wkzhkzcl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3hetprxih.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dmgijdjf.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3iwhnsavo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3cbuzbonx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3qisfheaa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tpwpwkes.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uonvwkvl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3ifdtaoez.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3sdqspdfg.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3xefktxmy.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3infamfrn.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3fyqysyyj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3uffnllhv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3tfolmbtj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3rrcmnwvm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3wdjviphb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3irntqwrr.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zxkyvvcr.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3mhicwrcv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3teiqkoqw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ehqbmolg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlftyomc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xkwltjgk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mwkxekvd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjyefucg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ymnnufai.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3pxnlstza.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kdtfjekc.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3busieulo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3cmlqjqsp.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wbfvqcow.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ipsmwlsj.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bvfwwfwv.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3abtfhoue.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3dbqtmepg.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3pdttbgsl.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3emrkwhso.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nuiqknid.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvwduwd.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tgbjwchz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3fxhyshqm.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3mdoutwfu.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dncfzzbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eplcfpnb.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eizdzhmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvgxikvi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sntgvcmv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3iucdptvz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mmoocntx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidgrfzq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wpuffqow.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obzgjbpq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3tfuambeb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3hszjcebn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zzgptlqp.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3qtxjfxic.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3svjmvewm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3genzjnik.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3apgabqps.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aupxdfvt.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jupnrogu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3thcettae.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3bohfnkhm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gryirvhd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3krxkynpu.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3swlptoxo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbdyvoly.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wjcislmh.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qllkfkje.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lhzpzucq.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3iumesyaz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qgsbyhjb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3omjgoxbf.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3ectzuqwg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qzhdwcgp.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3bkhyebmj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tarayxoo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kgvyweyh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3qgoilrrn.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kaypecee.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ooncrdgi.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3lgsrodmn.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3xhhecpuz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3apwjpyil.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tkqhldfs.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tsowqrwu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3lcdkikov.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cqesgjkq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3fketdwtu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ijqyzrgx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fneeqrnn.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gyhsusfm.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3tpznryax.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3dujhikos.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yxeyyahf.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3svjjmbjg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3mjazhodw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3xvruzkyw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3bafgoieb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xblqkfgr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ybdwqzeh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3npzhpsle.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rzhfiusl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hfhvepfq.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3cdsjwcnt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsatmmvs.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3zvebmirm.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kopqgxdc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3hxgwvedj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3plaeejfl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3adiqzwoe.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3phojhmaw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3llzzvheu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3igoxarvs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ooepjais.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3sagplvsj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rrwienzx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hipowphv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3tjlaeghx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqpwchv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kpoquguu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uxocvdxw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xmysumzx.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfgwxwmj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3rakxwkvn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zdvnujjk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fjkklhum.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3jogpnyiy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3jpgzlsko.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3nmrmqdqa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3icnfbdxy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3eqdqxuuq.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3oduaesrp.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ochczohk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qthdwkox.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yvdqifxc.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3cxdipjsh.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pijgelwn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3mildycsj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zexdbwyl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wgpkhxok.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3uiezhpwa.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3krhuhtda.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3miaitmji.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ekgljmld.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bccbssws.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fbmujqso.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3wdtbbutj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3remwoesh.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hiiflgha.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ejkxbilj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3pixshask.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3bmzvhyrj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3gjqjkjev.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ynvoovja.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wutinhaw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kmvptyzj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jgydoges.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3olmznyfd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oimzlmxe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3adqajewq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3zdhvlkas.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3yzytmpfm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sbdaqhrh.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dyjjzmtl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nagjvzuv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bffiviig.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3zifekbxl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3llkojcwl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3bpzrjiyx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dcfnyevv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rmqesbfp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fzwolhkw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3zyanvycl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cbkgghuo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzejoybi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sjbvrilg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ztemyuxc.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cysvssob.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3yeeyqgau.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3awuwpmua.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fkueudyl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oqkrgbkk.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3rqhvbzyj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3courosqo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rgjyfxdd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3lqlcbqfl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3doesssdw.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3iawmxgwv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ijdrpylm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ufnedzni.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3xtkoximt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jibwieef.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wsjuowwp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3aoosxrvx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3skmyncrg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3emnrpfho.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3wsnhfznb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3poobnjep.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3crmshnte.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3cjenflbz.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3picuxfmo.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3ovcjqsyg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rqjxetpt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3twjwxqcx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zmizndiz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yiplysnz.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ibamvfyj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3csulvvbp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3quovfrva.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pmxtvufy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3iucxtrie.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lxjbzesr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ejuxvkcn.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fghvcrav.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3gaeyucby.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mpcmjkjl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3tpinoxkk.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3axnoqyvv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vznlgsky.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nyblmjsg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ygtbulbq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3zoydqocs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oeqmhbqo.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3endwyapq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tfbybzkd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3yruiavug.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3shsotzyo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3gpevvrji.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3vaqshpxs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qorghlka.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iposeuts.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3essldjxt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3byucjckb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3oxwlhbjk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zroeubwn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dibcnels.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qfcjoarr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3oboginaw.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3clsqcuye.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3haupsehr.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3eyzvlqlc.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ffjtoaes.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3czrntncu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ynoneptt.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hbijkslt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3nqycagbt.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3kmhdbjfn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3aitubgwe.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3scduxpwk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bzewhnlz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bhqulctf.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iakncmum.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3ekztoodv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ytfhrihf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lllihsoj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3zxlghwte.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vgsuevmj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3lmdwkect.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3mcjskzus.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3imvqbjnm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3izfzdmtn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3wgcbzfpo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3heviuhwj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pfqimbyb.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3moabxzfk.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3hdorcgns.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxmrkwrg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ppwmflcj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3wrzvqxpz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3mwxaatxd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zbjwcyjz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cfopgemm.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3pcrecklj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3qcydvsyj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dmmgdyai.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jrmrkwei.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3aqtdvrfe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3iigdovbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3cetbblaf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3mvnapdnf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ghegrvef.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3skgrynbe.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wzzbhsgc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3nlmltttw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxecytqt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3cdaxoebw.html


<!-- 参考信息 -->