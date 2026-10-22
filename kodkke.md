代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2moqzsblc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ffhdpvyw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2iwalxfcp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2zbpjifku.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hizmsrla.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2yazrxdjv.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vvuaacaj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2tcfzfcoo.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lfrqdzqy.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dnuphzwk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2puywtjlw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2ummbjpwt.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2cgxhxpav.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2twjblsnj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sqknkdba.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2purlutfb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2ylkefwav.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lfotpvpg.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2juldlnsp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2crdfipxq.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2grcjwbsw.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2hqvjwqeb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhfretsi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ofpcqmfu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2wonxnrnf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2fyrwwufv.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2yajfjaoa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjaqxeea.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2eqeymisj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2mxmlektf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2nzasfglw.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2yxxzghfo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2rvmisees.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2otffetnm.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2fbjzkytd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2mcbpjdbd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2acwtsmnc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emxzsskp.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mxlghuzx.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ruxxtyxu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2hmpmdtjp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tulfbaka.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nyhfkbgm.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2gnnklwxy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2npnuvzpv.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oawfrqts.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xfqaquoi.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2muahzfxk.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mlwvcjai.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xwxtsbpm.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ocxejvhh.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2iovxaqwy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2acqcobkr.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2gkadhhri.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jbwgtimu.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lombfewy.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wfxzkkph.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2wxbzghzy.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2vieanptg.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bzqxfpax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xdaxlild.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nzjelqxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rnkmjpsf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tvfocuux.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2gchstfrv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2imixwfec.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhtarthh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsklrter.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qmjwbard.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ozqafrcn.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2xvqluhou.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jidpjldd.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2feftdfwr.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2tphwdazh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2oocwnmxf.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsobkhgq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ethpaafj.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2rghhhfel.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2twzcihsi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ptumsiuh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2awwuppfi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mprcybfm.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2tmhhbyfo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnbgzljo.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqlqgiks.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmdplrkp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zpqpsmfb.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2qcslysjz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ypiedwso.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2rrktxntc.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2mxfqfpdz.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2htyozpzt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wvnhunyb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2deyxpbfo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2cfsrxigk.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2qdrfjnia.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2surnvkqq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlggkzy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ohxoqxvt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2jeugqwth.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2mgxweiqn.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2olhjcyer.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2iqrlflyy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2arpxnbfl.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2tsixnhtz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ybpkrvzf.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgphzbiv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2ayrxkscd.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2lidtktac.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2njufdakq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2qpzlxjzb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2sdtqjven.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2neoxrdhi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2obklzfnh.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qmwtnuzv.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ejbmjiwl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2wkurcswm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ahkhdxec.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2doycffcm.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uklwpzvm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2ljanrmas.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2rkdaqjzx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2bswgysmq.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pugdcvdu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wrdzvndg.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ezqyjoaj.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2thpeokba.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2fjmbabvf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxuvhulp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jpgvxzez.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vxdphyck.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nblqlxzh.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2cpjovzzn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sozlojmf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ngokekmv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2zbgkezxx.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2gmqwgtmb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvsvmkxz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ssdeajcu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sryqjiyb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2naxrbsah.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2dtfqhigb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2muxqblie.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2rksmvfbt.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2eorooqhf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dabbtrfe.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lbbrrhun.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2oqjwbcaa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2icplmjvt.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uxfiogse.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hygaerhj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2qsvzkiru.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2dgotkhqu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jvstogbg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2yutnhadt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2thfjntjb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2mgeahxkp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2bmvydkmw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2tijvdcqu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2pedbmpsp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hdfwinxe.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2gcivbxvy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2cuzttstm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2ckxoqsew.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xcwpqgpp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2fhblpswx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2nffslcjj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2nnomnvvp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2fpgtjwhy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2sdghgdyu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qiozpemb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2emqoucib.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vpaqcqdt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2smrtmfrj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2lrjqhzos.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2debgnkrx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbpmzhzf.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xhptzpsf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2vrfywtxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2midsnbbw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2pyjaogoy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gdhwbkfw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2osbfjpae.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hwdvhwtw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmpomxpw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xjtfhxmc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2ekmrdkzg.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2uwilvcef.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2myrddprd.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2lahtrltq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2evidrmtp.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2udoqwmax.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2geklzekn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjapzzjr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2oehagktn.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gazgqjpn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2obdgpnin.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2gjsaxzlm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2vjdjbmsc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wsroqxym.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2qaxctjpj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2hyvtbrou.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2yhiopktn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ciopgpry.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2rxugkkfd.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2bvbuqili.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkvrgiud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bkgnbmtz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2afsafszw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fllcexdk.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2tgqbctbz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2oenexbfw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2razypywn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2exhxvhtr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2qprxplbp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ylysoybx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qzjqcdvq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2eclhqlhi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2wuupcszb.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2pzbzfcad.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2koyvrqzo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2mwmwfvwj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eaxpavqc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2joklgnuf.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2efmxlbch.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vwpxfzpf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2vbfeytws.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2qmkgpwei.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2gepoegvc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbiwkpas.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2zndhdqyp.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2sgwqysik.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sgoalutm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2whguuuju.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fnzklets.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2jqklomih.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2awekhzdj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ntwmuozi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2blpmpfmd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2guhcqchg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2itamhpln.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2diouyebj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wzzmwvio.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dkkcrssy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kelhznkf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2gazqscll.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2smtbyrnm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hpzpujzk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2qqkvgiba.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2otmugtbb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2xkxujxjq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jmriuvwa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lokwvnuy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2emdgwrfi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ycanjhpc.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2doltmias.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ygkmzojx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hcqykssh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vsksqfzz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nlhvdebe.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2osulzktu.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kkvlupep.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2zohopppr.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2tvasfwxr.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2fcszkstz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2uevjgdby.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bgkscfco.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jxbazcfj.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ltbjptce.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dqkfgzxm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2isqtrzqn.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2kxfnvgzu.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yvvhbjsd.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xpsljstm.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2dbmhefqg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2ojtcvrah.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2axjnzoap.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2jbrctltc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2vgyrdddj.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2kjlgcfbm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2swyijrhv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bcvvclec.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wxoetywi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jhniqebu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lqipdpzf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2dlsrwozd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cfexvdyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2sicbcivh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyxlhkec.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2drwrdevu.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2oxudbuix.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2lqujcfji.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2lekpaywf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uyptbvqy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2mokujeyu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ecvephuo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2jsqlemfb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wzpqwblf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2ebpwiadq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2tyfehjxv.html


<!-- 参考信息 -->