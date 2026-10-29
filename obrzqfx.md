代发 wailian999

Java: if (data == null) return;
来源：http://m.share.zdbjq.cn/Article/details/gtgudueyk.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/guahizgsj.sHtML

Ruby: return if data.nil?
来源：http://mobile.hesvh.cn/Article/details/gkismjufp.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/guflrymss.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbzubygrs.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gnvznqbgu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfbelfgax.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gbmgplnvl.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/gzerlfzgr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/galjbcsae.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxftvtxi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gpnbzrjyy.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gsasyqrwl.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://read.share.fehbvm.com/Article/details/goimpqtug.sHtML

Ruby: def add(a, b); a + b; end
来源：http://wap.fehbvm.com/Article/details/grmalwjhv.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/grnnimont.sHtML

[C02] 默认参数
来源：http://wap.hesvh.cn/Article/details/glfbrefkz.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gisgrkbwl.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.fehbvm.com/Article/details/gttoygkak.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gtpkespoq.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtqhvzezb.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gsslgdgfu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gfvsrudmo.sHtML

Ruby: def greet(name = "World") = name
来源：http://read.share.fehbvm.com/Article/details/gwaaxfomc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gbdqhhwdm.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gchqrhodb.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/gcblffsqo.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://read.share.fehbvm.com/Article/details/gzapnwoum.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.hesvh.cn/Article/details/geooxlzkx.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/goutpjsfz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://wap.fehbvm.com/Article/details/gjstbukas.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.hesvh.cn/Article/details/gtidfxopg.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/glarbohks.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.fehbvm.com/Article/details/gznaeffdx.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmacscg.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.share.hesvh.cn/Article/details/gsssidfqu.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gvzmxcrtx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/guwynpthd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://m.share.zdbjq.cn/Article/details/gdipvfkjn.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.hesvh.cn/Article/details/gzhxkzrjk.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fehbvm.com/Article/details/gwzqhzwtg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.fehbvm.com/Article/details/gnwlxehzy.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gbuzxnggy.sHtML

[C05] 返回多个值
来源：http://wap.zdbjq.cn/Article/details/gwssztuow.sHtML

Py:   return a, b
来源：http://3g.fehbvm.com/Article/details/gmmvuwfhl.sHtML

PHP:  return [$a, $b];
来源：http://baike.fehbvm.com/Article/details/gdkjkzttb.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gaavuhaym.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/guebolvht.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fehbvm.com/Article/details/guqtjdbmm.sHtML

Go:   return a, b
来源：http://read.share.zdbjq.cn/Article/details/gmteyrsji.sHtML

Ruby: return a, b
来源：http://mobile.zdbjq.cn/Article/details/gihhobwwh.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://wap.hesvh.cn/Article/details/gsfxzszka.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.zdbjq.cn/Article/details/gyrwmnvwv.sHtML

Py:   square = lambda x: x * x
来源：http://wap.hesvh.cn/Article/details/gmccbzxak.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.zdbjq.cn/Article/details/ginnebyku.sHtML

JS:   const square = x => x * x;
来源：http://baike.fehbvm.com/Article/details/gsuavvgmd.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gqeulxatn.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.fehbvm.com/Article/details/glbathdyd.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/gglhkcfls.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/ggeexgafq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gvtwncyrg.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.fehbvm.com/Article/details/glmjldswy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://3g.hesvh.cn/Article/details/guktidlgy.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghlabvfod.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.zdbjq.cn/Article/details/gxrtijzrh.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gitsckskl.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.zdbjq.cn/Article/details/gigxgddks.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/genvkdxvd.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gkpnspgmr.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gatbmpqlo.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gnmdotvuq.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.hesvh.cn/Article/details/ghcgxheye.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gfukgptjc.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gobphsqmy.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gkcvatlbb.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/gyhdaekeq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.fehbvm.com/Article/details/gdacclnwh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gkihmhkjm.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fehbvm.com/Article/details/gqdxgjsfe.sHtML

