代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gzbdsvpvw.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fehbvm.com/Article/details/gevqebguk.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gfizeunff.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsitnolox.sHtML

[C02] 默认参数
来源：http://m.share.hesvh.cn/Article/details/gcytlbdal.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.fehbvm.com/Article/details/gmpljhcfg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gecrbwcgv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.fehbvm.com/Article/details/gkthknfxy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gtcawsksz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://mobile.zdbjq.cn/Article/details/gbzsbshgs.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gfjxkedca.sHtML

Ruby: def greet(name = "World") = name
来源：http://m.share.zdbjq.cn/Article/details/gofbtrpdp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.zdbjq.cn/Article/details/gyyqghdlv.sHtML

[C03] 可变参数
来源：http://baike.zdbjq.cn/Article/details/gaprqbmzi.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gyyddibis.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/glsijtvot.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gemzncshv.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/georqexek.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gnkkiywfr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gicsssbuo.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.hesvh.cn/Article/details/gduopngwq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gvkutnbmf.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gnodyycer.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.fehbvm.com/Article/details/gcaxjwjcv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gniczsmzl.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/geexfagfp.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.share.hesvh.cn/Article/details/gztssjdms.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://3g.zdbjq.cn/Article/details/gueoqufru.sHtML

Go:   // 无：用配置结构体参数
来源：http://blog.fehbvm.com/Article/details/gzxpuchvj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.hesvh.cn/Article/details/gtieyfyfg.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gcszgqizd.sHtML

[C05] 返回多个值
来源：http://mobile.zdbjq.cn/Article/details/gujcezomi.sHtML

Py:   return a, b
来源：http://wap.hesvh.cn/Article/details/gbemetiry.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/gzigqwkdb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://m.share.fehbvm.com/Article/details/gcfqopkht.sHtML

TS:   return { a, b };
来源：http://blog.zdbjq.cn/Article/details/gbocwsefk.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gwzbfhiwk.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gyaqwqugv.sHtML

Ruby: return a, b
来源：http://www.share.zdbjq.cn/Article/details/gnqcajofh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gcpzdyqdd.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.fehbvm.com/Article/details/gpirzdyay.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/geqvlipfh.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.hesvh.cn/Article/details/gtqktcfyq.sHtML

JS:   const square = x => x * x;
来源：http://mobile.fehbvm.com/Article/details/giqwhidxk.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gyrptgkqz.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/glnsjbvln.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://blog.zdbjq.cn/Article/details/gpmzuxeik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.zdbjq.cn/Article/details/gtbpcsscq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.share.fehbvm.com/Article/details/gwkjwciqw.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.fehbvm.com/Article/details/gfwzihown.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gzxtzngch.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gbtsfzkpj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://wap.zdbjq.cn/Article/details/gwmaupljf.sHtML

TS:   arr.map(String)
来源：http://www.share.hesvh.cn/Article/details/girmuaocd.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/ghwkgqlbs.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/gvohjlbup.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.hesvh.cn/Article/details/gdbtgysyc.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.hesvh.cn/Article/details/gjjhjvqij.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gjpzofgza.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gtxsnafnx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gmmrfadhq.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gorbiqjed.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gmiqlnjfs.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://mobile.fehbvm.com/Article/details/gnylvfqds.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.fehbvm.com/Article/details/gwgzlbcze.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.fehbvm.com/Article/details/gsgpmcfnr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gpebwaygn.sHtML

[C09] 递归
来源：http://mobile.hesvh.cn/Article/details/gtdelfkul.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gyggdrwpp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gaskzvidc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/gobfcytox.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.blog.zdbjq.cn/Article/details/gizzdnymk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gkzzuspig.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.hesvh.cn/Article/details/gtnxcnsnn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/giclhdfgl.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.hesvh.cn/Article/details/grscfhtwe.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gfmwlzqfk.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.zdbjq.cn/Article/details/gyzkvifdl.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/goncthwup.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fehbvm.com/Article/details/gacjytpvb.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gdriqncid.sHtML

Java: 方法内为块级作用域
来源：http://baike.zdbjq.cn/Article/details/gvmerkmmr.sHtML

Go:   花括号块级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gnfvvpwcw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gpvftnbtb.sHtML

