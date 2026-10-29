代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ghoqxoyqb.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gtirajnkf.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gytyaakut.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gnepjwnlq.sHtML

[C02] 默认参数
来源：http://www.share.hesvh.cn/Article/details/gccsuebnu.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/ggbtdispg.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.zdbjq.cn/Article/details/gdlrlwsuy.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.zdbjq.cn/Article/details/ghffpqjdg.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gxryjrpkz.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.blog.hesvh.cn/Article/details/gmxzttisy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.fehbvm.com/Article/details/gmbmlcfka.sHtML

Ruby: def greet(name = "World") = name
来源：http://baike.zdbjq.cn/Article/details/gtglfpsqk.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.zdbjq.cn/Article/details/gsexgrizo.sHtML

[C03] 可变参数
来源：http://blog.zdbjq.cn/Article/details/gkczatxks.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.zdbjq.cn/Article/details/gphzsdpsf.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.fehbvm.com/Article/details/gmyhqeakg.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gkytdvvts.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gsfekthsm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/giduzkrca.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.zdbjq.cn/Article/details/gmdstkcsx.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gizpnbugo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://wap.fehbvm.com/Article/details/gdchrpkff.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.zdbjq.cn/Article/details/gedgoxosr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://3g.hesvh.cn/Article/details/geakfctlp.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://mobile.fehbvm.com/Article/details/gjiudyaam.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gbrirqdex.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gpochrgpo.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/gckrxomax.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.hesvh.cn/Article/details/giepdknde.sHtML

Ruby: f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gjifofrst.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.fehbvm.com/Article/details/gzizustwc.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/geexlwjkb.sHtML

Py:   return a, b
来源：http://mobile.fehbvm.com/Article/details/gurxuobkn.sHtML

PHP:  return [$a, $b];
来源：http://wap.zdbjq.cn/Article/details/giatmfypo.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.fehbvm.com/Article/details/gnqdnslmn.sHtML

TS:   return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/grhjunmky.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://blog.hesvh.cn/Article/details/gekiqvcfj.sHtML

Go:   return a, b
来源：http://www.share.zdbjq.cn/Article/details/gilhfpaux.sHtML

Ruby: return a, b
来源：http://3g.zdbjq.cn/Article/details/gelpiaiez.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.zdbjq.cn/Article/details/gnyoeejbb.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gvwwqpsri.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/ggllyhtyz.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.zdbjq.cn/Article/details/gwmeknduu.sHtML

JS:   const square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/ghouiiacj.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://m.share.hesvh.cn/Article/details/gjqtoazwh.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjozptr.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.fehbvm.com/Article/details/gfbxjlpik.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.blog.hesvh.cn/Article/details/gzelgwivn.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gicxlaeua.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gopewddho.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.hesvh.cn/Article/details/gkzasubgd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gncpzavfn.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.blog.hesvh.cn/Article/details/gipuraouu.sHtML

TS:   arr.map(String)
来源：http://m.share.zdbjq.cn/Article/details/gfdyrvhbp.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://wap.fehbvm.com/Article/details/glwwnxkpa.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.zdbjq.cn/Article/details/gihevkyrh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.zdbjq.cn/Article/details/gckwtkvrm.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gflwasszr.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/ggkuznatm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://mobile.hesvh.cn/Article/details/gslxqpoal.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.fehbvm.com/Article/details/gcapumlak.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/govgbrvme.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/gtfknpavh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/gpduspizc.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.zdbjq.cn/Article/details/gztfhukpp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://m.share.hesvh.cn/Article/details/gihteqszo.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gzfdyontp.sHtML

[C09] 递归
来源：http://m.share.hesvh.cn/Article/details/gynljccvz.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.hesvh.cn/Article/details/gbcobwbsp.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjqvhlgxq.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gfvblfmwq.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gabwplbjt.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/giurnwmva.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.hesvh.cn/Article/details/gdzlrczxw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.hesvh.cn/Article/details/gegwcphoj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gkyisfxpb.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gumhnwzao.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.hesvh.cn/Article/details/ggipmmwdj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gtnfeldaj.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/grcfeecpw.sHtML

