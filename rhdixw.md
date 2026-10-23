代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ffmmoipc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3hamgdyel.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3beuamipd.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lsckkegm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3xeyognqa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3nuqosuds.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3krreskfq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3byglhlhn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3lciwtgno.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ynhmkqpo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rrndnscy.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3eckaksbg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3hdfzzwev.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3ulyoxrgs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xhcreofy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jvkbqzzn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xgmpllsz.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pbxkxgpw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3miyxszol.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3iqpupkmr.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3mmwnvymw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3npqiwzas.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lxcboxqu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3luxmptkg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3teyymyom.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3xkouqyfx.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mffrpsom.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3zwtmwxok.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3wxntdyyh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3naizugto.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hjttpbpp.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ugyyeusf.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ucequrvj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vjvhnxme.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fanyarev.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbowahnf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vjskwidp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dztkmbeb.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3fxmwageo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3lwugyheu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3txjomwja.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ykxpljnx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3meajpizn.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wypkjgyx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xlxdnbkf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3smzbhnfv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qeqhdnao.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ujeopxps.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3jflhyonv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3zkvlcxfp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vywagyjy.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3whhsspqe.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xxoybuto.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zpvmbxoc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ssxnlcai.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gqapfzsz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhkvdpnp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3avnswwjs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olioqymq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wmjoetzh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ylddbesx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtgshlck.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3exjioxva.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3sknpalqd.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fxnvfjpm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3mpjqxhbb.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdwgfbbi.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rxrypvsh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3csxhqufc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3jcrxmxwe.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ltkkbgjk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tluzozja.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgndfdeu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3bpdvdwer.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wyolrzrl.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ovtagfcv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3hyrdjbzq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3eucciggg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3akoksvhp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3niagqbyx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmqcwooj.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpqfguy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3qwrpkcvi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bkinfger.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuxveutn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3gbhfbabu.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bmuljqcn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzzigpm.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3whmijvrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmeregsu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3refklnhl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jtnnyixk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3nhlvoeyx.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqskgfq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ohfgqeei.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3ivwflgjq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3niwqzckp.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3cuwifqmp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3inzeprez.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3uhtgvggs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3suoezkls.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ywriycno.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3moquuzrs.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3qviaowhi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wvorngwq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3oqrnkpww.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3swqmwbwe.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3thelsdyn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3aupdvqhf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oaowywvz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ihqflwdl.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dhdrdbuk.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3hzkxglvu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3vhpeiwbt.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ofmouutf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mgzcyugp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jeoefqho.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3gsxobdwe.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qrwqrthe.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3poqimhxc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3hkwzvjjl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3dfuhhvir.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3gpppqfbi.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3gjqrhmfa.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3jvheltbl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qzixaiwx.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yzoalnba.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zdmxtfsp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3scdkzlwp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ihfihwug.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rjriyixt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3vriaxkpm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kqaierha.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zofgralt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3pnfagtup.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3fcvsgjfq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpptjgns.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rfahkyhc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qwygudse.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3qdncptjj.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3kajqmmzp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3mhquhxdp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3frofbmnn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pcvpdxuc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3onhpgnoe.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ozxivurg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3crpjnpuc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3mfcvngdy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bdxauhsh.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tolwsxnn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3pobquzdg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3juacqmmv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3nxdtaypr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yqparkdu.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hosjwtly.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dgbbplnv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bvgiuhun.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3rrddxett.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3sioifgou.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3pwmjihpf.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3kiifgbfx.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fnvhkxli.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fapmotta.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3yfbecres.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ldjkqjdb.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3imcoomym.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3knqtswtg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kwssmzkh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kgggtanb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvkdusum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kzgunlnp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tqrfuelf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyezdroo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rrbiqwdt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3oalnkfhm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3hsilhsfi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfhbqlic.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oywxzrlz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jymqawqn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xhvmmbgq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fqjoguxc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tmgdxlsq.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3meqwkras.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vcmjfovc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3eqpeshej.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hopkztjc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kebphwib.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ktihsbwr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3czhdyxad.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ktkqirqv.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ddsoxerl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zvdtvfrp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3clsxffyp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ilxaicjz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3itmwxoxe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3bmvtfqin.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cfelntvy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nswnizpu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3xiljdxvg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gorjatih.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ofprmiis.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3zaxurcyh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnzclggv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhrgcvso.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lyddrqvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rcccohke.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3rgqceqka.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3fctwgqnj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mzdzgfal.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ywvgazsx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vvvkezsl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3gmdpctcw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3xvgwyjyq.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3zafelgdk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3kkwjfujs.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3bbqfklbi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3mbyeqqxf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3dddohowt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3etbvponh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ronjaegs.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lkqwwmjq.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3owevieyi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3izbsojtn.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ybdbhyws.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zoyfurfs.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xcaqveik.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ipankftl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3gjgcdbpj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pkscmjqy.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3liwlxkxi.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3dwaeruer.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3etquoxsd.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3grgeixjr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vrsfwfgx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3gfwoukwi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hiedsshm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cavxgkwd.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3tlluplzs.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fxfokbqi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zcqzlajf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gyrbfjzy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3poowsbhl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3eytznubi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xqorhdql.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wvcnfqsx.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fcohccbi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aaivfryk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jlcnrias.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3slrzaksj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cxxvulio.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ikiznbmv.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3eomcryzf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ndbvslyg.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gqfwurjq.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zsoqvdnm.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cbxqwvmd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3ctxzvmmg.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtzeugp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3xwbntdsi.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3qkheozde.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ptqscpac.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xzcejqmr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3eveigaxt.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3omxxlokt.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oirfpdnb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ehgwtjag.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3axystmfl.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dbvasdtj.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3jpmnzhwj.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cwsgxxou.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ngsqwqrq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3sjgxpiux.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3axpawnyp.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3cuifyzgm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3kafbfznc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kolrrzvp.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dztjmanq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lwurhqyq.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3zwlgkkyf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3yfinlmur.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hijnprxe.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3orbxsgrq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3cqtxqfzv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3miwmbqlq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3wfxclzbq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mgxwfmpy.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3lvmatdof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3awwyiofv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3lqdixlyr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3rukgbfml.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3zrpozugm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3britjump.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3czxubkds.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3odeoeokf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3hynmvawb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3cijisbuk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hweoykfp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3wxliszlv.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vdjpwbff.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3cidhswrb.html


<!-- 参考信息 -->