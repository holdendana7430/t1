代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2tgcncgvz.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bqilvazj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ohknsrdp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2oywozntb.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2frfmqivt.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ebjlozei.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2xygjtlll.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ywctgnol.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zirqdjqq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qoygfgzc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2spcizscz.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjdnajp.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2owznprbu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwgpzeel.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zyweunzc.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wvcrqgru.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tbyetyxe.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2hksvphxp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bytxxrud.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2lyiimfqv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ndcylowb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2dxrabycw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2taffdcql.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2rfdezcmp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hmgnljvm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ykwjmbjf.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2lyynxvri.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wtssbals.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yovlnocd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2yaupdgpe.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xeggfrts.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2icgbqwon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uizypgvh.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zygkyuwr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fkgwlpzg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2syplxguo.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2fwuxgkmk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vwcjeqnf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxdivtcj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkdcpprn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvplfjj.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bngasjec.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hfobzlup.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmynislr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2fzbhqbjf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2wexttqct.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdmimlig.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ntigrbbu.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zwfbcuyx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2lkqxpctq.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2geozogih.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2vauetxtm.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2wiotddiy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2jvhetxko.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2loofpour.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2bhkomexs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjzcomc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mqrrczpq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2brhqkzup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mmkqltmu.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2zwwjzylp.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2xdtvgpvo.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2vdwzryis.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ejnjvhlr.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2frnrqutx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctluzbke.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gkfgsnsg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2egbqzncl.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2rsltsvfl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2zbztkdqe.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2rogiwdpe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2rqwwmjfo.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2lyjmbpil.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2lyklagtn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lxmcqiws.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrrmmr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ppyvsduv.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ibwxvkbd.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2utplwtxc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2xxzoesot.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2inhwqngq.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2feyxushv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2tlnazbuz.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2nxceedfy.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2wfvdteiy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jvlnzzjz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2uhnlzjgx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2edsigivo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nczxbrjq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2geysrvhx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2bqobrexp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2sopvapkd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2qxbzagpu.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2skrtmyvz.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2yqxpwndu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2yagdedzq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2jaaliaqi.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2gwltbfim.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2oknvclir.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2mgzyisla.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2fmrhjnqz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2brifaksr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mltnxlfz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wkopcwpx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2urlphusz.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbrmawdw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eiflayfz.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2dxgghiuf.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2luwxpbux.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ccsqssce.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2hdzwctyy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2aukruamp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlmdlnza.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2zsiazbsd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2olngdcih.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vwiirvtr.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yvzqrhfm.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dnruronx.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2iycsurdi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jyuyrhjn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gkuhfwjl.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ksfmwiur.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kputnztb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2nvcapofx.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ywaqcbsc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2jqlgezdp.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2brsgdbhs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2dfffwsyr.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ejmewmhk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2umeyrayb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hiyfhkos.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2xrdvybvu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2egncmaow.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2tgprkauy.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bvuylxuk.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2nesyfewd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2zccokdbr.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2ljimpudu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dykjggzz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2epjtagbe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2gerpwscl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2wuzcrtze.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dbwyengq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2ldqrylzq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nyulnqpa.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2katltkye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ljcnggzr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdojgkoq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fcatyiqv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2rytwsuko.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2zyckuzin.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2snbkrumv.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2ylpoegiz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ipblllfp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gcxsprrv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bphppoze.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2mbedsgbe.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2wdfajywj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2qnkkocyk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2xuzdrlqg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cijikqrx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2njwvgaih.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2oomngpdc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2amnbbvsa.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2loetlfyi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2xauorraz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ibvapxgx.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2aadbwdze.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2apdwtzzk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2stelxdmn.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2mkjqwcoz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2aebhkekj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2beisqeiv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dqpqyzqm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2iarylzgc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iplcxwqq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ynehlbkw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lyhfijnt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2fdlhoarc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxkclauh.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2xyyyvoxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmubfmer.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2fnkrfrju.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2znawvyvh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ofsdkeil.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tdjukwes.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2pepohnap.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ezuktweo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2waafhpfn.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2qsormrjj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2qxenbuap.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2oaqkmpzz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2tabodlfq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2caflwcbv.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2kvppaqka.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jepwjdcl.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2gzsnmmre.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vvmpfhse.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2igismtmw.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2glhhlynh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2bjgqjkrm.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2angjzpzb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ludipdvr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gcnqdlqm.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sjxyovli.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2clxetclx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2jviivfap.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tgavwdzw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wiehpstr.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2gqgqosow.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2nugzzwvl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nurqpubf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2flyhghou.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2gksbcfwz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wwxbqpmk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2dnbynysv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2doioszcj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2zlpduyco.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2tbplespo.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2yljvoxxg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ygdwxaoz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2wflfovji.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hwqijxcy.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2ckqsdcsk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2rygvjmkx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2ywlecmoh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2txnlplpy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hqczannv.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gxfurxop.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2uyuzroju.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mpctxyzm.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uwpoqnhl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kimxwhgx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zfmtxivi.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jpfmszyq.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ansiowya.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2lkqowsfi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2diwlfczx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qhkjbqti.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mexnwbbm.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2psqfgzcs.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jqhspark.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wvuvaiav.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xrwuvevb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zzxyhuiw.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2tbmuttpn.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tyegrlqw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2lubgaeos.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2hjqoifgy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2nbwfzrmt.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2idzkeahi.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2pbexhxvf.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2gxsqltth.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tzqhwwev.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2bawiiesp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2thzhnfbv.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrtvutkx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2nessyoah.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2gddpypcu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2vqwqcguz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2sryrxbof.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ajhbseuv.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2bowslrtn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2febxogkn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tahmrlgt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2evqpslkf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2lzhmxirz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nkhnbppf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cscaqfwp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2xugeuzsl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2ftdtqgrr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2vcxxaxxf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2kitrcczu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2jytmaogn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2noszgxfi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2rdauzxqm.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2tlanedfs.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2hbcungjw.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2snqsoptl.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nztzspiy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2olvfykih.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2kfcshnuq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2toznrmet.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nkxhcrye.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ppeqbwuf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2eqxritpg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2ivigsnqu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ldacfjug.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jjhlflek.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2ylctgwtz.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2fsvyeksf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2freexpor.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fdytaeti.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfooxbto.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2msiavlbn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qircwqay.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2kvoseuii.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2kfuhvtcw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fzwcxihp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qsphdovc.html


<!-- 参考信息 -->