代发 wailian999

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qxrcifps.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2jnelawiz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ukwnskpk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bbohairr.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vwujurbw.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xyvugwwe.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vyvxwjui.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2eakfhhuw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bhihpqui.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2onceyggc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2wplqxbgd.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wfvdfxrx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2azqkxtwx.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ksltvlms.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2gxbbyvma.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gettpvpt.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ebsrysja.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cbvsxccx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qzgoojdg.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2legxgfcb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2yoavcpth.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ssjdvrqh.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ycpfmszc.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2irxeizzf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2gqprbzxe.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2hydhdvry.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fccfrgcz.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2aywgzymx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzfwmmyj.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2axilfswy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axmcmmly.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2yumzgugp.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2andmwucn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hgwsawzb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zhbbwkke.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vgojhqnp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhaiagvy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2videeyvy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2hrczntog.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynousjhq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2bobblqbv.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2ubfpmrlu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lxcqmunv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpofqrnd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2poqiyveb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqimfp.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ddyrhgsd.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2nbpcczwn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mhwaeltb.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2pcfmvkqi.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2dpxnfkgm.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2vydktwcs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2brksomhm.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxxflapo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ngwimoei.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2guyuhchh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2kljoodqa.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2iovcpkwf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2uipgkkac.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2yaqxmgfy.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tdnzxvkx.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcyfgrdd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2sohonztb.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2vzdxtigz.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2kztedwqs.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mucladbp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rvfmlubt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2mjozvqdr.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ghfvnikd.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2kamvlhrk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jsavlseo.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2uzaklhlu.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2utkytgkb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2rytphgop.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2cwimiofh.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vgegjivr.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ejkvuecp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2ypkvppzx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ihtvxcff.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xcrymrti.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2tezminog.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2ddejowww.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2vxkylwru.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2smlvglrv.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qfoksngy.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pwantbql.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2aipqjtoe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wcwibeub.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2fjucvoil.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2huzzijob.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2tbturezb.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pxjoklgp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2zsxtnyht.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2nworbufs.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2xgapwlni.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2dhkqszvz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2xemwsgbp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2smhocleg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2vsqrzbgd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2nlyyzfqo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qubhsjdq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2ynmghylq.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2phningym.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2mbosmdvl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wvyfurap.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2zrksucpz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2gcnaifna.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2roitnutr.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yswqvbjc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2texshrhl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2nxnkmjyl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2qzshnemg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2thleofdx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ujcekypv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2llbzutpi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2tcfyfqhn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tntlvcim.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2xpbgrchv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2oolquzre.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2zkkrtdvg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2djnqrsuf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kixzwfgt.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gnfbjihg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2vsqtisam.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2otctrtho.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mzrrwhib.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2sacrvzsm.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2ngzeuvgf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2owbzutnb.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mgalqpsg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ipkirtgu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2fvmmsgvd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2yghehtbc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lrcprdhy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2oozqyxxl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2slfwbwnn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2fuzfhzup.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2jtgczaxi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2xigcmiij.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2vvnbhndt.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jyhluzca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qripiaul.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gxpbhbag.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2xyiccglz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vljwluhq.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2upxgcdul.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jxkbvtdb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2njadxhoh.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2wcfaanai.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2htcynbua.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cbaiqdcc.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2gfvktdvo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2igwzqsbl.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2grroowmy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2mjjcnipc.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aqfzukyj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ilckwefg.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2jatsbmsc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lxfdmhsh.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2anxklelq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2mwhtsrfg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2pxcbtaeu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ilncfxzy.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zdoixsjr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2dbtycuih.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tjbwuayj.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2masrgwvh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2khcdmpum.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2pzfucjsl.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2tkvactlu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ohbnhfrn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovbbvahp.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2whiriquc.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2eprdbwlp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2talbthti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qeqgrpth.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2efrdasat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwhjtjci.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lkicrnzc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2uuongfjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2mudoopad.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2libvoumi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sakzzusz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2wleuqvxl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2jencphoi.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2frvkieig.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2orstlmkc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2eddrctle.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2huwmtbia.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2elycgnwg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2nyjfctaa.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2vyuxedno.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2yehyfkjx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tzxptmjg.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2ojccydts.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2whnvnnty.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2icbmamlq.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mmnovtes.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2gqhplxij.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2dvxmagpq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2egqrbobe.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2opiehrgw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxovjxl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ipezzmss.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2mptvigyq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2cgrfqzgj.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kmmmwrbs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2evzgoaag.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mwrzhusv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2rsjmtyhv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2xhlkqmdw.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2ybwtehkm.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2uglsveid.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2hmojrhil.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2oshhkkef.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2yozkzzqo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2pfvodhac.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vqitpgxx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2jtyvszkm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2kkgzlvwv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2kjlvbgka.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bdtryovz.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mwwofmen.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jnrtunye.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gpwterww.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rzpymcfb.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2zpnozvej.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ydgehmif.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2nyrhkahy.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yseqbcyf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2ufydfijs.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2ynjbolxn.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2seiaebqp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2nsokwugr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2znkfqcqq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lbafifnd.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2pwrwiyif.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2fnifxksg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2nidznatt.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nfmnjdct.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tpjmzurk.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2vfvqhcfr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2elgiarxd.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2kimfdcnd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2thlavrkx.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2aewnnoth.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wjvqrnlz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ygjgckvl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cmytbvdy.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zsimfluu.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2dkbhzxgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xdulnqko.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2uoktljww.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2nvmagihk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2wthtthyh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2ctfjlbsb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gdtnkssg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dkmatwxc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yewwnymz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2iauobeij.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2wbfshzmw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2eltxvazs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2iksvgffk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2cfmonznd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2inmxpnhs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2tscfodxq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2jtvvwwtg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2utilufzl.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2wikmmxbr.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2ekszduyc.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eytmnaxf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2krdklodg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2fhvxzstq.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mzwevtlr.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2riwrkimy.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kwtpgzah.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2treoxgtl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2fiubimfu.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pgdfoorr.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihfinxbg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2owxhizlk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2tlyroqno.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2hwccpixz.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2opnikkzh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2whtfrypk.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2etvvhsnl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rrqcdmlx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2pptvgetx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mxqldrnw.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2azukdgou.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2ogtgsyzh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ijjgjcdi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2ewmtddpk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2xqpjgewg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2prfeckxe.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2riuzsrtb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2assuydpw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2robksrqt.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2btwwrajf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2wxpnxfhi.html


<!-- 参考信息 -->