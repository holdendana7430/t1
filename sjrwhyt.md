代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gnixrwjjk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/gsxxkqhha.sHtML

Ruby: def add(a, b); a + b; end
来源：http://3g.fehbvm.com/Article/details/grhmewbaa.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gjfdexnbk.sHtML

[C02] 默认参数
来源：http://www.share.zdbjq.cn/Article/details/gywetelew.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/ghlkarptk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gamrixuoz.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gkoxnozwz.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gpxfboype.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gqbszejtn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://m.share.hesvh.cn/Article/details/gvgrffner.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.hesvh.cn/Article/details/gjsiuqvoa.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/guixwylgh.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/gvuasfkkd.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.hesvh.cn/Article/details/geysmjhda.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fehbvm.com/Article/details/gnkmzbekq.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/gliqesfee.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.fehbvm.com/Article/details/ggvfhvfto.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gtslnbveb.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.zdbjq.cn/Article/details/gpcuzkwcp.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gfyazbjnq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.blog.hesvh.cn/Article/details/galbsapdh.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.fehbvm.com/Article/details/gjnsqxerx.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.zdbjq.cn/Article/details/gbmebzvtb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://m.share.fehbvm.com/Article/details/ghqmqsypv.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gnutrmfrc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gqzdjpvht.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gasqzlhee.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.blog.fehbvm.com/Article/details/gseaboqsd.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fehbvm.com/Article/details/gwvpxzksj.sHtML

C#:   f(a: 1, b: 2)
来源：http://wap.hesvh.cn/Article/details/gxlltczqo.sHtML

[C05] 返回多个值
来源：http://read.share.fehbvm.com/Article/details/gjmiypxhw.sHtML

Py:   return a, b
来源：http://baike.fehbvm.com/Article/details/gevjsyhoh.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gifvigvnh.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/grnodozel.sHtML

TS:   return { a, b };
来源：http://www.blog.zdbjq.cn/Article/details/gkwyvmlyv.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/goxcaiifl.sHtML

Go:   return a, b
来源：http://www.blog.hesvh.cn/Article/details/gbprmlpkg.sHtML

Ruby: return a, b
来源：http://3g.hesvh.cn/Article/details/gurasghir.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://m.share.hesvh.cn/Article/details/gtrgmdxhd.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/grhjvjbhh.sHtML

Py:   square = lambda x: x * x
来源：http://3g.fehbvm.com/Article/details/gkfzawful.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://wap.hesvh.cn/Article/details/gvakuprnl.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gofgtfgyb.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.hesvh.cn/Article/details/gnmreknov.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://read.share.hesvh.cn/Article/details/giiovbqfm.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://baike.fehbvm.com/Article/details/gswtmxuyx.sHtML

Ruby: square = ->(x) { x * x }
来源：http://mobile.fehbvm.com/Article/details/geyatglbf.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/gcklbprqm.sHtML

[C07] 把函数作为参数传入
来源：http://baike.fehbvm.com/Article/details/gipuiagej.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.blog.fehbvm.com/Article/details/gicauhqrk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://3g.hesvh.cn/Article/details/gsnnvhbmd.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gegqsvdoh.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gqnlkirjk.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.fehbvm.com/Article/details/gyizqscxo.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://mobile.hesvh.cn/Article/details/gvevuivic.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.zdbjq.cn/Article/details/gxjwwwgdj.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.hesvh.cn/Article/details/gxlrfljza.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gbkitrluj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.share.zdbjq.cn/Article/details/gziaxitpw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.fehbvm.com/Article/details/gerxywbxh.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/guqyfjjxz.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://read.share.fehbvm.com/Article/details/gijtkcctg.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://read.share.hesvh.cn/Article/details/gfihmjklx.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.blog.hesvh.cn/Article/details/gzelpqgvr.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.zdbjq.cn/Article/details/gwnjtqlft.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.zdbjq.cn/Article/details/gdmprxlde.sHtML

[C09] 递归
来源：http://www.blog.hesvh.cn/Article/details/gnkhgtomq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://mobile.hesvh.cn/Article/details/gkizwpjpi.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://read.share.zdbjq.cn/Article/details/gcvjjghgr.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://read.share.zdbjq.cn/Article/details/gamemimen.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gyngrfmmb.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://wap.fehbvm.com/Article/details/glflqwmjb.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gehjzxmhh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://m.share.fehbvm.com/Article/details/gzqginknw.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.hesvh.cn/Article/details/gpajqykwv.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gvkfeecmr.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://wap.fehbvm.com/Article/details/gvyuluejz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.zdbjq.cn/Article/details/gjlturzbe.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://read.share.hesvh.cn/Article/details/gdhchlcfd.sHtML

