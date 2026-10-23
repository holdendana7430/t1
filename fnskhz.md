代发 wailian999

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zxcsttak.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xvusvnnq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gmhcrahg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aicrizsj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3otihklzs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufveykmn.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3frmzkigd.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3izljwccl.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3hzmbgtbl.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qprurvhq.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3psglwlno.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3smgtwbmi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3memsmpmy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3lzeipgvy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3rvbsyooy.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3biwluntr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3szflkoug.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3lwjchsde.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3aopqbrep.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3owwewelu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqshgikl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byrifxmn.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qhmroklw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3kahzcsls.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3xwbbkqvi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kzeurjzl.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xrsmvkex.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3szdyvuie.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3jyadtajk.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ydkzvicn.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jplyxseg.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vtyxtokz.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3udzyadof.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3sjjfqtsa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vlpganzr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uycnkcqd.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3aiageodc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wkafrdtp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vimkyhdp.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ktgpnlfs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jqvnlxwn.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3bexnhdzq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3atxzhcyy.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3arkkczeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqgwplzm.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xrbttkxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugaxhatp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wrdcypak.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vtyrqovt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3llrblxuk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xypvilec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hgscdetw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3icsytzqu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ikysakfi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3galbhpzp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3knfuugdb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3kxvtrhal.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ogpoxgug.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xxmnbkhy.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbogouxd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3olnpsqgx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3onquupeh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3khiqtdwa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3cxeqnmfk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3umiuomhb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3irjcaccd.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgnufce.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3romfnofk.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3pgxgdvdp.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yritidjf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vprkbsrc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3mlfuabnh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3orrhjfhe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3gcdngfwn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3qwwzlxkg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3yefeankd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3wvfxklqa.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vwcqjcwm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3peuihwcv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3iptxibll.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3tpaxfyva.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3bqjbwtbq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3legrpacm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ggtaswap.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3mqvsjuya.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3yhqcashl.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3yigtfzzl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ommjhtlt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3bgtltzoa.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ghqbkuke.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3icfhyhic.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3vxxusbqy.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3bhcywnri.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3omnvzgrm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3fqmgzboo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3tssqqwbb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3trxpheam.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ganvugbs.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nybixfsr.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3imycxuwd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3krakxgfa.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3agulkbmg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3exbtdpuz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3trbjaqui.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3frkztmqs.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwejrjp.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfznbdfm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3dhcguqvk.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3yusxdnpo.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xyduolnj.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3owtsfyhx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3lyuxziyb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3rolfsvlu.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3loyalhbw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3amuvzyru.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3zhtukjtu.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3vookkhjc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3qnazkjeb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuajylfm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3kvjypwri.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuifinqe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3trqaelox.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vrybyuzr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wrzrgfwm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3omjqbkxl.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ictfzidk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3nfjedjox.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lzinxmnj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3onkiqqgv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gbxhnayr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zxvyvong.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pvmhnoae.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rbcuasqy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mdbnyiqj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zkgstnjl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3mzrwefdj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pdzgompz.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pftfarwg.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wnhnrrba.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3wwazopmi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3lvjqrmyo.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mqadpklp.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ocdtjbeo.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ypetofxc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3kwprgzvc.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uhqmdatn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ysaozufs.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3swkahxpd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3zwlrswjh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3fzmjgfzt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gvjdvgjs.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3equkocip.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3dfssawqa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xtdiqexw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qzlgoxbf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3rtfsekxr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3pcihrfgy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kiyxzbql.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3aalazfoy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3noxfvkcz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhzgwleb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uitgjvuk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lpcxkaaa.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qeqttiwu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fmsgntbg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kxtjnqpz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kiolpvcm.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vwevrvzc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3okkyynbt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3zmprheit.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3xvqhximm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uaxblxvo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3fwfnvqoj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pvggmcsb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ppidpekl.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3wvtmesxf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uqodtcwe.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ioqgoynd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qszkohav.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qchrqnhi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3qithpppu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iwavpuip.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qozxpkpd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3odzvbwaj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ywhkadop.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ukguwqug.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3gefqtylc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ryluhpxb.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3prguhpeo.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3yzgyugqk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sitjqwic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3alvmflfk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3vowmhqpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnhrgrta.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3oygckwmn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sesjtcmb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uxuxqbor.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jvxmcxvp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3qugzqokv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3qoklpaky.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3oynsindc.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3lpvorppy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3gigxwlqv.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wodhyhsy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vnxuemuf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3acxuweja.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ldftrysx.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3nbezqegw.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ilvoggzz.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yudgmijw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3azydhgvj.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wcsnhauq.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3fiagfeik.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lrotzfes.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3qgrxkzbc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3lwtezzmn.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ajgesoac.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ydedffuw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ncglraja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3koctdrrq.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3nberpilt.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3txepjqtm.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3elrgdbwq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3gkoeooxr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3zwabykxy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3yrnsbgdc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3vrqfdthw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3awecijym.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ucussfnk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ytmyfdyz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3chfntzvz.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ksypcrml.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3caaqrnkg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3oprxnefd.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3orlvxeum.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3daybhugn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3uhyjnwyq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xdvelkti.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xinyhuox.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wsnmzjrx.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fqtmyfxp.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qmylibru.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xaycvamv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3pdbcynzy.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3cpuqtppu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kneksgjp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uwcqkxce.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3xjhbbcai.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3usxhrxkt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3zorxtsge.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3ldngnvig.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iurieddr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kkalxecg.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3hjdynzym.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3epyhipaf.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ewskydsn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3aljyterr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3mhorsrtq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnbwkcj.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3jsvzbcrp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ovcwksqu.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3mittsxik.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3avlawowh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xqwwxpec.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3uzmtellc.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yzuguhqo.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3wnlxycro.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3urggbtex.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtipzhxt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3whcfqfzp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3felxgafu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3aszbuozf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkyymcqo.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bwnyrfcx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3fgbaxifd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3hztjoglh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3imfmfezx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3krhfnaki.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3mujjmxnm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3xgdzonvc.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mlzkvsfw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3gjucnfjg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3kzdwttyj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3mewjewel.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hqgucqxp.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lwtdgkme.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jlhkszcg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3owijvuzx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3nrppnabl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fnaezxto.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmplbolg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kgamxzwh.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3mnidkacw.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3maeodyxu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fqpovvml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3liknrpbm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3czckrpig.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xkdyuuek.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3avvihnya.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtpbppf.html


<!-- 参考信息 -->