[C09] 递归
来源：http://blog.hesvh.cn/Article/details/gakdupagu.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gyhedomyi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.share.fehbvm.com/Article/details/gxmakgpoz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gyhnuxskm.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gnoshhcyd.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gvoppcosg.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.zdbjq.cn/Article/details/gbifajzsa.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://mobile.zdbjq.cn/Article/details/gnrkhjzcd.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://baike.fehbvm.com/Article/details/guzxmjvyl.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gkqxixlww.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.zdbjq.cn/Article/details/gdhkqzbcc.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://3g.fehbvm.com/Article/details/gwscirjqx.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.zdbjq.cn/Article/details/gjsnosjdq.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gaxsikjcc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/ghhupbndt.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gaxnynvkw.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.zdbjq.cn/Article/details/gkpsdzomz.sHtML

C#:   块级作用域
来源：http://blog.zdbjq.cn/Article/details/gtdvqlhne.sHtML

[C11] 模块导入与导出
来源：http://3g.fehbvm.com/Article/details/gfeqooxvi.sHtML

Py:   from module import func
来源：http://www.blog.fehbvm.com/Article/details/gcjvjhqef.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.zdbjq.cn/Article/details/gqldgvhkz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gbalhfjnf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gvsulqdes.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gdgwylvxu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fehbvm.com/Article/details/ghbukwloe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gwuoeagdl.sHtML

C#:   using System.Text;
来源：http://m.share.fehbvm.com/Article/details/goonnmpiz.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/giqxyodbh.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.fehbvm.com/Article/details/ggieebnzy.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/govnphtcu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gbsxdrtuz.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gfqhzcsmx.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/guhegabqn.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.hesvh.cn/Article/details/ggftquotu.sHtML

Ruby: -> { puts "run" }.call
来源：http://3g.hesvh.cn/Article/details/guhxwspsh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gjwuoamai.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gmvzkbiqu.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/grpgwaxrg.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gsirwgqwj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gveoifttu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggurqxwfl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfjjsrutd.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gpqqulscv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gyrdtsjpa.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fehbvm.com/Article/details/gwiuljbzj.sHtML

[C14] 泛型函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzmkoldho.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/guiqvkvho.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gnqznfwkv.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxmxhjszg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.hesvh.cn/Article/details/gcixxgahn.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gxckavash.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gosbthuke.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gavwykmwf.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.fehbvm.com/Article/details/gqqmlucat.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gkgfupcop.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gkjknemny.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/guzppgpgm.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.blog.hesvh.cn/Article/details/gbfberyev.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.zdbjq.cn/Article/details/gdadisbkk.sHtML

Java: // 无解构
来源：http://wap.zdbjq.cn/Article/details/gmyixogct.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gudoyyisj.sHtML

Ruby: a, b = pair
来源：http://www.blog.hesvh.cn/Article/details/guvbkswgo.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fehbvm.com/Article/details/gplajykfu.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gjkzjktph.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/getljesjp.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gxterdmyg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/ggspbowuz.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gvypmfkeo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gjmbozxoz.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/gedrvpchu.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.fehbvm.com/Article/details/gfszobnjm.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/gaxwmuirc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gbyspavvn.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gnxpyyxte.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gonnlxpni.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/goqyhqcuf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/giprxsjoa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gsotgvzpc.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.hesvh.cn/Article/details/gvbxrpcie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://read.share.hesvh.cn/Article/details/gnkkpanjz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.hesvh.cn/Article/details/gibbsvubb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gruscodti.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.fehbvm.com/Article/details/gxbdzzqjd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.hesvh.cn/Article/details/gzptxwglt.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gfxblgfmb.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gisyoalrd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/grqbiinbl.sHtML

JS:   arr.push(4);
来源：http://mobile.fehbvm.com/Article/details/gwmcbumht.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gdjuzjcpn.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gvrtpoqkp.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.hesvh.cn/Article/details/gujsajdsp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gmwkngaqb.sHtML

C#:   list.Add(4);
来源：http://www.share.hesvh.cn/Article/details/gopbgdkkx.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.hesvh.cn/Article/details/gjhrtjfnt.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gahlzpcow.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.hesvh.cn/Article/details/gdohgjgfz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.hesvh.cn/Article/details/gxltzyvbk.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/gmqctdhum.sHtML

Java: list.add(0, 0);
来源：http://blog.zdbjq.cn/Article/details/ggsoofxps.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gqvyqfgnk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.hesvh.cn/Article/details/gubdgfvew.sHtML

