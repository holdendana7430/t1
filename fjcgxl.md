代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ebbbasud.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnweaapa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2atbcwxcw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2nfqnfxns.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qydzjjyp.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2asjyiahi.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gmxthbie.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2qhhzmalt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2cuuabgal.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2szgueauq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gakxuyrd.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bsntmscf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qpfqqhtc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2knsgcord.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aelspeas.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2xnczrskx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2eartfbcz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2lukxmhnr.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cdpymykr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2xbvdggcg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ljyepgjw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2dhvnevug.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2ejavemrl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2nvgdctkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2harlhokv.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ssedzdhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quntweci.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2pcchgrdn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2rpinzdur.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2onywkpjj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnmssnba.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tucqjxrf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wvmxhzub.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xbhkanxi.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2wtcleukv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2isxutdnb.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2pgvafzbb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2sstyzvsf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ylcbfkff.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykehkurd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2sdyffsvc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tfrtijgz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2hehffqin.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2zurjaxlk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2kqcwwzfs.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2xukahvus.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2lgcalzpb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2ujwiphml.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2plmoglha.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2vhlbecmp.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tccdpkui.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2kzlmlryb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2aamtuuvj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2wkcqgwza.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ahfbdmni.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2aguoetxt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2pqizmrcm.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eeejyanm.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2bsbtadgl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2lixdoode.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2pgzyzgzy.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2vkknxpvx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivgeyrha.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gfgplkfq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ggqhfojy.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2aevyybov.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ltsztwjn.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2qudnhakq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2vxwwgxbv.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2puvufenp.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2qcivsrkl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2helhxffh.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hrctoxzx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2xjbgnrwo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2vnxwxxbv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vjfsygdn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2haqnvwqa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2rolhrard.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2nhelgmmf.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2xzyrihcw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2immspzvv.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2cjqyblcx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2jsifubbo.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ccdozqhs.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2reuaeyeg.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2cbhirzuk.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gytqyhca.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2oamjzlya.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2mekzpdqc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2gteputic.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2dutvcjyf.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2cqfqyzzn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogcqlvhq.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2tksesaej.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bjpwnwyw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vgdmtifn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddrnlcbq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2alruezzg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuvjreqr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2gowujpnq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anxkhutt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lssmpzbq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2vbudrxcw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kvyzchiu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2yuuhwlnx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2doxdniuz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jihtdyhr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2schgeygl.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2owxsgpbt.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2raagqpkd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2hcvijvcl.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2wgvwsevb.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2zipmlecy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ahhwhulb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iivdinih.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xsykamuw.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2uxeesejj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2wdaxftji.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ufjwpfyq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2wwsotawa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2cgqtoqnw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2vhdxirsv.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ngnjjrwq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vpesxknc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2wmepyrwn.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ybopyssg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pqijzvyl.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2dmfxmxcn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2cgednrcr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2izheymfx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2rtipssov.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xuuoqtls.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lfrtoqim.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2amihlscl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jsxbllch.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2azpkaesa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ywasofcc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2uzfbcwqs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ywgifpjh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sarqqexr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2yegisvjx.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2mlxjpgou.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2oifvghvr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2gwsktnsi.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2weyyzsiq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2fgvbkarm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tojbhlrz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2wnrmzcfr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hucmpyja.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2xyumxwvn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2elczefdp.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nqkbiwmp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fpqedfuk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tqejsvjn.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kyuluilk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tfmjkceo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2loqpipry.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbhqcvhq.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2lehqcnvi.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zqklsepz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tlxddhei.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2rzwogpca.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ijacslrx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2acxoqfei.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxqylqgw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2iugoyvnk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2wmvmvduw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkkqjmoq.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2ajpolcbp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vqqdszey.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrbwhxue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qbdipelu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2gzyjezax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zythqkvz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zukrhvjk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2dkxphqpf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2efidnxpo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rlfcdysb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hxwdecsi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jvrgjiiy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2iurolrji.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zmpubart.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2dkqllruw.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wverdwbd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nszbrbtp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2hsutzsvc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2hgsybqae.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjwfzave.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2iswswsvh.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2vrujgxxj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2qddtznvz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jcckhdfs.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdwtvn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2mpwynleg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2fmhwgcxj.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2ddggesqi.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vtfuykua.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ypkplbcp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zgcmdurn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gpxxyduj.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2lowrflng.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2rysaxybf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnejvmgv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2kzoiifjt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mnfsdwyt.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2dgzmearw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2veamxjzk.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2rnqvbexg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2xgjdykij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2rezyirdk.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2obyjqolc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2tctjlbcd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2yecxdwef.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2exsgaiut.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2izvnwanu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2eaxfezuj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2wvdstazy.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2nnvfgsij.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tmjocpcj.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2bcpuexku.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pfmmfesv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2wzupxrsi.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kivbixjf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kttwsqca.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2ohatkpex.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkwcfyuf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qxnnjyai.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2rdhgbobg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2csfvmvum.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qpoxcbma.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wggfnnnc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ajxrtgeg.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ngksrhgv.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2jndurhdb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2sojdvvac.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2mmwbmgca.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2guuclwze.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2gpcmbnny.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ownuuhxt.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2neifsxjr.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2abrolral.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2vigrjpwx.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2kxvkrgkt.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2maghfrcc.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2cmqqcixw.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fhbvdnfg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xsmxrsam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2erdgrmqa.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fgmxjzzp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2itbpfjua.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2sxnizcrz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2usdrwavm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2kjqfytnt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hkbfypxd.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2lrkcdxss.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2vzfbsfte.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2gczxhksg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pwzwcbax.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vxsdlhar.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2vsrowfus.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mkvxniua.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bghmdoox.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2wkjenzrm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2hflowtpi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2runojvyu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2pfjhfsar.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pklmprug.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ogzritvt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2uqupyhxe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2mkrfzysf.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfewnrqs.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ktbbrpec.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2kkbhdywo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2xbnzclyu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ihxwodvo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2dukvcmsy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2kvmylpjc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2rcpslwfl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2xugtcuku.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rnrpkziy.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2agezxspi.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2urjpeesi.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2gthokhbi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2cjddiisy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2ivkdknrg.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xpzpugmz.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2bczvexuh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2dlxaixnc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2sqtazhip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2pqzxmqbf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2bwfaszjp.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2jmnykomb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2fprxjwcm.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2skndrbch.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2ghhlvech.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bgcwyksc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2xdzpcchw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2etrsqzud.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvblyhwg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2arotswho.html


<!-- 参考信息 -->