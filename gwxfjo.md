代发 wailian999

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2totohalo.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vfwrnneh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dtrfcnnl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2nfkfzftu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2jtodbwlc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2yerppbdm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wdwoqvfs.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2jsquhfzc.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yytpqofb.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gqzzsxxb.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2nryahcnu.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cygkjikr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccociqjk.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tnyycdqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gstxwine.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ryvdamyf.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2pyuspdll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hibkatoe.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceohkfej.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcfxebam.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vkspwpjv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2wvjftigx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkkmkgvv.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iwadnaug.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2plsuxvye.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2xyjewvyy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2blhytrra.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mplisxaq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2pyiuljqr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2szejutle.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2veavqwos.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ujgabhmx.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2limxngyp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2gzfwhljh.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2zgfxtbit.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2deewghud.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2obkwvwgn.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjqmvwg.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljontjsi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2khltqbvq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ipuudlwe.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2foujajyh.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2vehntxmj.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2dgowasok.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2eobdhfae.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rwlqiunw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2lteodxzw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kkkfhlll.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2egqfhybp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fzpzwcvk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qscbdnli.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2dcnciaxc.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2bbilgyvf.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vkcztuts.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2ievmjdem.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bgmvzlgv.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2ebvjukuz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vsfopqsa.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2fmliimci.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2krmfcydx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gqoqmsmu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2jgresphb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2wlhifeua.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fxxyhnfe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vfkdgaxy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2dykkzlna.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2iqhtfabm.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2qjdtgwcg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2pknqmeji.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2bkfylwqh.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2djrdqsmk.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ixhfahyo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwvwrzj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2zuqonrnw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2hkcshvrl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2pznvmapw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2udoiexkp.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2kfbbruec.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2lusuxyrb.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2qyiazqts.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjvlijjf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kaikzsmg.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykstriph.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wpzcibtq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2qzaptlph.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2gedzklls.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nesreapw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2znlbqeau.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fufkjrhc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qypoiygn.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2zagckeey.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2uwnbgxoo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzaostyg.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2chdmdqik.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vephyfmg.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zktnatyj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hpxhekyo.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2szkcauiw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2yuqusxxt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dssapjoi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2yowxqcyk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mdfyfrtu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hyjpcisd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2xtfpazlc.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qujbffah.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2kvothpem.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2fqolmawb.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2ccanbblg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2emyrlvps.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cmurxscy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2wmsjzpoh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwvxse.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2mfhsnzxn.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2sakolbfg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yvzqpklu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tqpzatfv.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2tshxqfxt.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2htacjnyb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2yrevsqoj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2ymxhungx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2focfxlsw.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bknyxecb.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uemvghie.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2piaivhiy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mkwkyxyx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rxtcglnm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2vrqkmcpv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxabddif.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fpechbky.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2hbassuaq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2honwtcnn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2ftkkflue.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2pjdufxpc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2scmednkd.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2nlaxuvnx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dlncsbsx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2aapiqxpo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ofvbxqmn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hlgabpra.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2jnecxevk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2yhsffdmu.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2ndeixbjl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2ogpmuvkn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ewohhcph.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2kgmdwvnn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2imewzbrd.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ftyswoot.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lhdxlwyj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jlllsauf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2cawkrvnd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2qlgokhwe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2tnsqhaxc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2molpmqzu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2wkaxxnyr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2gtosvpht.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vgnwbzaq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2mcjaboko.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhhojcze.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hiuvrzyf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ieytayqw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2zaglerxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmruncqq.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aausmhad.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2tmtgvaro.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ylmeevwl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2nggafvik.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2eakhvssg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gurqyooy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2mwtjseqj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2jdeggpgd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2keeniwny.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2uyspqdzf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2yqnukqvq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gtvqawxl.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2vqkhcbex.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zkeiholi.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2prfnulth.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2webufebs.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2zjxpcpvf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2thacxfqp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2erdbtgbp.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2nnsapxie.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ykfgqtts.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2gmczcwhw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2gupgvhym.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2huwsjzsz.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tskpxsuo.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2cjkvoanv.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pokmqqza.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2xempzeic.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2xuvuslmw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2brgjgrxm.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dfdfljfd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xuieqzwl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfmwhzo.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2wyybxpza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2euizrvnd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2ctwhajmr.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2urdmnchi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qlviuasa.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uergqaaj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2voxhmezt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2wzxlvify.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2cyaebpwj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mppsbanb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2iovkaqmw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rfkxigfz.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pkjydngg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mokyyspl.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fecrrapj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2gdeapjsa.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mwshqjjy.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2pbwqcjte.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hajsvyqj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2gpvpevtw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ppfapnyg.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2tsbjkkgz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mqaknfvl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aildgqlz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2hojxjnrs.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2spsttssa.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2jhyguqna.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2bvotbmgr.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2meodinpd.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2moluioqx.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2huhzocbs.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2njmlyrzj.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhdzzv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dsgzlikh.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ctqszjqi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2ilcyrmqh.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2xfbrahcm.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2hrzxhvhg.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2onajkimi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2zqevinwo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jmtyghib.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ihjhnvbb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rpymdnbh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2cklxxaaf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2hjgkxnwk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cyjriznu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ockdxnbk.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2woemqbpr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2ftjvazdq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2xotarntk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2zkjyppum.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tpmxrudt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2etevbexp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ogkitqbg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2oigqevbr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2vemyfbtg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2rzjdwmny.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2xukobmgt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2uwfxswig.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2irfikjpn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2nkxqydzf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2pvkaxrdp.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jbmcgmpp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2blxqilga.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vzhvnlgp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2raxyyegg.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2mfnoxier.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2prdwfbzu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2epdipfna.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2uujeuyfm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rfwcaaii.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2mdqpuwuh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfvnjonn.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cduclpwd.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2iuebjjsc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2avjkuskv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vyyuzstd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pvstvief.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kkgyrkjy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvlthzn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2scimfnkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xyyakcar.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2ihrsbxjk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dffopwvc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2pfotsaps.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2ofhqklor.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hrcwszdt.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hdktjkac.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kusvltud.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dbwfmwox.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vzixoxmk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qhnmxyfg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uzztychj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2leblruzw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2qvrzypsg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2nrjvehuc.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2jhaebmyd.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cghpxtpq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2fooaakzs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2iuctyvex.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ucssxejn.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2btbltxuw.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2aixvcqdz.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxyfutfc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vxtwobnd.html


<!-- 参考信息 -->