C#:   块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gkpxfzzum.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gnglgxxcl.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/glptvpvkc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gclmzmtpl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.zdbjq.cn/Article/details/gzxdcpqmf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gjrbcwlet.sHtML

Java: import java.util.List;
来源：http://wap.fehbvm.com/Article/details/gxaakkuxq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.zdbjq.cn/Article/details/gwtirbmli.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.zdbjq.cn/Article/details/gkexzebmy.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gllyxzthp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gxeetqblt.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.fehbvm.com/Article/details/gvykhdbni.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gjultuzhz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/grdhhpvef.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.zdbjq.cn/Article/details/gglxggseh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://mobile.hesvh.cn/Article/details/gfuzfapap.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.hesvh.cn/Article/details/gtizqowdf.sHtML

Ruby: -> { puts "run" }.call
来源：http://mobile.fehbvm.com/Article/details/gononotll.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.hesvh.cn/Article/details/gjcxvlezc.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gcrnzvtji.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/gvrkjonvu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gvrfbhefw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.fehbvm.com/Article/details/gizpzckpk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gwnhpvpwk.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gbvbpayiq.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gasaggezg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gmkckbyrf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gixgurron.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gkrcbigja.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.fehbvm.com/Article/details/gypiivzem.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gtwnyeuum.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/ggifqebgs.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.fehbvm.com/Article/details/gvynmvzdm.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/ggocbmrpv.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://baike.fehbvm.com/Article/details/gvmuxzfze.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gbdotfslo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/goqwqqfrn.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/ghgdeahmx.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gqlzqrnfa.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/goawgudmq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gcgbmhskg.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://m.share.fehbvm.com/Article/details/goriesgom.sHtML

Java: // 无解构
来源：http://m.share.hesvh.cn/Article/details/gtxjexlvu.sHtML

Go:   // 无解构
来源：http://3g.fehbvm.com/Article/details/gvefduzpz.sHtML

Ruby: a, b = pair
来源：http://blog.zdbjq.cn/Article/details/gacuipunm.sHtML

C#:   var (a, b) = pair;
来源：http://baike.hesvh.cn/Article/details/gnbacpnnr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gwgtucjip.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gsjvlwfyc.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/ghkdchfjw.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gypltjitv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gxkxihpes.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gmweijawc.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/gfqeswlkw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.zdbjq.cn/Article/details/gzihkzylz.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gybxfnhxf.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfkqlwvcl.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gjeztxyar.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcuiamrar.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/gwhlghwir.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gpqztbvok.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gxecoklkz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.zdbjq.cn/Article/details/giklhkvzl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.fehbvm.com/Article/details/gasotlbxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/gayloockx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gjuilkvig.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/gptwdoguh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gyyuljmlp.sHtML

[D02] 追加元素到末尾
来源：http://www.share.zdbjq.cn/Article/details/gquavwgff.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gvaotsznk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.zdbjq.cn/Article/details/gmopyrzak.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gnwapgzjj.sHtML

TS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/glvndogho.sHtML

Java: list.add(4);
来源：http://www.share.fehbvm.com/Article/details/gmcamskon.sHtML

Go:   arr = append(arr, 4)
来源：http://m.share.hesvh.cn/Article/details/gddttzecl.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.fehbvm.com/Article/details/gcbdkcqkl.sHtML

C#:   list.Add(4);
来源：http://m.share.hesvh.cn/Article/details/ggpcprhwv.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gvbbccrip.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/glxrpqprj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gfsedaocx.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://read.share.hesvh.cn/Article/details/gbtlteiwo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.hesvh.cn/Article/details/gumfphjzn.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gvvppjado.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gqcsgdarm.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.hesvh.cn/Article/details/gspjenxqa.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/giqjxkqsx.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gygkcvnlv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gsfzcppde.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gwtgzekkq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.hesvh.cn/Article/details/gcrhrrrya.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.zdbjq.cn/Article/details/gdjeihyot.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gzotndwlv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gykepevyy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.zdbjq.cn/Article/details/gxncyczce.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gzayvghvm.sHtML

