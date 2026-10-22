代发 wailian999

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2zmpedcus.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2htzslxsc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2xsdmemvp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2qlulmorg.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ahuzhipn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2ydhkansb.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pgnpwpzg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2riffhpvd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lbefhslh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2ycqhnavh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2yahkrmgz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2vrkqdsjd.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dzsmzmoi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fcledhcm.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2asihvxvv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aormmzoi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2quanyrwf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2cwopjbck.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2dxvaugwx.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2lxmonght.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2shxodcis.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2etervdoc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2hjmrgfeo.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2zmfjiffc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mropnpaf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ateysxfm.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wbpytncl.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2bjmvjbjq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pidisvtw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ghdqkdej.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ivaknbaj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qdvijqne.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2murbbagh.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iejplkgd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zaglwret.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jdmjgwdm.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uxvjslnb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xptadueq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ctpuugwk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2likiqoms.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2oxogtnvf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ooztuoyx.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2nltcjqum.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jfsemthw.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2undiukvh.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2snfytvfa.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2jcgkgcof.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vnvezqvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2moqkwkub.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2srnsbhxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tndmfkam.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2mejvmdrr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2fibykpzo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2domomcbg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cscvmgop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hngslmqi.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2meyujggi.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqssvtnn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rpzvxewl.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hmjougfh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2gxttqkws.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2msazdqjv.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2xllvfcil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhvbeopd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrjbtvkx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2hexghwzr.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2uzgmhvni.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2pdzjsnam.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2pkmcnkel.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2wpfontyg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2hqiuzxhz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjteoks.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zkzuwrfp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtsecxjl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ehokqkfc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2cruaiwqm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ujxvwbwp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2upyfnvrg.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ncvzsgsi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjpnxi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2zhvtkknh.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ximecrba.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2nptuzhad.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2rxvdjacw.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2yjoaykwd.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zbkyiapd.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2saodhqyg.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2shumkvff.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2onkpbyid.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2mhpztdhj.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xgenmezf.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wwrzgfay.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2kqjixfzb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2fvcmbmxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2clntiiva.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2cbbtylqk.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2podqsqkj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2cavjdwhp.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2tdesytli.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sagsstjl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ivhcryet.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2vrimavrm.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uoicfpsg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2jknzmkia.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dsnllbxa.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2hjkuvloc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2vievltdd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hvbzkaxt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xbffxgsu.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbglhkv.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rykftwga.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2bklttvbn.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2oigydvcz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2onuybbhh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rogoqrnd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2igcdbsfi.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qivtfrjf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2oalrdwzd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jfurhiah.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2txddpgdu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2hrlafvof.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2iiuhvgaf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2anbjrwah.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2eeeouweo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yrzhnkgo.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmquakjp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2aitivwmv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uhcuxzpl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2rlmqkhfh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2yxmphxbq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2drvyzdzt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2glrcjkhe.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ugrdqqiy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2ctrpabit.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2kmifjhdi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tblhupem.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2pytzqfxw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2viftbinc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2rnfmtdwn.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2kuxkwpci.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aqjmwfsu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2bjeabnaf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2hprcqrbz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tpoyrhma.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2zvswshoa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2iwlyrstx.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2opsyjqdf.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2jxrmcrpm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jiywwrji.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ydowmnsp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2cnraemtu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2iisditdq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zdlgzgmp.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2johccegd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2icuoqhna.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2eufvcxxv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2yxfsyxre.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2cpmgycid.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2odyuckwj.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2jtbpbzaq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2xeflacil.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzvlrldd.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bbtaxbng.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yarmekud.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvtmcasu.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mjriqqdl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lzgpdmwy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2lgkgdzhg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2tuzgysbx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ruvtxqkv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pwdkhxjz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ncgzzdzj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jvhvxksb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2snlzugas.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2emenfoyb.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lahnbhih.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2mktrkose.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2wwnacqes.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwfbpt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2ivqqszlc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjyzqtjj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxlefapu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vgdjpcwr.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2pyglkwxg.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2gdgncmvm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2kntgaxgk.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2emjzulwh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2syexmqfy.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2wtebcbjm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2tafoytol.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2alnowtet.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bsdxbnyd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mqbbfsny.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2egfdapbc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qcjdebet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kyfjrdfr.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2pjrpzabn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qitdwzrg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gxwtghes.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2hxgqgdrv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2npobkujg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fkxfiaid.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2xhjtzppc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2bdsyziwg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kndtbvcf.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2vxpbesxb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2afgqaxsd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2oiyrifgt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2lonkvils.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2xciakpcm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ntjqxelw.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rlhhbzbh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2svubrpzs.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2watqlbgd.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2qeozjjmv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2bwkozvpp.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mubklwxa.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2eydtlbls.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2yjvddsbd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qcudmarh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vioszjph.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yjbkghbq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2fxopowlq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2rvxaevtp.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zkgomlzz.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2knqjlyvi.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jcbplznv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wlndswnk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2tsgofvks.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2ogxcgirr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2icokqtma.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uterrczc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2oeosozlt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrlbmizm.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2nhbrgzjw.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2stqlsbhz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2sqwipdgp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2tsgnhbsl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ydgaxztt.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2lhpvvvil.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eiptybmb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bxctwjmz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wlwxgvou.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ezdazzjr.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pxzowqve.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfeokomg.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ryjvewdr.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2rxubntba.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pvsfwwkq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2juimhuno.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ggwwveac.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2njlhlkvt.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lzgmjooi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2hfhkznin.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jddufhrc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hednqhqr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bnjkscqj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2dndspkgr.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2iraiyvfb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2zvycujfv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hhcxtgal.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2xfoubfpr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ibblczaj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2fapqelzz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2penikdhj.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2hczvfygz.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qqhmtukk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cmunvvft.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hlsnhhuw.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2psjfdtbv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2xoxadcfo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2zpchighh.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cfndhzsh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2kdykzjav.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2ttkpcuza.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2fmrslxpa.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sxecnugz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2nooshldr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ojmewtlt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2jcxwoene.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2ikgvpdoi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2avuywvkx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2kabhkuqb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2esycivxr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2wwlzfdkg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2nnutswsk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2yrujjhmk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2sppkavvk.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2ynajztoq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2beljtlov.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2ksgrvzzj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2vptakmby.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kpaxnwlc.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2bigsveqy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2aexqlnwo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lgpjwjmb.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2rawqapxv.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ugayxsep.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2kxdspdkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lbmvjict.html


<!-- 参考信息 -->