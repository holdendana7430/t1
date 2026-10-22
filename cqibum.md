代发 wailian999

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2xlwqiffg.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmndvvt.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2iobizjyt.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2aejunjzt.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ggeoriyp.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bommwipv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zltbqics.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2pmhjyipi.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yzryftvl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2odinazkl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2yualmzzj.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2luzeooyg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2bugghecl.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2stcxukoo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pblnmjgm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qccwppgj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2viyvwsta.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2grljamfk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cfyxjxxv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2jgrljdoz.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2tpxbxtlo.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ichvqugq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2jrzdqvcc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2ubyfivzq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2syztdjtd.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2skjbosgy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pmohjsqv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2jkedozlk.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2bmlkeocf.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qcbparhz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2xumelsmj.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2hnmyudqn.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gqjevmlc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2szmmizun.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqgtdvy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtnxdexb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2nvohozpm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vtnsozfe.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2mzqlxwei.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2juaglliw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2rrzwiwxq.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wtajgurm.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uvvjlatd.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhxdvldv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ufzukqyz.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2othbpqic.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2drkbocmr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2kjuxzpwm.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2svbufyou.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2pwkxqvcr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2fcxdntlt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2vljoqmqk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2tlexrkgf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2noyqahqc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2amlmrtrb.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2sbmsavcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrspiilz.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2oantcybo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2taohrckk.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gwilorys.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rwqwwcqt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpkeyla.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vyupnobj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ozdinqqt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vvxdazif.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qnmjgxrl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2yhpvzunc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmytdqnw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2cgyiaerz.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2dkknvngm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rqvhobzn.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xgwejjsg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jviznacz.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2nrjzkwmw.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2aykvdame.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kdxabwiq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2onpvxrzx.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2utxtneav.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2grtoivrv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kckicyho.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2njionfyf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zgwxbeir.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2njcujwdp.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2nskqzgie.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2jnkjyufi.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2irdzdjev.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2umsagbfq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2myexkbyx.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2gykbgwfu.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mdswkeue.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2aqbmtpyt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rnvudliq.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2zupntbpd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qmarbaxk.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jywqnttg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2jmplsjfi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2nrdhjddw.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2almkbtlt.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2obmyvaos.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wciysjwk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2whvncnun.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bomvyenm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dxgtmvmg.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2furithst.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2rgvdparp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2sjxmgqke.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2zlwjlkuw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2rrmqzfds.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cunaqpew.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2iuauehiv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2zixbocwb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2oavzibhm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fyeckvey.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2whtvpijm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2wzysesms.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dsttuqwl.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tyiwzckn.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gkbpogrf.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ymspnwcg.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2ahbicqcv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2yefummrp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jidiweiu.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2qaycfkun.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2ghpordhf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccbthexn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ruxgnitb.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2benqeczy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2bvfasuoh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2yndlyscj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vxrqmxdq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gwprhtyb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2qoahibpo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2olowzbqg.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2aosrjifu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2evlpbzhy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jjfnlvki.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mltzppwz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xxwldpdx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ddlsiirw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2hljuctto.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2sovlusyk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2tbbrfrlj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2gcrsuylb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2fntpenhj.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mxoijlds.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iyieiasi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qqzldgdt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2rjmppdzy.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nshetqpd.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2snztlweo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ohwpegjy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2quhfljrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2zgemcfhd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2gtrneskr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jjwyqtwo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2lstlsidx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2upanptia.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2bozfbrik.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2mvkvhtuw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2emubhdyb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2pqzavicz.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2uagsppsj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2utxczfcr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2suuefoht.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2dpvjnnts.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2advgkiyd.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2fhceylye.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xknnzwoa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2esfhnlob.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogzsrhon.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2unfariaq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2orfwflby.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2guwcwxob.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hvijledb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2bhbdlbak.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qsdtzwru.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pwyqmhtl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2jvvpbkfx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2sxgcgziz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nobaxgzl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vlxzursp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ngebltwk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2aysljdlg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ecqaizmv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2cuigrjhc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wcvijfzv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2bmwudrqf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2bsczxrut.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2cboshykc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgouikao.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jvrahtmy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vytykwhf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2bxgaxinl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2jbzruqjf.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2viulrige.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2vcmlcrqp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2oumpytiy.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yabxgndi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2uhszjbxc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2cuovgbjl.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2oahfjabc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ufdijrbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2hdcurgcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lchngxsj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2tasozuix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wsjqewjr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2euglzidf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2cnizflzs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2wnfxjhzd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2bkygxmck.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2cgdwgquf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2skgtfreg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2dpaqpnaz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zfcbfbjv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dfvhkkpd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2uaznovic.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2glpqevvd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2wjzwlwuh.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2focsdile.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2audzehwh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2plyyrtpx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2czjvduct.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfbormz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2sdnitsws.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2dbmdmafn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2pslqfygh.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2dacqothp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zwcmputm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hlexkibu.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xdgugbvz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2mhsinimu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2aeixczkq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2arpmsnjl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2iamvjtfo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jrcpjmbi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lyvvyayt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2elflzoom.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2kcdjpcac.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvysgwvj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2oieuopsf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2eflibcod.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2boywzqfx.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2lwjwvokb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iztqznxv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2gprnjgse.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2yzigixcd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2tnhpxejl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2drvnvrwt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ygbysmqx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2xyfemanf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2heriacwd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2airznfki.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2cumdqpjc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2qxrbpqmh.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2yfdgbwzs.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2qskeavkc.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2nsnpskel.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwejufa.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2piybizmx.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2xsjadbql.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2pmeyprxa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2kpgbchsw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xfiuuwoi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2sescuwsw.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxkwksbv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2idlwjwcc.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2zomnvtvv.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2cxmcvpae.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2smslizui.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2sroedkuh.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ulmrrnsj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gjexthkb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wmgmeibb.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jmnqcghe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2nemdqlfn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2yprbecys.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dozpnpbe.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2csfwltpf.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2opmygumr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xivduhfs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pnalfoff.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2txkpqfwb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2lyxuqswq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2roygopir.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2azptvupw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ewpbeqxw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bitjfkbd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ipztgyyy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2aqsoesej.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2nbzxwcso.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2juyzukny.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dogoqdzm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2nbupkngq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nzgzvqwe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kyoiskkf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2ifvpsvtp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2abserjfa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2oohisddu.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nefyzust.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vruiyzne.html


<!-- 参考信息 -->