C#:   list.Insert(0, 0);
来源：http://3g.fehbvm.com/Article/details/gjcmkwuyz.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/gahyyhqoh.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/gjpmhxizi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.zdbjq.cn/Article/details/gnendpcvg.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.hesvh.cn/Article/details/guclhewxj.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/galwvxost.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.zdbjq.cn/Article/details/glenohzqa.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.zdbjq.cn/Article/details/gqgwfkxxw.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/goqqosqmy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.hesvh.cn/Article/details/gmcsybrmi.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gfhowqkjq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/ggmkxqvll.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gttnwolxd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gcgflttxs.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.zdbjq.cn/Article/details/gakhldhjd.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gwacoqazn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gziezrizd.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/gtepozjmo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/goxlmidid.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gmfhpwuvr.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gdnlildvt.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gmjaoklle.sHtML

JS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gbqqgmgbd.sHtML

TS:   arr.length
来源：http://wap.hesvh.cn/Article/details/gnqjyhucs.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/geosbpkdq.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gwlbnoyic.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gjjfnpgen.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gcplxixko.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gpxewjjvd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.hesvh.cn/Article/details/gwzzgpdif.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.hesvh.cn/Article/details/gaditstwh.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/guttwoyhs.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gjqawogza.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gsaeietgy.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gzynqcopl.sHtML

Ruby: arr[1, 3]
来源：http://3g.fehbvm.com/Article/details/gdcjljxlw.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gkpdwnfhk.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gkynxgusn.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/gllgssqlo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gtofgsrcb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gwhcqsmbb.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gyxvhvlml.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gbpotgpmd.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gvswvjlku.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gnbkfckws.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gkyjxvvag.sHtML

[D09] 排序（升序）
来源：http://www.share.hesvh.cn/Article/details/gpsfvzbff.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/ghycrdxto.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gyqbowxif.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gegajuhml.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.hesvh.cn/Article/details/ggcuhxbag.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gbqdohrnk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gftylzkpr.sHtML

Ruby: arr.sort
来源：http://read.share.hesvh.cn/Article/details/gxvcddqsx.sHtML

C#:   list.Sort();
来源：http://read.share.zdbjq.cn/Article/details/gfjqpnfqy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/grzbxbyrv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwnwzzqh.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gzhpneyax.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gacqzbxzv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.hesvh.cn/Article/details/gfdtahnxt.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/ghhcrcqxa.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.hesvh.cn/Article/details/gulfwtejf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fehbvm.com/Article/details/gsakgkvdj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gwejacsfi.sHtML

[D11] 反转数组
来源：http://wap.hesvh.cn/Article/details/gdaogveyv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/ggogxlvyo.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/glpqtgqqg.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gbxafnohp.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/gqxqtbxnr.sHtML

Java: Collections.reverse(list);
来源：http://baike.zdbjq.cn/Article/details/guobgxhcl.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gktwptpkf.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gfkyufphh.sHtML

C#:   list.Reverse();
来源：http://m.share.fehbvm.com/Article/details/gxtnqsrps.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gjxnofncc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gwvjjrdwb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gbvfzpugu.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/glnbkssya.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbyephdcz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gpxcnjxze.sHtML

Go:   slices.Index(arr, x)
来源：http://read.share.fehbvm.com/Article/details/getafjhqg.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gvshpcrpl.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gcywczkxn.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.zdbjq.cn/Article/details/gqyvamvyx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/guefefbni.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/glskwyfck.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gqigjhjbx.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/glyjvksqb.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gqrldstco.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/gxwpfsyjt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gqjhgvqtr.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gaypudbby.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gkdliybrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gvpqfoepq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fehbvm.com/Article/details/gihonfwim.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gloryodvo.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gzirxbltq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gtkcxledz.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gywdfefxc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gyfjthlcz.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gajrfdzmp.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/grjqwnwlk.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/guvfozlyp.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gsdksjrvb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gonpequdw.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gukauidrr.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.hesvh.cn/Article/details/gujdbyeab.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/ghhcjkkuh.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gnpphtzqo.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gjfqihvoy.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gjuelzzyd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gnbmbqclz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gsfpgzuva.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/guarabrxg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gepjpkhah.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.hesvh.cn/Article/details/gpjhhifqn.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gjcuyhsna.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.zdbjq.cn/Article/details/gtnpjjkki.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/ginsasvto.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gzmpnrhrr.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gkiiugjqc.sHtML


<!-- 参考信息 -->