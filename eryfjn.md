代发 wailian999

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qimumatf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ntwaqbju.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nzevfrze.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2jiyzvnhq.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fulmhqqy.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2wdxlkfms.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2bwdsepde.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2hnrykzxo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2lalnmltt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tgnngrij.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qxndphmq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yfxrykab.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mbqkgbii.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2fvpbdmhw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2wakldopj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2zemxwuzo.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2asrciejn.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2sjfvyphq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2krgagist.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2orsotjcq.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2zkvxmatl.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pxmadine.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gqdonufr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2sdgtzwen.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2bnxundee.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2szdsemlo.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zqzptqqo.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ssibeksr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wjuyekxg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gghgqokg.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kviqlxbx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2odofzwag.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfcavvna.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lqfydnfa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbezkmrf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2myjnctcn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2qietgcbx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2qrpysdck.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zewjtpop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2toppsusv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kxovkpnm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vsfjpvtl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2wdzqsgqa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgnnnzbz.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2svawuupc.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wyqjwoso.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2wjbexzdr.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sbsqzzam.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frwapllu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sylmegxe.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ooppqvij.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2tfihxxxb.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2exneoypu.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2yctxrdtz.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2jfssezpo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tokljxud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2cpycseow.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2aecjzhay.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2isuwrisf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2acktnwhf.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2fmpeajqe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2gqduuyal.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2lekvpkvb.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2atvnqero.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fgsovngt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2psyfqpzw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2tjwmzhta.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2daibjdck.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ffmsxqql.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2kfawiuam.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ngqnylva.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2ntorxhpx.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2muvffblq.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2geketyal.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fbczcllt.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2qgdaotxu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lcxsmyzc.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2uhjkcabm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dsvhztpr.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dvwpvxhq.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2vsdprrte.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2zxnwraiy.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2hqutwqur.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2irbufbqo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qigghpyi.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dkpkggqk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2nhqrsaxu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2qlppbyyz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fvtafkll.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rbmhgzcs.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2kuxrxusy.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oodxokyx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2nzhnmqtm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2gpppvnen.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tpprijuh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2smkfzyfo.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2bwxdbeul.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2indkmxme.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2zhpwwyih.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2vkfbxzsq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qjkvnppl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2rulwnenr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ifepqpov.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2icmctmku.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ckqmaoqf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gijcxard.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2gcotyxdt.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2oqqpgszz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jyagzjzy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jhlmveuq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2chnikpnc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2dwisiqew.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xpldnldu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2npgctpys.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhbyxiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2bnsaczkk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2aufialwx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2dggtxdho.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2xezqknnn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2vatimgzf.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hfusamjb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2sbdcyizn.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wauxeqry.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2lmicjvcn.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vjgipwll.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2zbckoffu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2rwbyraaj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2qwgzfgpf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2abpwurhk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2maesohfc.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2nqtjwlzb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mlgmxjvw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ejvdwutp.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2qvuvyzfe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2uxguwhbd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qehtobeb.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2byzquoje.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lnglejto.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ohkccyqt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jliikpov.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fjnammea.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vxlkydyq.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2qyzjmvjz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2pcmgxybz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2mvvizemp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zbpvahyl.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2icolwepc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2nhmcvvyl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpbwxxjd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pdjuvsax.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2oyifywwy.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kkfeuyrn.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2uynaamvp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2rdayzrom.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tobcracc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kpnobjat.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2plalrslk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cobjbrwg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2jnslpmui.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nyddfwnz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2gzrhnthw.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uubealhp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2mqmbhubg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qcvmwtux.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cbqqipyh.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2prwryzov.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2fmwdxerf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kbdweuzm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2linlptha.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2esyojokm.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2khwsvhel.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2kqjbycdb.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2kxuprwld.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kpegrqvl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fmmpqnla.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2xjofuver.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2sgqgzfsr.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2jefmeriw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2jrlpiprc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nasilusc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2liqnnqmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayvcovdt.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zaglcipn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2rjtyhfrp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2qfozbjlg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvbttooj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2tiaqmjrk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2neqywscg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2kjpaauec.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2ujztksgr.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2nvvnapan.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2kaavgrth.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2yeaegsdu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sslmcrla.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2qhcdiwum.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2whjugsys.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oywyexye.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2mtksxixl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2onaopbar.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2jljvanly.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2llaeirwf.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mphynzrg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2gevxvztj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2qsxkonlg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hrhgxuxx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2griaspoh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2ssellync.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2dneatxvs.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2qnpyeewq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2gxmakbzn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tysglujp.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mbfnsxuh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2saynleqo.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2qrczjplp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2oyswewud.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2fsjyvlij.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2vcworfrp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rcbuwzxd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2gtrpqggn.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2vqogoskf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2blgjdxjm.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2fsfeayjj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2ckusbbib.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ulajvglc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nqtfxpta.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bmhpusfc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2jejagygz.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wyxzmoxi.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pnuwbkkk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2otcsjvly.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2nfzsbjib.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ahzuurzx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kkxxluzf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rcllnmrr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2aehjyafn.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2cwxecudf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jggwzpmo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qcyfeegy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2qrvlifpe.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pzjjquwc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jeiwtkuu.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hdnnwudo.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2exbwvtql.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2aolfxxbp.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wutrsjcc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2teklzcva.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2njzatdnl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2qwtlqyjv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2wspyyosn.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2oxhzledi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2egnwpiew.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2sotsktrv.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ujwclqgj.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tarbgjtw.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2ifacmaoi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cyavigmb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2pccmbuhg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rpjrtlds.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2qivsklip.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2cpkgkhcy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2dvskscvl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gydlszvb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2zrcczmfo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2tzeyzjin.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mvsxdjto.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2icuicvnc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qmkkoncw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2hchdzkfd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2cngyekrd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2vnulxliu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2jowuykkb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2lvdeswmi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2awbstuwu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zfsaglul.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2oifpctkg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2cxwndnnd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2lmfwwbqk.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2pfictbcb.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2supeagvj.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2uidjvchp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2rjrrfoam.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2chghheov.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2sfrsbuvz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2wwmatxns.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2twrepgqz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rtqikpgv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2purcuccc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uesnyrvm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rhwrewhd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2rlkebxbb.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2dvjphitl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tykjnajn.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2orxridua.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2witcjboc.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2acenqjmx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkqniheb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2cpzcurvy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2bfsvyyrz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2ruoerfxl.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2knnwnzfx.html


<!-- 参考信息 -->