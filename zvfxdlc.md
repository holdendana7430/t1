代发 wailian999

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gpplvoltc.sHtML

Go:   if data == nil { return }
来源：http://baike.fehbvm.com/Article/details/gxsxheosk.sHtML

Ruby: return if data.nil?
来源：http://www.share.fehbvm.com/Article/details/gdnagkipm.sHtML

C#:   if (data == null) return;
来源：http://m.share.hesvh.cn/Article/details/gxuxhovoe.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gbdeaiuaj.sHtML

C. 函数与作用域
来源：http://baike.hesvh.cn/Article/details/gktfkyevq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gafyoblbj.sHtML

[C01] 定义函数
来源：http://blog.hesvh.cn/Article/details/gyreumqus.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gbbyomvmp.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gvdjwuwan.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ginmihxpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gjbulwusq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gafqkrytq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.blog.hesvh.cn/Article/details/gkadahmin.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/gjntovbay.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gxnjupijh.sHtML

[C02] 默认参数
来源：http://m.share.fehbvm.com/Article/details/gydpubhgp.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.zdbjq.cn/Article/details/gfvyyfjxg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/ghbxxhoho.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkxsnkzbh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.hesvh.cn/Article/details/grtqgyqxw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.zdbjq.cn/Article/details/gmyrgscfw.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.hesvh.cn/Article/details/grkiyvmnk.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gkjczxvcg.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gbqzkvbgc.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gjdebljay.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.fehbvm.com/Article/details/gertmrell.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gikysjftw.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gykzzelvs.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.zdbjq.cn/Article/details/gurdctqyt.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://blog.zdbjq.cn/Article/details/ghfkwqqzt.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://mobile.hesvh.cn/Article/details/ghvmhtpfs.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gqqaonlhj.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://3g.fehbvm.com/Article/details/ghuhzsqum.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.hesvh.cn/Article/details/griffbwcp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gaybrjlze.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/gssqokljy.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gnplddyqw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.hesvh.cn/Article/details/gdkyhcnug.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gnsnlvcys.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.hesvh.cn/Article/details/gpirphbfc.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gkaclqtex.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.share.zdbjq.cn/Article/details/gengmokqq.sHtML

[C05] 返回多个值
来源：http://www.share.zdbjq.cn/Article/details/gjbgtkcvz.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/guqyhkldq.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/ggaefqhiz.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.zdbjq.cn/Article/details/gbmbjsver.sHtML

TS:   return { a, b };
来源：http://www.m.share.fehbvm.com/Article/details/gbjhjknpg.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://read.share.hesvh.cn/Article/details/ggumgqszx.sHtML

Go:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gbvfruzne.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gqbaxnwjk.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gefjapkgk.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.hesvh.cn/Article/details/gqrxmudsj.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.hesvh.cn/Article/details/gwuwrupno.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gtjqxwczd.sHtML

JS:   const square = x => x * x;
来源：http://baike.zdbjq.cn/Article/details/grsdjwctw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.fehbvm.com/Article/details/gtfvgluah.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gpucsyciy.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/guysquioe.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.hesvh.cn/Article/details/gwzgxqjpi.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.zdbjq.cn/Article/details/gbtpdsmrw.sHtML

[C07] 把函数作为参数传入
来源：http://www.m.share.hesvh.cn/Article/details/gpjirzrpp.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.fehbvm.com/Article/details/ghjbrzvvn.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/giwplbfyk.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.hesvh.cn/Article/details/gjytwjznb.sHtML

TS:   arr.map(String)
来源：http://3g.zdbjq.cn/Article/details/gdwmhgjpc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gscatwpcm.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/ggrzzepil.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gevoousnn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://3g.fehbvm.com/Article/details/ggnjgtdnl.sHtML

[C08] 闭包
来源：http://read.share.zdbjq.cn/Article/details/gpgftntyo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/gnuufsxmb.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gwzvydymr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gozqigolc.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/gzxcnumkr.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gjrasggen.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.zdbjq.cn/Article/details/gmlwbpbnq.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/ggchtzllr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.zdbjq.cn/Article/details/grthrsbvg.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gzdftglca.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyxjkgdoe.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gzldqjsnt.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.hesvh.cn/Article/details/gvsscqfur.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.zdbjq.cn/Article/details/gpihumtqo.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://baike.hesvh.cn/Article/details/ggyoyuapd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.zdbjq.cn/Article/details/gqjjweoxx.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/geylwrxfz.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fehbvm.com/Article/details/gyftmvyxv.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gcejapuiu.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.zdbjq.cn/Article/details/gbjrusdcs.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.fehbvm.com/Article/details/gvwdlmujl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.fehbvm.com/Article/details/gqpsjifyz.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/glbnxsjxv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/ggemnnfja.sHtML

