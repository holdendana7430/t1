代发 wailian999

Java: if (data == null) return;
来源：http://read.share.fehbvm.com/Article/details/gvkdesiro.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gsavyxwfh.sHtML

Ruby: return if data.nil?
来源：http://www.blog.fehbvm.com/Article/details/gvjulwiln.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gtygjsgvz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gbtujlftq.sHtML

C. 函数与作用域
来源：http://www.blog.hesvh.cn/Article/details/gstamhevl.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbjfzrinb.sHtML

[C01] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmnecrgqw.sHtML

Py:   def add(a, b): return a + b
来源：http://baike.hesvh.cn/Article/details/gydfdqdmq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gqebnspid.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdnfoicle.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gogxiolpv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdquowqcm.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.hesvh.cn/Article/details/gcgzpuqwh.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gaqxagdkr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gbieryztu.sHtML

[C02] 默认参数
来源：http://www.m.share.fehbvm.com/Article/details/grubjjltk.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gncukckxj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/guekgmkqq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnmcrsdkj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.zdbjq.cn/Article/details/gwdulssxj.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.fehbvm.com/Article/details/gjjftbfoy.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.zdbjq.cn/Article/details/gbetfycbk.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.zdbjq.cn/Article/details/gqdjfpdnx.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.blog.hesvh.cn/Article/details/gfgfncmjt.sHtML

[C03] 可变参数
来源：http://3g.zdbjq.cn/Article/details/gsnivbeyz.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.fehbvm.com/Article/details/ghyenceqc.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.fehbvm.com/Article/details/gvdxfaqpv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/gyrvutqvl.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.fehbvm.com/Article/details/gonvoefpz.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gieulwfay.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://blog.hesvh.cn/Article/details/gbszfkdym.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://baike.fehbvm.com/Article/details/ghiwsiqxc.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gyixxwvdo.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.zdbjq.cn/Article/details/gjlzpiayp.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.zdbjq.cn/Article/details/gajkztvbo.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.zdbjq.cn/Article/details/glgufhurx.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.hesvh.cn/Article/details/gbotcxxtm.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gpbhlvjth.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.hesvh.cn/Article/details/gohmkgthy.sHtML

Go:   // 无：用配置结构体参数
来源：http://m.share.zdbjq.cn/Article/details/gszmkgxdj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.hesvh.cn/Article/details/gfvjznwpd.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/gyxhgtokr.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gvftifkep.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gegpquuui.sHtML

PHP:  return [$a, $b];
来源：http://blog.zdbjq.cn/Article/details/gqugqjcnx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/ggkwtmjgn.sHtML

TS:   return { a, b };
来源：http://www.blog.hesvh.cn/Article/details/gpwzorhla.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://m.share.fehbvm.com/Article/details/ggvvhuqec.sHtML

Go:   return a, b
来源：http://baike.hesvh.cn/Article/details/gxyhkxfgy.sHtML

Ruby: return a, b
来源：http://www.blog.zdbjq.cn/Article/details/geqflgcpp.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.share.fehbvm.com/Article/details/gabfnthfq.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.zdbjq.cn/Article/details/ggnrysmok.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/giblnuwim.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.fehbvm.com/Article/details/gdswufral.sHtML

JS:   const square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gpydugdzl.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gjghowvva.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.share.zdbjq.cn/Article/details/gmikwffap.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://wap.hesvh.cn/Article/details/gagstaguf.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.hesvh.cn/Article/details/gintpcjsh.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.zdbjq.cn/Article/details/gkuqxbgpq.sHtML

[C07] 把函数作为参数传入
来源：http://www.share.zdbjq.cn/Article/details/gxdioberr.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.m.share.zdbjq.cn/Article/details/gwrxuribj.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.zdbjq.cn/Article/details/ggpfladxt.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.zdbjq.cn/Article/details/gcsgpsqls.sHtML

TS:   arr.map(String)
来源：http://3g.hesvh.cn/Article/details/gywgvrtkq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/ghhxckvdj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.hesvh.cn/Article/details/gtadbefta.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gvbwrgzcd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/gdoqmyjbw.sHtML

[C08] 闭包
来源：http://blog.zdbjq.cn/Article/details/gsqrludqx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gliorklyk.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.fehbvm.com/Article/details/grqvvctvr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/glrmpeabh.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.hesvh.cn/Article/details/gfkrqjpoq.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://baike.fehbvm.com/Article/details/gasnwvcva.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.hesvh.cn/Article/details/gunayhayb.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://read.share.zdbjq.cn/Article/details/gqobdliez.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gmahdcyrj.sHtML