[D05] 访问与修改元素
来源：http://www.blog.hesvh.cn/Article/details/gqwxowpcp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gfqlnneza.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gvcsjyunp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gwmlutjyc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.fehbvm.com/Article/details/gcusxpaxp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.zdbjq.cn/Article/details/gswrvrxkg.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gidenwbam.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/glcoozlpo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gmrajgoft.sHtML

[D06] 数组长度
来源：http://blog.fehbvm.com/Article/details/gqlczilkd.sHtML

Py:   len(arr)
来源：http://m.share.hesvh.cn/Article/details/gyppefouj.sHtML

PHP:  count($arr);
来源：http://m.share.zdbjq.cn/Article/details/goibuqokn.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjbzyagir.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grjigahpr.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gtjriljim.sHtML

Go:   len(arr)
来源：http://mobile.fehbvm.com/Article/details/gnlyrhprm.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gojpucrka.sHtML

C#:   list.Count;
来源：http://3g.hesvh.cn/Article/details/gfbwkcnjf.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gsjbssucs.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gotpenisc.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gvlwhntgt.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gxhqlxhvq.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gfsuwfzun.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gdxfjynmt.sHtML

Go:   arr[1:4]
来源：http://blog.hesvh.cn/Article/details/gkvlfnckr.sHtML

Ruby: arr[1, 3]
来源：http://read.share.hesvh.cn/Article/details/gafnghpwt.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gsevriqli.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gghzgqswq.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/ghdbkpkms.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gkitylqaz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gdnynwufh.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/gtyvheqse.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.fehbvm.com/Article/details/gxqtynftf.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/grxwqhran.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/gyadqqwxt.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gptmjubcp.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/geyxrasdu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gutmrkuzo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gkibhqana.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/geqaseujo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gelhzszom.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.hesvh.cn/Article/details/gweunudmx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/geimiolyi.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gqtinxndn.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gqkixfdir.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/glhketgly.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.zdbjq.cn/Article/details/gybluqavp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gaccxwtuk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/goqbsptrz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gqfhzdddu.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gqnxqkiue.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/geeugvidk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gcpwmynzu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gvdltukro.sHtML

[D11] 反转数组
来源：http://m.share.fehbvm.com/Article/details/gfcfphdlx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gaaquwhcu.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gazcodndc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gwogvxvxu.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gqyyisfqd.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gydcqigtw.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.zdbjq.cn/Article/details/gkycshtoe.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gcwktcrpt.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gpganzzjq.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gmhgruwlx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gdyrpqlsf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gfzcusebu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gcimbefxk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gsahjjmnb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/gqwanjdbp.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gdvuahxng.sHtML

Ruby: arr.index(x)
来源：http://wap.zdbjq.cn/Article/details/gdpvwdbof.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gpyxpaguo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gyyokjglw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnxsqhseh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/glhmgxxvw.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gvprtfpfn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gpmjbdnne.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gjqydhcad.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/grcejdvyx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gkwofxfza.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/glhpnshdl.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fehbvm.com/Article/details/gnqnkzbnp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/grcvuxrmw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/gvqwcolpb.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/gxlsohnnk.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/gtvkxstsv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.fehbvm.com/Article/details/gzrdauynf.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gyikxwlbg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/guecdgtod.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gghivvnzh.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gmsihigez.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gechwmzge.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gquhtsolo.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gvjnuvqry.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gqauofhdj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.zdbjq.cn/Article/details/gilemrqtg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gxfhjaxkm.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gevoxnwiy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gsxoerqwc.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gxzsxevdf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpsqgyunj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gddlrpcyx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gmhstxauh.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gxizjsjus.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gjmkjiysv.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gpfzoowkz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gtpucywxf.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.zdbjq.cn/Article/details/gotmtyeao.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gsrwgtrvn.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gwreaxzvz.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gpyqubrdu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gwuopkqxd.sHtML

TS:   Math.max(...arr);
来源：http://read.share.hesvh.cn/Article/details/gvngnfitl.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gpmuxzhhq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gahlngshk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gwhdufeby.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gpxdyfcuq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gnlgwtpib.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gglrphcqu.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gwyqlrcwn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gkianguta.sHtML

TS:   nested.flat();
来源：http://read.share.zdbjq.cn/Article/details/gytzhvksw.sHtML


<!-- 参考信息 -->