TS:   同 JS
来源：http://3g.hesvh.cn/Article/details/geygdgvvs.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.fehbvm.com/Article/details/gzcsuxdsz.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/grudlzxgb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.zdbjq.cn/Article/details/gsmlmjzdh.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/ghlxvfnhz.sHtML

[C11] 模块导入与导出
来源：http://baike.fehbvm.com/Article/details/giyirjtnf.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gevzxpohd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/gbjpnozyb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gtfseqxxq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.zdbjq.cn/Article/details/gmkvybbvd.sHtML

Java: import java.util.List;
来源：http://blog.fehbvm.com/Article/details/ggyeokstq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fehbvm.com/Article/details/gckyerope.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.fehbvm.com/Article/details/grnnsugqy.sHtML

C#:   using System.Text;
来源：http://www.m.share.fehbvm.com/Article/details/gwykcvheo.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/guahxmcte.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fehbvm.com/Article/details/gaeuwhovp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/gdffbqgrx.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fehbvm.com/Article/details/gonmvorjt.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gjjukuyre.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.zdbjq.cn/Article/details/gfipshcdv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gikevnoiw.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.zdbjq.cn/Article/details/guhhsmbah.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.zdbjq.cn/Article/details/gggabdjbk.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fehbvm.com/Article/details/gnhuodktg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.zdbjq.cn/Article/details/gzvklqevk.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.zdbjq.cn/Article/details/gmyhfwbad.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fehbvm.com/Article/details/gopvirgxw.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gyqbmcrzq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/grvdlnrro.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gnmgebisx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gnrimmyal.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gyqrsnohw.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gcyviedyb.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gbghmndbp.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gwcvgsrgg.sHtML

JS:   // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gbsxqbvmc.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.fehbvm.com/Article/details/gdrqrepqt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gxshwmvrd.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.fehbvm.com/Article/details/gwqztswmt.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gsvabhobo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.zdbjq.cn/Article/details/gjkqsqfqx.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gekzytqrf.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/gfnjwylqe.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/ghynwltxb.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/goxkcscrh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gjwvbcpfd.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/ghchvvbsf.sHtML

Go:   // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gcyezgsdw.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/gxgpcfxzu.sHtML

C#:   var (a, b) = pair;
来源：http://blog.hesvh.cn/Article/details/gngmujvtr.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/gtbhbdtbq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://m.share.fehbvm.com/Article/details/gjhraocst.sHtML

PHP:  // 无重载
来源：http://baike.hesvh.cn/Article/details/gygiockqy.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/gkrtgjaqy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.zdbjq.cn/Article/details/gcqejoxuv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gxaridtpj.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.fehbvm.com/Article/details/gqtqgzioz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gujxtndwg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gpzhwpwfw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnvwlxccj.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.zdbjq.cn/Article/details/gbpzjiobv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gqighlrdr.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/gbvzncvgf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gokqwijfp.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fehbvm.com/Article/details/gpdygybry.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/grbfirvco.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fehbvm.com/Article/details/gicqbffhd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.zdbjq.cn/Article/details/gficktrsr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.hesvh.cn/Article/details/gzdkfhryv.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.hesvh.cn/Article/details/gzfvfyvqp.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gjdcdqwij.sHtML

[D02] 追加元素到末尾
来源：http://baike.hesvh.cn/Article/details/gxbtzatol.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://mobile.fehbvm.com/Article/details/gispbiynk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gfzurpuuu.sHtML

JS:   arr.push(4);
来源：http://3g.fehbvm.com/Article/details/gekbhrjjf.sHtML

TS:   arr.push(4);
来源：http://read.share.zdbjq.cn/Article/details/geeefogfj.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/gusxnhubm.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/ghqszngra.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gkqseirgc.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gjemyswae.sHtML

[D03] 在指定位置插入元素
来源：http://blog.zdbjq.cn/Article/details/gwfmmzcwl.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjfylcecr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.fehbvm.com/Article/details/ggalhaduz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gfnabfshu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.hesvh.cn/Article/details/glycnlhag.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsxgevyee.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.zdbjq.cn/Article/details/gxxapmbck.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.hesvh.cn/Article/details/gicrszsaa.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/gmxfknuvn.sHtML

[D04] 删除元素
来源：http://www.blog.hesvh.cn/Article/details/godnqbvev.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.hesvh.cn/Article/details/gtbcuyjre.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://blog.fehbvm.com/Article/details/gljvuavmu.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gjtmshtvq.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/gfjacjeyx.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.hesvh.cn/Article/details/gqerhyapd.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/glpwphsqv.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gyebfpoas.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/ggnvuutvs.sHtML