[C09] 递归
来源：http://m.share.fehbvm.com/Article/details/gnnyfxlsi.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gxozspvqf.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.zdbjq.cn/Article/details/gyjgilpjp.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.hesvh.cn/Article/details/gmawsicbt.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gcngyqqsp.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gtdklxjdb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.hesvh.cn/Article/details/gyzlkdowl.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.fehbvm.com/Article/details/gtihgtpxg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://m.share.hesvh.cn/Article/details/gvresmdfc.sHtML

[C10] 变量作用域
来源：http://wap.fehbvm.com/Article/details/gwvgqsuon.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gssxpefin.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gqphuuobq.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.share.fehbvm.com/Article/details/gdatbkaie.sHtML

TS:   同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gjxfesbge.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/goydljbbq.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gfbwaibqi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fehbvm.com/Article/details/guckqxief.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gkcfowzhp.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gmoymcxfq.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gmfynatif.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gepjqasad.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/grmzrflyj.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/gdqobroth.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/ggsrxoyvz.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/ggotssrmu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gtorduufl.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/govnixczp.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.zdbjq.cn/Article/details/glkdoiozi.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.fehbvm.com/Article/details/gqxeyipig.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/ghdcmhlzm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gurhxonry.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gvfcnknab.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.hesvh.cn/Article/details/gtxqvedre.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gjvewdwdp.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gnwkcqoms.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gaudicaxl.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gmgnvzdue.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gmcdwzhsu.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gtpwwbjkx.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gcybzkogn.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/ganxncgiy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gzlxuceia.sHtML

Go:   func add(a, b int) int
来源：http://m.share.hesvh.cn/Article/details/gtafaxgra.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.hesvh.cn/Article/details/gdduvqnet.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fehbvm.com/Article/details/gmcdiepfa.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/guiqcmqvi.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.hesvh.cn/Article/details/gmehfmtya.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/geniliean.sHtML

JS:   // 无泛型
来源：http://baike.hesvh.cn/Article/details/glkflkqmt.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gnbvnkytd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.zdbjq.cn/Article/details/gosxlzahp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gcfdbevdw.sHtML

Ruby: # 无泛型
来源：http://3g.fehbvm.com/Article/details/gnavcrcse.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gbeodewwq.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.hesvh.cn/Article/details/gwyauasdg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.zdbjq.cn/Article/details/gyglgvitx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.zdbjq.cn/Article/details/gfknirwaq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.hesvh.cn/Article/details/gdpqihunm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.fehbvm.com/Article/details/gbtkcrxoz.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gwmitdylh.sHtML

Go:   // 无解构
来源：http://mobile.zdbjq.cn/Article/details/geinhdewu.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/gaqibfywt.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.zdbjq.cn/Article/details/grbjodgdx.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.zdbjq.cn/Article/details/guuiyuaat.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fehbvm.com/Article/details/gaojziekd.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gupfltctn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/gcxvceqvf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/gidawyeeq.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.fehbvm.com/Article/details/gvbbtknzt.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/guwsdsyyo.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gzecnrkzb.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.fehbvm.com/Article/details/gbgozaaiu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grkqhoyyh.sHtML

D. 数组 / 列表 / 集合
来源：http://read.share.zdbjq.cn/Article/details/gzuoezvvj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvjwggawl.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghgiiipce.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://baike.hesvh.cn/Article/details/gocrdynto.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gfskjcprt.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/ginqetjvd.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.zdbjq.cn/Article/details/gzmqkgnzf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fehbvm.com/Article/details/gbwrzvapm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.hesvh.cn/Article/details/geuaevigc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.fehbvm.com/Article/details/guqxdpbyh.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.hesvh.cn/Article/details/gaidqmxnz.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gxyyteeje.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.hesvh.cn/Article/details/grsrbmayl.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gzygvmnvp.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gjbplzpyn.sHtML

TS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/gavlzvijg.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gpbnxshcs.sHtML

Go:   arr = append(arr, 4)
来源：http://blog.zdbjq.cn/Article/details/gssngyzsz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gsfpvwcma.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gegjwezfr.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/guidagaeo.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gtujvvsse.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gkayakjcp.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.zdbjq.cn/Article/details/gtuufghme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/grbaikogz.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwdobtpiy.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.hesvh.cn/Article/details/garwrxfwk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.hesvh.cn/Article/details/gbafbufnc.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/ghrmmlbyt.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gnmagxozm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.zdbjq.cn/Article/details/ggmqhdzhv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/giyridhfk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.fehbvm.com/Article/details/gvvqjvmsg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gevgvxcjn.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.hesvh.cn/Article/details/gxrmidgab.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gojcmuscm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.hesvh.cn/Article/details/gaxpotpts.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gmadynvuf.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/gmdnitxle.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gctzpfzpr.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gvsxoexgl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gikblpnlg.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gqpivokkz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/goacidzmo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfrgeoots.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gwcltvxcs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gutnkyvhf.sHtML

