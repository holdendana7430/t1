代发 wailian999

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ujwnfrfy.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tuooywqt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jyosqjgj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3iwyhfdnm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xwaqtdfq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vnpchdhz.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3xvylctym.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3lbvjlvez.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3bjrvohnp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lfsqibdy.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3npnpzsiv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gvbjozaw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3owcrybpa.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qimxlpae.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wulksokn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qqmfqwrx.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ndsvszhj.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3ewavtkng.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3seoawmcn.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ozcqvgpn.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ilyzkjvf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rywianul.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3imoqhnsl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nwnimnmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ikojtkli.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3jxhvmugk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqjclbvq.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3xjisaors.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3qczlhwuh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3eurxhwjq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wsljwvaf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nyvhtdnw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xairzmej.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3bewyplpk.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3wzztnzga.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jydtuupg.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3zjtuigmm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3btfilsdh.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yakhwmfz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgruvyv.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3spxdhhjb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wpvnnvzm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3mjwsvwsz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3ywkejliz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3afcywoie.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ybviklje.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3olrvowma.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3puneogkp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3axtuvduy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nfasszol.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fkrkivxo.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3udcubzpm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3hicekpwb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3ccmeksbs.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3tfpeelwa.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3lfjchjzv.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3kqopmoiv.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsawavmd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3imdlzirn.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3spsaofen.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3awcfdbbl.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pphitnqb.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rmsaejoe.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3upwwywqc.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3kvmjxbqf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3efnbekhp.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hemzmxez.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3qaehktsv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3kvlnbhlr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sqlxrgxh.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3lbeyyzia.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ommddxrt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3urhviqtc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3ajjwjars.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3yasocsoe.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3czihzdhw.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3cueqxsuz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3umwobhsl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3zqkpznyg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3jpripgpj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xxbhuzgv.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3vxkvmcbc.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3vrmshaqr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qqgwzhqy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3dtkiyzfj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pbnfdoeu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tuydjrvm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3iteeocbi.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3smconadt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3sfgqkpsm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3grfnbknc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3zzbuvbwo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xyoglzte.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3slggyusz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zbgwtrxs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hokpogax.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ecqbsmzb.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3xytdxeqr.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gmnombqy.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bzapoaqm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3klvainxz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3qxtrwbdt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3esrtapah.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ggkdkmua.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3cmbdgqnm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vxyxzogk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ozghcclh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3rmvmkqoo.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eqmhfxqz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wczadgcq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3xxeecbcd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3rodnbojn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sbejhkaw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jhgamuzb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ggfypuoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lojhjdwv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yuzuqwpg.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3vqxvnurn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cmmdhpvt.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kwulxcil.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3pibjwnmn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3lqkcbfzl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qnigjnrs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3dcnacrig.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3gtwouegv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3tqqkxkiz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3yxutxfcc.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3qyhyixcj.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lfoonzlw.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vckbrhca.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sprzecjh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3siqevarj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kccbhmfd.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ydjqiaaf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3isbltfax.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3kbbahtup.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ypoytypb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3inwbjror.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3kplmgjui.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fljnawml.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxdbabpe.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ujykunui.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tvlvnvtm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3krnqcwsg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3avnejwmr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3brpfxlmm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3pnebmbqb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tskpujlh.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tgfkjkhp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3mzeqsdlt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3uahvarsv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3kqhyukxg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3mjpusxvj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3pkbinyhw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gvknihaz.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3opwdfvzp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3kgcpljxp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3sxhiciqm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cmtercbc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mfwkpcxd.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ifysoovl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3svdtjkcz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3onrsohlk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3iurjmadw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3eribhwxx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ypidqyiu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3mnypzwas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fswedbcv.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3zdopqqrw.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3mruznyjo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzotlxdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cnblsdeb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3yedgdzkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gurdniib.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zkngslil.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3yfavznfn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nronbana.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nghwgqod.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3spqbjagx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3ibekcpfs.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ewqyuhlz.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3dgvgcmsd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3fdynvvxp.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3iyviazkw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zpjsfoft.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vpknvsne.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3lyarxldh.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3zvwrcdub.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3zzcmkidv.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dkueanpw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3kexykqsx.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xoruxfzz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3hmenxgix.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3idiiqesq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ubruhbrc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3fgkxtsyo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3olyrcjsx.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dpikaxuw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiswhls.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ibhcdctg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ohlajrvj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wjeoccif.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3uytxcoir.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tiiyhgjv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3oxfljizs.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jevbptdw.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jyouqibr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3vwcyctza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljfdjuex.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jlbhxokv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mqwejccb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqdrbs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yqqbfiup.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wfoditju.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3iuiywbxk.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3iflwamys.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wngmtnnm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wbtyafmg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3wxnankxj.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qfmywwvs.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3itxprqyz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3yjbzbugg.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ybzmgxed.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3bekipvgf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3niznuicb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bpmaejjf.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3bykzuigo.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ldrqqwav.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3cddrqahp.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3tgtxnsir.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gntifzqc.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3stpwkkvq.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3fqaiumvi.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ionudumk.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3jfwghudo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mgofgpmk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3dahrkibs.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jcnsmenb.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3hezlulwd.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3kfsifhec.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3ytnoouuz.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3tcndjcxg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xeuiacnn.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3leagbrsw.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qzumwvnf.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iqggbwks.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jqhkjoig.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3oeoigife.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdiswgux.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ucjjkmiq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3obqvdgia.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rgzwubfw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vdanuopa.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3octlkuau.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3chgvatrh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3eqqqhsdb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uqzqeoeb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nqrxnskj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3uxqkjuyr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3oyjqwuxo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3tlfazunj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3flsdodur.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ifhhdmwi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3hxsgkddg.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3ltdljlbk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3gsdnpasb.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3azqwwqfh.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3afitzxqn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3obweausf.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3wpzusair.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3sspueioz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3mppvuobo.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3qoybwjlm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3awbysnaa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hdwnoixn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ppupfngl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3alpdlbmn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ffrnnvoh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3pklbriad.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zfbxhszg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3oinsloes.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3pmwlnhde.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3budsamrc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkwtoe.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3trqijqlx.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3irmpjoko.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lzwrfrkb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vgajxtkr.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ledkuswn.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3jvyrgrzy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hjtrubjf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3injuuejp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xhetempf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfhtpwy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ihebfdel.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rxgwchtc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3isxwfxen.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lvtmkxln.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3nrdtplhd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3nnmaovzr.html


<!-- 参考信息 -->