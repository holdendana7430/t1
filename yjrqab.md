代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3qzggdjwy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wtmamgik.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3dcracjdm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3optjvvnp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3ugrqdczc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmicslru.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3pkicqqgr.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3siquefii.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ydjnfunc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ufkorujo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3frndacmt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ybpyldjl.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3owbdzvnw.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3kdazhwde.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ytocibuh.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3veiyqyab.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3cdqhijxn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3bxsdazfi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shghuknn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cipoyvfn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwfpwagm.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3quxqfdsi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3nfojagcw.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3olqeoyby.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3jhrvicgk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3smtqurey.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mfnjiobe.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ryzulcqc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3vbhltjij.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3afkivxix.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3cbrvmeqk.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3dejadvzk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ifnxrqjg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3illkpitb.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3jvpplxgx.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3jrmtuklj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3obxwaqdl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jnzwihrg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qgfyahme.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3xqwezteh.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mceupdat.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ffbdmkpv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3byvwxodk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3yknjwwmv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3xbbqlxxy.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uurrgvvb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ywthwyww.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aybqpecs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rbdsrech.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xdolopcc.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ecerdrtg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3xzywtigp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3flbotbvs.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3vuirzarm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3koophbdz.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jjgelxyk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3hnzcvcoc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3skdyviro.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3kgaqrfed.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3brlrsgsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kthafzis.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rbkmwogx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lizjyaai.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3jtxmfynw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3turwaxtd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wxlptqqg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3utdjnkwo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3grnxvrqi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqjevnpi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3pzaltyps.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3yymsublj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzigcvec.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mcqdsdhy.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3wqbwisvk.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mwnuidep.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3abptpgth.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ckprpztx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ptcvoere.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3rhbbspiq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3lpznvhoz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3tnigagou.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3idjojnvc.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3zxfojapp.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ezxjjbrw.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3brqbnwlc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mayytdjw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrixjnlg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3pgwuoiko.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rmlhyiwz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3otysajvc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3odtzavjr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3hfwsqzpo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3jwystzab.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dddwywvj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3uvurwyvv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3nlwtnrdr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3uzqsqxil.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mscszjdw.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ptllvjkk.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3gllidixb.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3rwqqtral.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3eltrtwwa.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3thfvswts.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qckjcrzl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3uegdbkmj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wteitxfq.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bxuxfhlg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oaelzmig.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tkljttox.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3jaiurqdj.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ekbwkrdt.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3elzjdwzi.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nnmpdeyl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cfzbicne.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vnksmvcv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3pqxdfmzb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vxnjwoeo.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3ommnwxsa.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dqcatmev.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3kvqbpsdg.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3jzwewifm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3chqahjlc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3awpovgzp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3lwktbena.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3tdhvowhn.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3trczhqub.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3hqzmwrqu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3hloalmkd.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzuwkffh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hthskqml.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3agyucccv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3dmljvqvu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xgjvlbud.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3duaeqjec.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3vummzsnp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3duadramx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3turrccwb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkciskxr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ijgjvjey.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3uyqvqkjp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zpoebkvf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3iffgdmgu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ucjdywlv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ckbytqvv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hipmgrzc.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3begsvycp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tbwyjoyw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3dmiajjbt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kgkchhqz.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3otjidzis.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3voobnkec.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xatycyvu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gfclvijw.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zxszwxof.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wvpfjmff.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nclqnspc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3ztixpykx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cgrixlul.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3kktjclyk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3iycsdgyb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3yxrwgcnr.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3jgbnhhbc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hblbltkt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3zwxqzmyl.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3iwgwydpy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3euxlulmx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3flzmfijq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pbawrmrm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3fnxmzsgu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3fepywpsl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3oerwafax.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3xxxigzpp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bejlmpcs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3poeaijih.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uqgcflvs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3drrcoalg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ufkexqdy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3umkzlehc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ibabcspv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qjuwxjup.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ctyztgnj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3efrajzuy.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qekupglp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3diqlvuwy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ltgyorql.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vsjivlhl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fjmegioe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ejfglemq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nuvhocmq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lnophrjg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qfncvsjs.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3elvszhab.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oagiarhg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psoepskb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3mcytjkfu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nnjqfnoo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3glrtuzzc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3odisgsfe.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xfniytys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3icqibblq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3vqljguyy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vsnffonm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3dffabnab.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3yzbkkszb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ocicuncj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3azfkhefd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3spvdmaem.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ipfmphqo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lmqqeqgd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3onsrpvjf.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3uhcixtel.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3topckhik.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vihhvyqp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ccufzose.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ajxutfzx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ytlakryf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3lnkqgskq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3dzpttpza.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3zehynidx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3aejdjpqq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lbynkwto.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3bkvinwgp.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3wnbkmdqn.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hcdsaoom.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cgoucpcb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cfpdlwli.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rubmfrso.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3ylyxjcrx.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3roorlvth.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3bsreczon.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3cszhdxrt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lvxlumcr.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3lajmcqpp.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qremucln.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3vcpnodin.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3oqqzdglo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vlaqilvm.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mkcgzwle.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ixzcytwu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3suwdeqqb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3qgypvpfu.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3amzpvsxt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3yaylwykj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3opatwvuf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bbowacpw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhndmon.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3sxezndjx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3fwuafqgl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xlplgzvt.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3djcadqet.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3yfjxwmek.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3apayjzvi.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hyghxclo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3astpfthq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pntkirry.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lrexeotc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3orijzubp.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nbmhueqy.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dllldfws.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3rnxzxpyt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qhymkwlw.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3shpgizwe.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3vhmiahmn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3fyfpmyjq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3leyzwwyp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ekucntcm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqlgrmw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zeqqivru.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3arywpgig.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3chfavteh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vdetpplx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3yidkeiyu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mckiccvx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3rsbbtedn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jlqbopug.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3saqdfbos.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cwxxwqfw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xiyyfyxs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sahfwish.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ymmsqpst.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3lvigvzct.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gsdsuwwb.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dvzugorl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gvyxofgo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bmuhwlra.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3zeaigqoc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3beskydga.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3sswrnatx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjwyjjbi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mmoovmhu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3sxplfuat.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nkiwxxjv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rtsljbxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3dbdoaawz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3skigpckk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3oectbtxu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3epfqbldt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3ieberjpt.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3sggohwig.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3pxnqtafz.html


<!-- 参考信息 -->