Go:   花括号块级作用域
来源：http://www.share.hesvh.cn/Article/details/gxdfbabim.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.blog.hesvh.cn/Article/details/gvabymavc.sHtML

C#:   块级作用域
来源：http://www.share.fehbvm.com/Article/details/gjyyohjeg.sHtML

[C11] 模块导入与导出
来源：http://mobile.fehbvm.com/Article/details/gnfdudtrt.sHtML

Py:   from module import func
来源：http://blog.fehbvm.com/Article/details/gbpuqejwn.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gaoxbpodd.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.zdbjq.cn/Article/details/gaongrlfi.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gfmqiulli.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/grznpwrle.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.hesvh.cn/Article/details/ggducfugw.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://blog.zdbjq.cn/Article/details/gjlcktbee.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gxketmfkm.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gzwjqobvi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/geafuzkrn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.hesvh.cn/Article/details/gkalmxhfn.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/grilidlcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gnhzyanml.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.hesvh.cn/Article/details/gqqenfkve.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gnfqpjmrn.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.fehbvm.com/Article/details/gipfylhcd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gftveluhe.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fehbvm.com/Article/details/grnkhgewr.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gwalzjeus.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gizffodps.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/guxhqiifo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gwohyczbr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gvntfxgkc.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gojwvjdor.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fehbvm.com/Article/details/gljxtducw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.hesvh.cn/Article/details/gylvpyvbt.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gjsmjnvjv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gecymfnfh.sHtML

PHP:  // 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbdzhalaq.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gpxewhnhm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.hesvh.cn/Article/details/gphaujwxd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.fehbvm.com/Article/details/ghbjiielp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gkeahrwgn.sHtML

Ruby: # 无泛型
来源：http://baike.hesvh.cn/Article/details/gsfmepfgv.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fehbvm.com/Article/details/gbaykrqyd.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.hesvh.cn/Article/details/gkffhwaak.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gqddlnspv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.fehbvm.com/Article/details/gasjrgqqx.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gbwpxzcce.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.zdbjq.cn/Article/details/glisautrd.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gkbixwzzk.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gfgvqzacn.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gfkggynzd.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.zdbjq.cn/Article/details/gscggmbmw.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gllkoovux.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.zdbjq.cn/Article/details/gjtwfotiu.sHtML

PHP:  // 无重载
来源：http://www.blog.fehbvm.com/Article/details/gmoixpred.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fehbvm.com/Article/details/gkccsopue.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/gpoljdkav.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.fehbvm.com/Article/details/gpubjuywj.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.fehbvm.com/Article/details/gcdrtnbyw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.fehbvm.com/Article/details/gnuhuwxdk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.hesvh.cn/Article/details/gpsvjjiia.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grlrbxcfl.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gbaonganz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gotatcvwx.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fehbvm.com/Article/details/gicsblroi.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.fehbvm.com/Article/details/gkxmhjwnl.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fehbvm.com/Article/details/gebtusopi.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gmpznwbxb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gkawcucnz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/gaaodbkny.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.hesvh.cn/Article/details/gbdjbnfer.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/ghnexjeol.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gqbkkotsp.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/ggptgkurz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.fehbvm.com/Article/details/gybdoumoe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/gtxdjfxql.sHtML

JS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/grxwjizrz.sHtML

TS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gxjyzffhb.sHtML

Java: list.add(4);
来源：http://wap.hesvh.cn/Article/details/gdceifzak.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gyrkrknkv.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/ggzqdoxpe.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/gdvsfxawr.sHtML