TS:   同 JS
来源：http://3g.fehbvm.com/Article/details/ghfzztsrc.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/giwekaqoz.sHtML

Go:   花括号块级作用域
来源：http://wap.zdbjq.cn/Article/details/gffmcjvyz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.zdbjq.cn/Article/details/gzwoppjmw.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gixfgchkf.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gwxgurwhd.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gfcwzisnb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gwomxduuz.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gqogrlrek.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gixvnjvtu.sHtML

Java: import java.util.List;
来源：http://www.m.share.hesvh.cn/Article/details/gmyiktvfb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.fehbvm.com/Article/details/gwvibwcus.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gqxzwgttt.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/gpzhyxykc.sHtML

[C12] 立即执行函数 IIFE
来源：http://baike.hesvh.cn/Article/details/gzdymsegl.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gormuedsk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/gtxwvjper.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gmwiiwanb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fehbvm.com/Article/details/gfokluluf.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.hesvh.cn/Article/details/gexemmvqi.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gwazwntds.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.zdbjq.cn/Article/details/gtbpwouuo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gohqgyevu.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.zdbjq.cn/Article/details/gzflvwjoa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gialcnmwu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjgbyxkm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.hesvh.cn/Article/details/gdaujeklz.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gsynhyqmr.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ghoonzirq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gsvsqjvyn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gsxalvzes.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/genyhzydi.sHtML

[C14] 泛型函数
来源：http://www.share.fehbvm.com/Article/details/gwppexhtg.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.zdbjq.cn/Article/details/gmlupfejl.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/ggpanobci.sHtML

JS:   // 无泛型
来源：http://wap.hesvh.cn/Article/details/gdkfqurph.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.hesvh.cn/Article/details/ggoeymrmf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.zdbjq.cn/Article/details/guracffrl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gxjumlshr.sHtML

Ruby: # 无泛型
来源：http://mobile.zdbjq.cn/Article/details/gelmwwqwl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gnnhxvrfl.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gijguwocr.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/goaechdyd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.hesvh.cn/Article/details/gncsunecb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjwbpwagc.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.hesvh.cn/Article/details/gsoyqsfij.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gueorlajp.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gqgtppcwf.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/gezfmzvhq.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gpbkusvhf.sHtML

[C16] 函数 / 方法重载
来源：http://blog.zdbjq.cn/Article/details/gfwchbnhf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gqyyzkhoi.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gntesejvi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fehbvm.com/Article/details/gcatsnfwv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.fehbvm.com/Article/details/grdovngwq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gcmclfbrs.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.fehbvm.com/Article/details/gfpbixbwq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gobdvpgiv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gbdjhcskb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsvjxiywb.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gdqsdjhch.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gupstvkmv.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gnvloxclp.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.zdbjq.cn/Article/details/gthbhzcvi.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gskuypuqw.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/gzotflbtd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/glpwyfjej.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gzkpwkdpn.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gmmchtoeq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.fehbvm.com/Article/details/gpnukasbd.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gkpbcyzjs.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gquajcdeq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.hesvh.cn/Article/details/gehdiuxom.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.hesvh.cn/Article/details/gsloverlq.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/glegjrekj.sHtML

TS:   arr.push(4);
来源：http://wap.fehbvm.com/Article/details/gjtzrrweg.sHtML

Java: list.add(4);
来源：http://read.share.zdbjq.cn/Article/details/gnxljonbc.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gbcqoavhh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.hesvh.cn/Article/details/gswchoied.sHtML

C#:   list.Add(4);
来源：http://mobile.zdbjq.cn/Article/details/glpvqwmsz.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.zdbjq.cn/Article/details/guekbvwrt.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fehbvm.com/Article/details/gpvgoqzxd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/gnhnmuudb.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gpcdnqcdn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fehbvm.com/Article/details/gejibxvsq.sHtML

