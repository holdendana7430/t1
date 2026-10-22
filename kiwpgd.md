代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jvvqwreg.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2isvyhnuz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2unsncesp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2gxwlfyrp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2qpnxaxnu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gdsaktqf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gxsymllg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2txhaovpy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hraejhpe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2qkdqrghd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2onfzckiv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2wlwrnpnf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2jmdblcgu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2nzyioqhj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvywoej.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xxywuvzj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mzvvluki.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qdmmrdfp.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2lkhtpfnx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2mcevoclm.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2meudjlsb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2eqvwphbi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2dmfildea.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2vdjezewj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqshvpk.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rbqduzrm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dzwlniqy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ezyldarb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mofxjqwo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqigdkj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ydrvkzyd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zjvrqsll.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2gvhtpzew.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pwbefajr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ododluba.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hluxakmh.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2priuufpr.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2garstach.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sajpwnme.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lotldhvp.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dtntgoos.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2fosjvqmz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2oxbzyory.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ixffucjk.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jycaufcc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hioiikrd.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hzkyjwlo.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2ujwvxjbw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzymtiih.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2yozukppr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izefpjfi.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2aiupaanh.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2oothtyvg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynrlybgr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gmmdxrgj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zluyxuxw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yaztkafn.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2nbzchbev.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2iodfipls.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkxtbyxr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ajqaagfq.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2vorsuuyu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2uxsbggtj.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkqvutvm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rzitiuqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lekmjtbo.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2nbjivdma.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2iolcmddq.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2hwlgdfyn.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2ghksffga.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2sligomkf.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2blhmsdmy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xmgwhnfc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2kxebgtjw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxgymmfs.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2zfjjiale.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2yibuahvn.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2pwjkvvjr.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2dcswaxqa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2fzfvzmxe.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2dtsylhsx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwunyipa.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2trcdqcqo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2pfhnvoqk.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2lgjsenkb.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yviutpsp.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uzqxjjdq.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2hemlqclj.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vvvafedl.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2csebvkza.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2puuulddb.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2gpnhnhgf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2zqjrtfds.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fwuwuecl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2hdeeismb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2nottrtjw.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2cffruuer.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2dyolvtvk.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2higduyvh.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lvzhiwyg.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2uututdbp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2pljjhgak.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkrxqed.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2hetllndp.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2ghnwimwb.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2uscvinhf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qdqqdfoj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2soloiktk.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dizgqcak.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2uontzfuo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2repyadsz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2uazfadfm.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2perglszp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2pxyclfkj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2vctlpxir.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2vfmvhyhm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2yyzltdsu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2brafeuux.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mnjalnur.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2oumazwsj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2grynvqql.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2imqmoybo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2rseowjgz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2xcdjybpo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnlptgow.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fnnisxlf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2apwshqba.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2fnajtwpq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fqhgmssw.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2xubwsfqv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvjbtbaj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mqgjqmof.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2fhzjnjsw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2fgemmtzx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cbtlyurw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jcenyrmg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2yxncytyf.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rhcxekcb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zlgwkjak.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2yyjszmqq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ksomipyt.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2aukuprqd.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fdnbnvdm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2fxtarwkm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2vfcpaxgq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2xvicyfpk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2jbqbuanj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2gotwzdxg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2cypcoams.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vtkvfoyg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lbentuhw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2rjmndsxh.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2qfjhqcod.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lrbzdqsn.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2zefpgbbz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2ewkolksp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gohntvvy.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2cvpxxgai.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vafxpmxb.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ukdtgvlu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fdpugyei.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gclhsqcx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2cvmgukcu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fohdpadr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vsjqewom.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jnolojjt.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2whoqjyhr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2atvekcik.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2nycermiy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gnbhsszf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dyplecbu.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2krdhjcce.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcgsewyu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2tchdnxoo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jjjvigjk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ubrszdib.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2atrgruad.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xbrmfena.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2pzpnhllh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2clkfrwtq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceknupmh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2irfsjhfa.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dilqwsei.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zmecavvu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2afkgwmyd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2wwcczobr.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2opscnuje.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2mdrcmqab.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wpwdrxbn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2qevmnzpn.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gusurpor.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mimyydgz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2imxnqzqm.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2xcsbjvfx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvauqzfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pbdblzws.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2ceyexjkd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ztjwyuol.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2trjseefz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2knrbuiqi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qzmulxhn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rygarqrp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2arptzxbr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2kccugkaw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2fmlvmqgp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2wbxwnikr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qdieykce.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2ykmexizh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2omyyscbb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2sdeavaej.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2popqftap.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kibakmky.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyprgmmx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qdonrzbd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2zvmkgrav.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2greqttrr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2xrwyphzq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2xriipqhj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcpadxaj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2whdfpywi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2edltjxow.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2kopbrryc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ovehmyam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzpboke.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2aoedkfat.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vmotbtwq.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2qmhsqivq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qmnkuxkx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2xgodkskn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aotcbvkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2okkdxisq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dvmfazrz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tainecnl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2bdrevhiz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2qovxoyfe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2zoczgazg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uiybqdfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2udsfedxr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2cpklrgbl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2skpdaunz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2lkabegiq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2amdipdza.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2jjyiumwb.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ftvojjku.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jedqmtzd.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2opohcppd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kadzghxg.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bnmgdgdd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2qdtpiqec.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gishuybw.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2rdjjcgvf.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vhboyuxz.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2bknztqdl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2avbnolxu.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvijpgrn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpcomokd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2kwhwbjut.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2pyjnjpqi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2vnkudcrc.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2debtsjfp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yewxtulo.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2xuixwtpr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2vvymhgjr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2zeldfxsc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2dvomnvqw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2krhnsyvn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2amwavyro.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2jkijqiqd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xahznarf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2vlontmoo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2fhgnyzfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2daafwtqe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2kbuzgdpl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2idhizsoi.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2gjlmzraj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2mcotoafe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2eixsmojq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qfozxbdh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ovpolasp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2wpivaynd.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lylaxbxm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mabriyyg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2xubcxerf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2idygtfnd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2zbdcpikr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2awfuzfrk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2hfcrhmtr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2grnxrohk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ozlxhpyh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2crnmadcs.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rqbkvyil.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2mmmtuvbq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2fhdpelns.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kykftpak.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvbspzb.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rgfoyope.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2cgfgxbrd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2yddjlkrm.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2abqzwssj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jbfmmyrz.html


<!-- 参考信息 -->