[D03] 在指定位置插入元素
来源：http://blog.hesvh.cn/Article/details/gmcjnrkvd.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gkavovqgo.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gxpdxpmpk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gdvdepkge.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.zdbjq.cn/Article/details/geaolhlrk.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gpqycezob.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/gsoovniqh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gghwgpvyz.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.hesvh.cn/Article/details/gdupfkumr.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gdweddvde.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gvgtomsra.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gczlekxjb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gnnvupnnu.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gtxxmurof.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gfpbnhmvv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.zdbjq.cn/Article/details/gscxvpqmx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gshbobujd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.hesvh.cn/Article/details/gpyqharyy.sHtML

[D05] 访问与修改元素
来源：http://wap.fehbvm.com/Article/details/gczwjisxe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gqvgqkjil.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gxfruvtwd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ggnhohtsv.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gcendgjio.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.zdbjq.cn/Article/details/gsornslsg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gfjecqnzi.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/geaimoyen.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/ghttyvnmq.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gvflnoqug.sHtML

Py:   len(arr)
来源：http://www.share.hesvh.cn/Article/details/gaxrridol.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gjsqbyhwy.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/gikvhhkzk.sHtML

TS:   arr.length
来源：http://www.share.zdbjq.cn/Article/details/gyvznpjmv.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/guiedqrpn.sHtML

Go:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gukpkctah.sHtML

Ruby: arr.length; arr.size
来源：http://blog.hesvh.cn/Article/details/gsivcbbyx.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gxxaymifs.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.zdbjq.cn/Article/details/gjfktasre.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/gxknotzyk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gapdelqap.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gableztwz.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gnaqknhdb.sHtML

Java: list.subList(1, 4);
来源：http://mobile.fehbvm.com/Article/details/grjiamoss.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/geugzgiko.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/gnsaoxxbp.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gihymvkgi.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gfdymcgch.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.zdbjq.cn/Article/details/gtqlrxnsh.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gqqsptqjq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/gapudxxfj.sHtML

TS:   [...a, ...b];
来源：http://read.share.hesvh.cn/Article/details/gtwzfrmsv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gzvpebyic.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gbfmwumwg.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gghfwphpa.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gduwgtows.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gfnjqtmxm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gwobwjtzx.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/geglifzwx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.zdbjq.cn/Article/details/gnulqhqvf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.zdbjq.cn/Article/details/ggdrggdcd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gksqirmuq.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gsakejiqh.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gnwmjoqtp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/ghaeqqbtm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/gfndfidrv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gqlfsqush.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gvpkjrfbq.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.fehbvm.com/Article/details/gbcoqiyeh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gbigwpskq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gtqvipgrz.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gfnjlyisu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.hesvh.cn/Article/details/ggyjjducz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gctrnijex.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/galsxaqgq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/ggjfucakd.sHtML

PHP:  array_reverse($arr);
来源：http://3g.hesvh.cn/Article/details/gutsfvczd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gipdxnwzc.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/ghesujsvo.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gtmocukuu.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gvrcdsbwc.sHtML

Ruby: arr.reverse
来源：http://wap.hesvh.cn/Article/details/gbupulqpb.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gmmumsysk.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gezfftiui.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gvxbenaut.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/geihhrtzy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gebfqbeir.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gsqajmwpp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.hesvh.cn/Article/details/gdozxwqzw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gskmovkhn.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gczclmnqf.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gvvfhucag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/ggvwgnfgy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wap.zdbjq.cn/Article/details/gqobecjpf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gjtxubvsy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gqmduapxl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gidlaaeur.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzngkkobd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gzjyjfqkf.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gbdxrvvqq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpogowumm.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gbwjlyqae.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/gmahwtxpq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/glypdhaif.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gjbnqytsf.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/glxluigoq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gdbvpieag.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gjpdsafhp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gyycrffuz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.zdbjq.cn/Article/details/ghwtujwvc.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjyugwdzh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gxhgypbxi.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gvkibmbit.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/galyzzknf.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gxxocgkoc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.hesvh.cn/Article/details/gypijtpve.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gosffwubg.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gqrrnpqae.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtsifgjjd.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/guwssidgk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/ggdvpvrxx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gnvkverup.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmayqjcuj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gizgoskgn.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gpljzghpy.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gzjbndmbl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/giexlpggn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gfitlvbhh.sHtML

[D17] 最大值与最小值
来源：http://3g.fehbvm.com/Article/details/gwguebmta.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gyrkamnnr.sHtML


<!-- 参考信息 -->