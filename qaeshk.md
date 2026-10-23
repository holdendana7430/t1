代发 wailian999

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qnqmjaku.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3ytgmnbnr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qgnftasv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nywyrlws.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3kcsdcjcq.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3rawnxndq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3aqlnmaqx.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3cbbwbhpy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3disudyek.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3vgzkjeps.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qldiqsyn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3kqnbxoco.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vxkkjags.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3ldnlafdw.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3tmtqpjkm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3pdekeozj.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3huwdnxww.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3vzaghsjx.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvxzkjv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qolqgrds.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ssactjas.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3tzuwqsth.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3hpdsbooh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3plctzqep.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3btzmbtfv.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3bbifjthu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3svtpdqrm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3dupisnqu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aicvybqy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3cuwynytg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sslkjjox.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vntryyjc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mypkufro.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rzstsdjz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wniidreb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3bwytpmhw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3uxhqwdot.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3naqecueo.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bgohzxmq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dmtbagyl.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ojvcajdk.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3skdkywua.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3agbbrgxw.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3acmpvcae.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3ajwxozlu.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kesmtnvb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fgoakpoh.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3nctychwo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3pslyywjz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jtcooijy.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3wrpgmcvd.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lrpnoqum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3khqqrcsp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ywkichxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3plaqzgwc.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wkuhglkj.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3mmfqdqfo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vxgpaohg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inoypfst.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mzqumjwf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yajkqomt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3sairyjdw.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3rvgcicxd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3imrsgjzw.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3hatxgmib.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3obcfhmfu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3norzbyds.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ptrmgnhw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sywyftfc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3plpdansy.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3zqdxnbbn.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ynrnkjda.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3exaynade.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3tleijhai.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqhivdh.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3msskajyv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wbxcslus.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hppgcryb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3aguoirpj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qvfuphwz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3hpcnylxe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3nsoacfdw.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3lbzfiplt.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rptgcqhv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3pntvmreb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3myzxcnhv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qnulxqmv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3wpmfbpip.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3vvzseenb.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3dgcpuzsj.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3njnukfqy.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tahucsaw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tfdwkzxk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3zqvltiuv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kpkrpdqm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ftwirfug.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zfccqwdb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3pedzyoeo.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3gdfysxxj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bawmwaiq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3lbmahuvw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3txnbympm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hokbsihq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ajpwwjfa.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ldemtcvg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tzyfhddy.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3ablcsfgs.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3brgzfdsm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dzxiftcn.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3sdanyouq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3yvaogcoo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cqjyfwox.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3pbzlitah.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hsuvbsyy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jqwxuyhw.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3brwaessj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3uaignjjy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3sozfhyhm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3voazwrnc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qwrstisb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmrucnbf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3yalwcwey.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlbyeuw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3ttshdxpp.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xfbrette.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3agnfoyqv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dndbggzb.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3tpfxjesw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3xfyufhld.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbjmctkn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3wnumqbkt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3jkaxvfcl.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mdjyiolh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fsibikvp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ufeaslok.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zlcwjdxh.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3lgwlrevf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ywwcwwvi.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ucfradsp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3uqnjijtg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dghqtpns.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3idfjiynk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3gokmyzco.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zorgijzs.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tgigylak.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3wrfnkkis.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3hhgtkvch.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3ezauauoj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bqefigqq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3vlgzwpnn.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qzuzafqg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3xpoegbko.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3cxxetvew.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3ijyzyhxm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3rlddzwsw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3znnkrnto.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ymottdmz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3hbwkwfox.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qwgrkvqy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3knnnjghd.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oqsgppql.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nleisjjb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dbbsifsf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dphjnomu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3bdnzrqvi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iurhlpiz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3xisavmhh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kksgrhqr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yggkismx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tyloeijb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3hkldljlq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3dhgwfdys.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xlfcbekw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3qlpzsizd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mgqnvgfn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wtgqmbnq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3obaxidcp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ntvywerl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dluwddkq.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fuszcmww.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3wvpkelxv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ubzsnogm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gsrapfnl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lnmtpwqm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qewplafo.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3jdefdidq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3wpbijocq.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iytdvhqz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ugzwczop.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ayalodlw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3rnetqxgb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zfidkmfl.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ebnknfzm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3hhhwsrxy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3wddufkib.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvtdcnqw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3xuaubzjj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gsiawjns.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtsfbwdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wxwiziym.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3gsfjrmkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hnaqnlii.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wassnsxy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eixjflvv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3mozykgxy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eoxpjrch.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3lpptwkqm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3tgcghjrt.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3tzdyarfz.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3szxcgzge.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3lekdcvix.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3aexvcuob.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3dfvwqakt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hossastj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kjmtysyc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pczomhxe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lxnbbkpf.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sclvbzyu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3xdhvncup.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xuqrglyn.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypzcqhry.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gsyyxlrb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3oztnzvuo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fueflrnp.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3uobdnhzs.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3onkczcqn.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3jftfhorj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3neaybnng.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3qlnxxhzk.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3onioxpwz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3ficduzuo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szgjscwx.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vkwrknuk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ksxeygjg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3rhtptmwr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3megajxgf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3undwpywk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3vtatdocp.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3lybjsyck.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fsrkhyrz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pqbcnqdw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3pkyryzny.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3tqmyedaw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3uasrplpe.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vrddeqpd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3obuigokc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wjnumvpi.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uxmgmjzj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kkfkmrhl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jlylrhzo.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3apjucfkl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pnxnilwl.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fgkhepsf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bzhvnfwf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yawlorww.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3supmfndh.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3qpkevqoj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3iaktxgem.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rfjpgsot.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3cdchykog.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3iabzedsn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3prlkaxmd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rfrhbeol.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rutwakwt.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3kodbpdlp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3clwkmmmg.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3lkejxize.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ptlmmglv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lbgiprda.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3zpanrlts.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3lyihdzts.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3htgmejkk.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3egtevege.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tfpxetge.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ountwwqt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rektifiy.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3hfmrfjqx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xchdkmco.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3fbngcwek.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dmfnbofk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgarrgj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ygpdibba.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sftgslhy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3dlccjati.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3jinoyhml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3hxjldxvj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3qjtszyiw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3puksxsml.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mnckfzyp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3amzfmgmj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3kjelcqyg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3vbdzsktt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dsjgtcuo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3ezgespyz.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vweapanj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3qgzvhacj.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ltiwgruk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3vpgrsyfu.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3douutdct.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oevfhwof.html


<!-- 参考信息 -->