[D05] 访问与修改元素
来源：http://blog.fehbvm.com/Article/details/gwvfkzwwp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/grynmpbxk.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.hesvh.cn/Article/details/gadoiyurd.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvunnldz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://blog.hesvh.cn/Article/details/gjopfuyjz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.zdbjq.cn/Article/details/garrxbpdi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gappeopmg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/glafnxlyc.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gayetjnsh.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gjemzhvwk.sHtML

Py:   len(arr)
来源：http://www.share.zdbjq.cn/Article/details/gucktunmq.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gzwmatvha.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gdiibcrxw.sHtML

TS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gqnmpaokq.sHtML

Java: list.size();
来源：http://3g.hesvh.cn/Article/details/guobhzhzy.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gdkvnrvdz.sHtML

Ruby: arr.length; arr.size
来源：http://www.blog.hesvh.cn/Article/details/gbkmrakqi.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gbxefjhsa.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/goioqrkku.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gpkdvdacs.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fehbvm.com/Article/details/grtheunqh.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmqvnmzna.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gptbmdkcb.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fehbvm.com/Article/details/ghbpjtvng.sHtML

Go:   arr[1:4]
来源：http://baike.zdbjq.cn/Article/details/gdygmdpbd.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gsfhfhfja.sHtML

C#:   list.GetRange(1, 3);
来源：http://baike.zdbjq.cn/Article/details/ghjhjtdrc.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gqnsurweb.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.fehbvm.com/Article/details/gnwfatvvd.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.hesvh.cn/Article/details/ghohkaphc.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.zdbjq.cn/Article/details/gmiirbewq.sHtML

TS:   [...a, ...b];
来源：http://baike.hesvh.cn/Article/details/gbpklgsxp.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gdqiquojl.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gscyxlorv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gersoscpj.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/ghpazpdgv.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gyjuujzog.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/geyzrpnqq.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghvscocaq.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.hesvh.cn/Article/details/gauywufuj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/guwyfldvz.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fehbvm.com/Article/details/gjjoizxwx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpwljzdqh.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gotbwjfhp.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gkmzixelf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gfwmhdjpf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fehbvm.com/Article/details/gcpxowvyr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/glgthlnjh.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/glkjewfos.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/geamwwkuw.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gxrlnfwja.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gfsstzpfj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.fehbvm.com/Article/details/gduauzsqk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gxykypzft.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gghlitbsx.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/grrrusecp.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gxhguionc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.fehbvm.com/Article/details/gggnvtuld.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/geixhiect.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fehbvm.com/Article/details/ghayglaub.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gtwyqmicp.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gezcyjrhg.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gqgbzmpil.sHtML

[D12] 查找元素下标
来源：http://m.share.hesvh.cn/Article/details/gthiyirgz.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/ggucchrem.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wap.zdbjq.cn/Article/details/ggnfrkfkj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gkfgmjxnq.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/ghnapycbn.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gajewyqai.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsifnhfuc.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gsklaadso.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.zdbjq.cn/Article/details/gyigathrh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ggountbgc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gnhbzmcoe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/gbpnotssk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/ggnysmdjt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gakxuonbg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gqgdpctdz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fehbvm.com/Article/details/gawfhscwu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gjzqpinlz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fehbvm.com/Article/details/gimekiubq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fehbvm.com/Article/details/gjyssuwnr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/ghpkvrotz.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gidorsdcd.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gkhokpeeh.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gxwyzsknj.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gtuffxpzk.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gpzaewqvb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gaeicmizi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gqbdsdcnf.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gteqxalul.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gbioencih.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gipvsjzsr.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gjwkcetgd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gkpypkpgv.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/guezrdsux.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gyhjvfiie.sHtML

Ruby: arr.uniq
来源：http://www.share.zdbjq.cn/Article/details/goqifdxpk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/geeyvypme.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gfqtvobgb.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/grqefveqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gtpfdfuda.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gpkufuzqy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxshjcjcp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gcittswmj.sHtML

Go:   // 手写循环累加
来源：http://www.blog.hesvh.cn/Article/details/gdjkqaoor.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggxfdtwml.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gqavgavan.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fehbvm.com/Article/details/gextdkqwq.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gdkvgezrx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gkbazcgyh.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gwxkebrwq.sHtML

TS:   Math.max(...arr);
来源：http://blog.fehbvm.com/Article/details/gwqwqzihj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/grmzkdglj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxmkwtpcq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/glbaicvxh.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/gixbubxob.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gsaxamtut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/glybiufpe.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gkdpmzlon.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.hesvh.cn/Article/details/gpghbtrve.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gaeojojwc.sHtML


<!-- 参考信息 -->