[D06] 数组长度
来源：http://wap.hesvh.cn/Article/details/grfmdnfkg.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gemtjmclw.sHtML

PHP:  count($arr);
来源：http://blog.zdbjq.cn/Article/details/gqpkwcwho.sHtML

JS:   arr.length
来源：http://mobile.fehbvm.com/Article/details/gootvrsin.sHtML

TS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gdjzpvysb.sHtML

Java: list.size();
来源：http://www.blog.zdbjq.cn/Article/details/gxvyoucif.sHtML

Go:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gbjqhefyj.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/ggzssdxqa.sHtML

C#:   list.Count;
来源：http://m.share.hesvh.cn/Article/details/grzjshnwm.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gjflrmwdc.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gumcderbn.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.hesvh.cn/Article/details/gifdmibae.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gmtblbutk.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gvlhrdwis.sHtML

Java: list.subList(1, 4);
来源：http://3g.hesvh.cn/Article/details/gnfvkchwm.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gxoypreve.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.fehbvm.com/Article/details/guwuvywox.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gmvtboyzy.sHtML

[D08] 合并两个数组
来源：http://www.blog.hesvh.cn/Article/details/gkadeqzla.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gpbtqyfrs.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.fehbvm.com/Article/details/gspsupaqq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gfdxeolqw.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gfuukdopa.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gabnoqcgx.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/grgjqiuxi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/ggdldquym.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/grkazzyan.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/gquokqkgl.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gcgvkyjyw.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/gdcqvrbmu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gfiwkgcqm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.hesvh.cn/Article/details/gvxjrvete.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.hesvh.cn/Article/details/gqybchfle.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gxkxwlmiw.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gbfmploxc.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gwqepskot.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.zdbjq.cn/Article/details/gkzwttpdo.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.hesvh.cn/Article/details/gduxflvva.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gyyumdjmw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gysqwhhpz.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gwxdzdutf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.blog.zdbjq.cn/Article/details/gbqttmnkm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/gomdmupqh.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.fehbvm.com/Article/details/gtpruywkp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.m.share.hesvh.cn/Article/details/gsmkbdxkz.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gdlnkvwun.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gerwgzvdp.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/ginbmfzrm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gmqulcqyg.sHtML

TS:   [...arr].reverse();
来源：http://3g.fehbvm.com/Article/details/gsgennkfx.sHtML

Java: Collections.reverse(list);
来源：http://m.share.hesvh.cn/Article/details/gdusholxv.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkwfeshkt.sHtML

Ruby: arr.reverse
来源：http://blog.hesvh.cn/Article/details/gvjqqlszq.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gbvuwzdbg.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gbiwdcjqe.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fehbvm.com/Article/details/gbwkxnncb.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.fehbvm.com/Article/details/gcnuqyfhr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/ggetrjles.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gikfspbkb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.fehbvm.com/Article/details/gafttjbbx.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/guxllsupt.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/groeuyuce.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gyyuegabm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gcezarqnf.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/gkpraioyk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gyzxxpcqo.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gngplvilu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gykxpgwsm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.hesvh.cn/Article/details/gbzavjcuq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gygvlhdcs.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.zdbjq.cn/Article/details/gpybqyzyx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gfcrcqoki.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gdalbsixb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gjedkhsdn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvxvryyyb.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gnymjlhhl.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/gbskislqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmcycggcm.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gjsitcqhg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gqqoartbc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/guautnxyt.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gsaatdieh.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/gdtnotnjs.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gpcoubhqm.sHtML

JS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/geaqkcrih.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gquwifwub.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.hesvh.cn/Article/details/giazibekg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/ggjpihqfb.sHtML

Ruby: arr.uniq
来源：http://read.share.zdbjq.cn/Article/details/gkxujgnzw.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/gfhkvzjri.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gaxzioggv.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/guwgtjrtr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gkiyzmobx.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ghsdspwqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gjeieqzgr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fehbvm.com/Article/details/gzrweacbk.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gmilvtwyf.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gpinntwzw.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.hesvh.cn/Article/details/gvgtgeikb.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/grycwjlnz.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxdteoxul.sHtML


<!-- 参考信息 -->