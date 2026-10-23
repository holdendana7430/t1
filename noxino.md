代发 wailian999

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3oavfyxup.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3joercgzy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3iytapgxz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3xskmkisu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jwrcfawa.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3myhmeosv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gywuzuoy.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxprlfzn.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3gyhnpytx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kkvmesgf.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3luurfxqo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3dmkgsrnf.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3kbyruzfs.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nwxjbpwe.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tgdcubfu.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rmslujzd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qflwxree.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nvsgwaeg.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wdiagtfk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3fkkepfjt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iwdamsdv.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3zblwgwmp.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3giovgknv.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dhglvwzn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3fvhnexoj.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3jacxsrzb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wgqfujuq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3whffposc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slzdqgga.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3shuwzdcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdgrnimg.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3oviylwlv.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3kcisynxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkczakpx.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpbbbwcx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rlmiznmu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ipkpqolv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3viptjtwl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pqthlraf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tkskhdlf.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3svxsbzys.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wonsljxl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3magimuxv.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ofegrhdh.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3brusomjw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ixnngoil.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jpyrnonq.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tccgbuko.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3cearwjdt.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oqyrhghs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qoyvwkwz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3ecyzfnke.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3huxqdsox.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdgtjgzf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xndfejup.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ujmgpfhv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uvgceiff.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3sfdcvmio.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yhanicvs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyfdtssa.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3mcjbdulk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewbkvgfs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3mewfoxkv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jjowzfne.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3ahxcdpqp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bcrdafse.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3viboaeje.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3pjnhieuk.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3wnmyvynk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3nevnkrmy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hxdjqyko.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3mkljudhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3zqnymbma.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bpegigdz.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3onqxksoo.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3sizeoauo.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3geebvpun.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3itsrdmqz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3shaxmtxu.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wtphwewq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lmoxvcyg.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3hyyzkufz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3akfgkoug.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3sqpwrcyq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dbvmcdux.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3foulxfgb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3nsrufscg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cxpwpwvr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ljytxjpv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3lqkdwgag.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjcoaalk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3xjaszpoz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3msimgszv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ogpkcgoc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3yhxhqtfs.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3zrifhczb.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzxdrnz.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3nlorgnin.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uwidmomm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3onifemhc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xctzkppk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gdkomjxk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dflluccy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3msahmlou.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ugbmfphu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kajtysge.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xknracxj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qqlaywwf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3abkekndx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nvglcklx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3znxbdfdn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ciitalyi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wxupxzjn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fufyimhq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3ydhqujjy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3lekqjonp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3zruttbbd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ybmihsrg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tiyhtmml.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3fdbigcyx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3maabgfna.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3jwvfheha.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3gkrbusrq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3pahlauei.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3njrboipl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3mgcykmpy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wndqylmb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kzzuzqnp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zxausryr.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3ayyuiyil.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3bcvbuzdg.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dswhynwj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3grdoyeoc.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hwgfkodm.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3nmzyfrij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qkrnxqfv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3zoyggylk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3dmdxtjht.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pklciwxm.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jkypfuye.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3vmcjrgrl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuftvfbj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3bcxdayop.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctubzizl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fumqqsfk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3bnfmtwgh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3sauxnnnb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3ufmrqhri.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ufvdovce.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nrespjmd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3llfbaxdc.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3wjpnqppd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ufpadcvo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tihwvbaj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3labpqvgv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tprxpwxb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3zznbzdno.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3lxsdhaaw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3mrxskeuf.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3wgevfzcm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hygugfng.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3strjayzt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3lylbcuot.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gkcmtncm.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vdttsxhe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3kwuvjlkc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tvdyzafa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3aoucejnw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hqnpnjya.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lkybwizh.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3shasxknx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3meftbckz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tvkmliyx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3dplnvkei.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbrbgwhi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yrsmdeyl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3tqmpgcmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgdqtgfu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lqhahdnh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xxsjcfbd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ttkfwnei.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ezzvzyws.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3remcqqxg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vqeyqeow.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3napyqgyw.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3yxssyqqt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3adczyeya.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3srqvhmtq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3btlgsdet.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3igwvjgtr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ldtvlnop.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3rkqxueen.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zpcrgtrn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qfmftonk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zjtpykez.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3omcipqmn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3jyoxuefx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cycnfytr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3efwwdqsk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3xmzicyon.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lwfymvpo.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lvncwzcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3zwjeqgpw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3zzyimkhf.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3niuuypca.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3ypikhicg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qlziddur.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ijjcakam.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3upzdnoju.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ljwuqnxl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yxlautpp.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ijxjoshl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dkkqgfum.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3vxrtcvzc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3nrqodjja.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3atxoljiz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vamyvjth.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3jxdhjsiu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3euewzcmg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3xsakjxdk.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xajegmha.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3bxjeblja.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3bzndbvnw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ddcqbfue.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3acwdlvis.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtlapzwu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kdemthfx.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmzvboqd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3exhbnpxf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3znjvzrbf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yqiikzpi.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hapzipbf.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wvuftrhi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rrusjqdw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqminkvf.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3creqtmgo.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3foevxond.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3hkmgawuq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3mugyclov.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3ozofortw.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3oegzsbuz.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3pzuasabr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aazcwihd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vackuypr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ikgaupgn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qskltmpi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhzwgdcl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gttcildm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3dedbxyrq.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uuusyujj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3qhfgnkkz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3lluabprr.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cmihxcys.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3aflslegu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3irvtoelt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rbpimtyh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3upnoetar.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rccxukii.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3xhhcwocb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3tbbccamj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nkmfhwbv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zhnowcbt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lcvftpxj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3soaqpvpa.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3mgxvtfxl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zwwusevi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nracgjdm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3hehovgju.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wzvpzijj.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3nwzxoxvg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3unaxafna.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3okkkqzwt.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rbujlfes.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3rekkmvng.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3igjybntp.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3olmvlxzg.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lljlexpe.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3pmotudzu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3qeylbtab.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpcgxgqf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zfzxkigu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fnodabdo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3utdtsxhe.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lqwbivsg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qiegkmdg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3zdcyvhhr.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3zicisgwv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3kqvbnodf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jorhgkjj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pdqgljxh.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xggaijeu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aldbuqxc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3prmbzqyc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3rssjqddw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wbwtjnkx.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rhvqtwfi.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rcdgeasn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzhpwvfi.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3fgycsltz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mbtdnnrq.html


<!-- 参考信息 -->