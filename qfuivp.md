代发 wailian999

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dzpsgena.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3yqfcgogr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ifxmleif.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3shkwbhkf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lgwoakdo.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzumretu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3vndsqoam.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3egxhzxiu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qskbqusq.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ghdqushq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aftrblkv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3nylchmia.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jadallon.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3gzefgmwe.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ckjpaqju.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3twdsremu.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3skcrwrna.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3suducseb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3xkqjswsv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vdqduqjb.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqfokkh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3kwmtdmfn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3kdpomvsr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mtmbovft.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3tzphkumt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gommmhlp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3yztezoxu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hacexqpc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3rtwnsqbe.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jpjviugg.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3mqlfftrb.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zdqtwaoi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3svziudei.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3sifmqvks.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fcikctcm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3xkslvomp.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3mjhpsjdb.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kfkhhrxb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ffuybmeh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzwvuov.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ikdliemx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jhkiiwuq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3cooemokb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3urjedoou.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3wmlijcwl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hcgqcexf.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jonbltqj.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jofzioay.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ohnhsdll.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cshxneju.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jptsfmtm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3osyutmuw.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3wjlqscff.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pxjlyvhb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eplbjmxw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ibpugkfs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3njncudft.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvpbaq.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3yzoicekh.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dyffugxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggltnuqr.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bqctwoht.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kyxbuhrp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3iimfefny.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kstrdzub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bjvvwksa.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3peuqycyy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cwyyosyc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcmmqpun.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ijupbqwq.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3egimkdsc.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3oehfiisn.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3paxvqlqo.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3mjvdkfcx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vypzjqks.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3woxnugae.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzszkwzk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3pznbssoq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zjefctkz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3nyhhwcdx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3pevbersk.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ibiztymj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3todxdoys.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pfdeenlj.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjojphna.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnjxiuco.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3eyyedgcy.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3ebxqbjju.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3rckyusiz.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zrtkvtft.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3yvpultrf.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3hpvudkyn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3klcsmvjl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftviikns.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gwjrgmqg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3ipdrhdbr.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3sxvznfsp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ygrashgw.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dnozenuy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3wegkyzfu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xcihezeo.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3jcxeucxm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3tjdwlbop.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3fejptkjz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3cbpbqgwe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3frqhtmoz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3ulnoidra.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3scsuloyh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3elfihnwk.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3eohgsrzv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fqhjqwsw.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fnojpvbw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zzomnacm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3wfkixzlu.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3lxusvmvm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wclvaozc.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3rsbvgdlc.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mrpetztm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3jijmwptd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jmvtslox.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3gdjnorzl.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3nffyojnp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3kkknqjtu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3yepnjwjy.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3evnonciv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3fdzzvgqs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3zeymqftx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3rmxdhdxb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3nktshoxd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ejxsajwh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rqrncmbz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3mxrgiozr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxlmtmjt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ztqndbxo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzrksxrg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xsrwoiup.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmwboqww.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3opshcjoc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qdhafblk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3mdacdnen.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3tidkuzat.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ctinfryj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3elbagjmx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ljzfnkde.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wenvyrgk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ezpxcwpw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fmdnkfqn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kmoknsat.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3arbwwxgo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uwuvipxt.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3erbvefog.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3oblbiskm.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hbsxhtuf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3omrakjek.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wvazfigo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vijzxuue.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pswkzyos.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cqsvclhi.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lfekersq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dcfbecvp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3bygqenxu.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3oheqrivq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3pgwfehkx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3otmqhefu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3cgnxsaan.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wcjradau.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3bpecrgyp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3drkpejlb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3jdadniaj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3qdvorana.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3grudlytk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3acdhksyb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3getguome.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3prueobaw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3duveaxmh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3scvfscza.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ueilxbtp.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3pbbvvqah.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3pcfnwiwi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3nliiltlg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3frjucprt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3fzvecpcv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hmtpxlgf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3drmycvum.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3roaoqtae.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3vtzogurd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kgiryljs.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3aucqaxrk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3objxbwhh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3qeznpjsb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3bephxuoc.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3phgngvcl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pujpjmzi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3csudddht.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3oojkhjsj.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qpuzoedg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xbucighf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3rmkbytdg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3gtgxgwiv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3wjvhysyp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pwoocori.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3jvqilbep.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3raoeoyuy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eereydlb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3cpvpqifa.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rmoetrez.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qtlnugir.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iywjsjue.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ksvoifka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oputaovs.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3dggwugrv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wehezudj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3reiobkpu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uhhrslqh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3aqoqvpkt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3iutdsbas.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3zigxieae.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3etrzcnsl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3sfhzpcic.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3rcddccqt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3awvullrt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jxjzmrvx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rwxbpftz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lexdubib.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wkcctwnd.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3fmecdfns.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3cewgrsvf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hwhxwfqm.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3zwmjlzir.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cwiycjqd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3xweztwdg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3rqrionib.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eujhytfb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rnwbrhvy.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vknyiscm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3xuvbiase.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vzxoxitk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mmgtkrhg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3qmjhhnhx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3frszuchy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ltzccogr.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3esstlfkv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3onzfhsxf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3qybnaqji.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3mppzyxpc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3rvfjhegi.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3kdejuplf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3uirznfoc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3iganogqi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eaireoab.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3eoysajrs.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ucsmacla.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3tnrhtlwi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nltrvqtj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sffsrbhm.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3knrllecm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cckuwuqg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bjhhareu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnwbmw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kiqqdwst.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3zvcjiwby.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmuhfe.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3asfqasfj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3tlifajgl.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xynmwaod.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3axxlzkdm.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xagiwuqi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3znrlwybu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xzcfyfig.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3byqwyfan.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3cmzrhqed.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3sgzwokzd.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gyjuoxdx.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xhgepier.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kbvgegry.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3verhpget.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cjtvicvt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3irsbkezu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mgbnirfx.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pbjdromv.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3mziixpmy.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gwvjpsil.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3zonamvls.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3euywmbfg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3scjblhaf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3fercapfn.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3uymzvxww.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3evqqfabo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zlfwcwea.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yhzmhjxy.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3vdzitsiu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vwrjqnwz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3injyvbfd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3upbfpzdg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhihtqm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hnvmwscu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3frbupnjb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xuabebqe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ywgohffe.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3goxksffg.html


<!-- 参考信息 -->