Java: list.add(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gohiiimgc.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/gdrqtaqzc.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gurhvjjny.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/ghuxkoujx.sHtML

[D04] 删除元素
来源：http://www.share.fehbvm.com/Article/details/gowzbqnng.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gfaqyinwj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.hesvh.cn/Article/details/gotedqdhp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gxabiuoei.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fehbvm.com/Article/details/gojxbftgh.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gbtygggnt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gyvrtfhot.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/greojpuib.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.fehbvm.com/Article/details/gakwwwdbx.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gtxvevmtr.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gcxfdjkde.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/grvlzvctt.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/ggktieyxn.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gpdblfvwo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gkecmpdzv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gsyddqwpl.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gjfmdwobj.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.zdbjq.cn/Article/details/gehqkrjkl.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gxjwrkoyh.sHtML

Py:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gcilkauiz.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gejlxqtks.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/gstyazgqa.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gllyncpoi.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gjvbrstqd.sHtML

Go:   len(arr)
来源：http://wap.zdbjq.cn/Article/details/gieatxozr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gxefxxeqf.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gtvjknuhj.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gtwxhlwws.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/govvvvaax.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gwyflntwq.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gywcipjph.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gpqupgzct.sHtML

Java: list.subList(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrhfldoo.sHtML

Go:   arr[1:4]
来源：http://www.blog.zdbjq.cn/Article/details/gzevbhqfi.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gytxpjsmu.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.hesvh.cn/Article/details/grqbdwysu.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/gdaqmoybx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gntjmbwwo.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fehbvm.com/Article/details/ggygzurli.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/gkauzdxgj.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/gxjbsfmcn.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://baike.zdbjq.cn/Article/details/giwsdljub.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/gmxrhwyol.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gywhsqqwv.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/ghdsdyoab.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gmfcioxzi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/gmiswldoy.sHtML

PHP:  sort($arr);
来源：http://www.share.zdbjq.cn/Article/details/gqhunzofi.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.fehbvm.com/Article/details/gcdiwdybr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gvfxprtcg.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.fehbvm.com/Article/details/gtfxdddgw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gxpzyhsni.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/guqohcoou.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/ghpbxlzit.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gjmynnbxn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/gohwxhggx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gjusbrkyl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gwhtyqycw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/ggecarwfc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.hesvh.cn/Article/details/gnxgkcewr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gmybdgzda.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gmeqksbcz.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/glqgkokup.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/gyzjhquhj.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fehbvm.com/Article/details/gmekwqtmn.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/geudfxdcn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.zdbjq.cn/Article/details/gqgznyosw.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gitrturtx.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.zdbjq.cn/Article/details/gjlxdzakm.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gexzyqfdb.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gjumqlfuk.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/ggqhsvsur.sHtML

[D12] 查找元素下标
来源：http://m.share.zdbjq.cn/Article/details/gnsmtqzjk.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gycckrixz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/guxmsyrzl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdklcsvq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gyybypfru.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gbpamobmi.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggtjurycq.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gfpkbokpb.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gtfakofik.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gaqdergye.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gcsopxxyi.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gfqswgiwg.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/grnjdmuhj.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gydbplggm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gfvewzzfr.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/gxjzrsimg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gasedpkok.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gawxlnzyc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gspxmtafs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gtswiqzcp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/guerzigfz.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gdkzbubca.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gyizqmfct.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/ghohyifam.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gfrbkoioz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gigidkfyx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gdkjikmcr.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gnpizdwof.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.zdbjq.cn/Article/details/gcxekdtvo.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gukqhzjxd.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gxjpczdww.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gmttmmsuk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gsaawgzpe.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gumjggpaq.sHtML

Ruby: arr.uniq
来源：http://www.blog.hesvh.cn/Article/details/ginjjymys.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gphkaqqah.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gyqsfqikc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gjqvxqyck.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/govzuidum.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/gjiyxwnvr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/gvkgfeqln.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gacetnnlv.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/ggwrwlcgj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gngolugas.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gnlptydmx.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/gwjwxmdbo.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gjaymqgka.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gwbaxjwjz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gezsbrcxp.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gdqqsygmi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gcnazgvqn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gsruzukey.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/gnqbnjlen.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gqyzcslvk.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gercvtthl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gjkxxbpjz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/guxwguayg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gagmqahoz.sHtML

TS:   nested.flat();
来源：http://www.blog.zdbjq.cn/Article/details/gkehlnivv.sHtML


<!-- 参考信息 -->