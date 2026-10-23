代发 wailian999

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3onezegfy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3tsmheole.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lxqekqtl.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3toelvneo.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tcudxbpw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3zusocgec.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3rxymkqkq.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3tmoagiac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zevyljzd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eeszpxbl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfhstbsf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3lgkxatmo.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3jfxmfbmq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckafoxpl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhyqrfsq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3efectmrp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3frgitqjh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3tnjszxad.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3qnfcumjz.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iewmdqht.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3itchjjnp.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3aexdgzub.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3yafkvivh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3omdkpmcn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3imxlqzal.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3mykkzxyx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gzvjnvtm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3hjkfqwzt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3cjodvava.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3uebuwhzo.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3atqojthc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3mahtcwie.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3bnzqditf.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ttunwxow.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3sbcvczgl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qjqxjisa.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uotmrqgj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ifqlmhkn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3fgxzgwef.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3qshtiyvo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3egpfpfki.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ywcepaxu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xwzmfxej.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3xumnnlnz.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3diuaffil.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gjdwxeaf.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3rxezhbnc.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nctshssi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qrbksvby.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gzwzvjmq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bffhqvdv.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ghvbgiil.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hodckymh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3zedopayr.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3dfpnxblm.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3bytzqlbj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3sowhvpnw.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3kbwtmmgt.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3vobelopc.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3onrgcndb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3zmlrqxhu.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kjhxjxth.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3absvqikw.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3anmjimfa.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3gzipympr.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3yhucbfjl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3mqgcodnq.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3odnesmsd.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3obmkrklm.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3vcytxnyl.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ukciwdua.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3pzakgieb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3rwflauit.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3hupxuhsc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ejwycwyc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vuphbqoj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjzgyxha.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3mqaxhjhg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ficewrsq.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rxjntzub.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3fjwleifm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yzsbphym.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3iszvjkna.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mjmgojal.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3talxnwum.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqzyuxxf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3oihhwtaj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ewganoex.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3huhymydm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lvghbaos.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ovolgsbv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3impxhilk.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oevlxfot.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ejrchljk.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3fuacfait.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3kwnbhzyx.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3nanyzwuu.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3hriuquxg.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fgkvoupb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wzzrqnvq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kugeletb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3pslsyqxk.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3heqiaehx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dzqvijuz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3vmrsgbsr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3vzkwlkap.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3xtioeqtp.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3febfvdew.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3qqaivpop.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3sllwghdr.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3pojmonwb.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ghoelhax.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3koakbvym.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xuevbuac.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jhlbhfdy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3tgnqqvpx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3pbusogiu.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3uragszhx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3owbwerbj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3mleelegk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3mhskines.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3znqbhftn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3orqmhpwh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzmiswjp.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3pltaceav.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3wffjquss.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ikjrscha.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3szscxrwt.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3jmilmjxi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ffowmauo.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hzhwbyrz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wuzzgfio.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3agelfzba.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mutmjqzr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ostwyfxe.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3gcukdjqa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lqamancb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3esnvtlhr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3pevnokld.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3esvkzyub.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3vjnzdjrt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3prxbcyix.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3acbyknbd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xhqkhslf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3ozhwqkho.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lkkxoafb.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wzsumxly.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xulqiyxu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3cmytfgvn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3znulsoto.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3hiaogpue.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3gfuimooo.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xypmrsvl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mfxmvsie.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecjbkclq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iguxcckk.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tbjbeail.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzsvkxex.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cseoxllf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3eremfgii.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3giyblvkg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3hybwpnhv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3sasghiuw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3nufibbnf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ixedpybc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3fshhjcvn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3efwxnkno.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3dxsfoifg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3rvrteeip.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ljdypnix.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kgvosdwk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3znlcvszx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3eldxmwjg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3nffpgnvs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3eftfaliv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3jigvmqta.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3byrgzrwy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zqbqstuv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3htpoevzf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3ibwxqmwg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pcitbtii.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3yyewqxeu.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3qorjmsns.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zlllwesf.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zxmqdnqe.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3yutfbyef.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qmivlubn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ktumiogq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ccaadzrq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jlttlske.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3owbkefyi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3muqafftv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ascachoe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ymkgwwly.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ortnsdqt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ieaojtif.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3plsmiugj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mrrlhhcz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3skbheqmc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lgsjhzzv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3zhczxuhh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3txtnbsyx.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zqgihfdv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fyiemeex.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3iluigqcm.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhfrlwgu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bbcthyiy.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zezlhfct.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3lbwrtsjd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3plouyauq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zdfhawuo.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3pniwdlbq.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3fpkugtug.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ybhtbpao.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yjevvqes.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3sfddblja.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fdzuciat.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ydsfmnoh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3apfmpifd.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hdnezhqn.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3antrxlvi.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3mowwdcxn.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3rgyggyye.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3cubkcclr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pyqrzyup.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tkxvjfgq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3upxkawpc.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjkdshh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3zlloahqu.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3hpcdhkli.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3igalznkp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3zmjknsxq.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnwnctlb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aseretxb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dnvipckh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3fjeqnpbc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mpurktda.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3emrvkyel.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3hbukgxdu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3movuzbby.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xcuvsxaj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xotgjszp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qetameso.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3keswuipp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3aexvhnhe.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gvbdhomc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ypfwxlmf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xbtlltfl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wthcdgaa.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3jvmmzzcw.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywzbnyxj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vccectig.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hvqjhxlt.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lwhzhfpq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nyysjwdg.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lzadsvle.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3townhend.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3elgznkmm.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zglvqcmf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jcslorbc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fmslpuqj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmurwqja.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xavvdufs.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxmyhjh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3tebvdjwb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nzxglmym.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vsvxkvsa.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3iugerkbe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3hdgqpxib.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jhuwzavv.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3htldavuv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3opvkdmrs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3rxiidfql.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3txchednb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uebnqqky.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3uciusvln.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cemwbqge.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3veymhlot.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3urcgfcrd.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3imnzuprl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuiiprhb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mabcnjxl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vjvnxtmi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uebbxcbl.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3oepivnlj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3blwugxjf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3dqwrbpdi.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ylseidgg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fcbvxfvg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3uxrwedtm.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3yxzwjudl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3upqdwrzm.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vjdvxzvf.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3bdsxjblm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3kyrnmezn.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vvgbzhbi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jbmkacvr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jnkuxssp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3wzezxfdd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3mlnzqgqm.html


<!-- 参考信息 -->