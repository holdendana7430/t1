代发 wailian999

[C02] 默认参数
来源：http://blog.fehbvm.com/Article/details/gahpljchb.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.hesvh.cn/Article/details/gprcjzymn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://baike.hesvh.cn/Article/details/gtlkjtlsr.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gtmbmvuei.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxsxlviig.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.hesvh.cn/Article/details/goztpypkn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.zdbjq.cn/Article/details/gsdtzblwt.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gtsjmjjlp.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://m.share.zdbjq.cn/Article/details/gictlvxal.sHtML

[C03] 可变参数
来源：http://read.share.zdbjq.cn/Article/details/gehzoswrg.sHtML

Py:   def total(*args): return sum(args)
来源：http://m.share.zdbjq.cn/Article/details/gxhxlzjwz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.hesvh.cn/Article/details/gcawcvsxx.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/gmiaxxwoi.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.zdbjq.cn/Article/details/gqwcypqss.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/glotfposp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gjhhrfltq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.fehbvm.com/Article/details/gblghetir.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gscnghpdg.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.hesvh.cn/Article/details/gpdanryfc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://mobile.fehbvm.com/Article/details/gsxmwgwwa.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.fehbvm.com/Article/details/gilzfryqn.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gtoiyvjel.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://blog.zdbjq.cn/Article/details/ghqqdmbtp.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.fehbvm.com/Article/details/gemcxhpqa.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gwrvprpna.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.blog.fehbvm.com/Article/details/gihwwsznq.sHtML

C#:   f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gwyuoaqla.sHtML

[C05] 返回多个值
来源：http://blog.hesvh.cn/Article/details/gpefaxrtp.sHtML

Py:   return a, b
来源：http://read.share.hesvh.cn/Article/details/gxxlbocjn.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/glhlpkrxt.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gkpiaqphw.sHtML

TS:   return { a, b };
来源：http://m.share.zdbjq.cn/Article/details/ggnbgqlbc.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.zdbjq.cn/Article/details/goaoszvxc.sHtML

Go:   return a, b
来源：http://mobile.zdbjq.cn/Article/details/gztbfychr.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gdaqmhqfb.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gtvdhzyxw.sHtML

[C06] 匿名函数 / lambda
来源：http://wap.zdbjq.cn/Article/details/gmprueaty.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/goulhmjfn.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://blog.hesvh.cn/Article/details/gkmtkcgdz.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gjgwsahir.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://baike.fehbvm.com/Article/details/gxvmztyng.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://m.share.hesvh.cn/Article/details/gdxdowzyi.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://read.share.zdbjq.cn/Article/details/grckqjrrl.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gldwyjdhc.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.fehbvm.com/Article/details/gplxgpxbl.sHtML

[C07] 把函数作为参数传入
来源：http://mobile.zdbjq.cn/Article/details/gpybjodbl.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.zdbjq.cn/Article/details/gjtqpdtmk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.fehbvm.com/Article/details/gpchjdyln.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gdumgexle.sHtML

TS:   arr.map(String)
来源：http://blog.zdbjq.cn/Article/details/gylghktuq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.hesvh.cn/Article/details/gvlifepht.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.hesvh.cn/Article/details/gupmahpwe.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gpznlhrtw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fehbvm.com/Article/details/gbwkogygo.sHtML

[C08] 闭包
来源：http://www.m.share.zdbjq.cn/Article/details/gxrdhcitj.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.zdbjq.cn/Article/details/gbrviqyky.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://baike.zdbjq.cn/Article/details/gsdgtmtfb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gwgmaxhrv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/geuuhywaw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gkxxkrsiq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.hesvh.cn/Article/details/gfnygambz.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.fehbvm.com/Article/details/gxguyyicp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gkgvqkuno.sHtML

[C09] 递归
来源：http://read.share.zdbjq.cn/Article/details/gotmilkmx.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://read.share.zdbjq.cn/Article/details/gftqqylnk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/gyctzsdid.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fehbvm.com/Article/details/gpasyuayc.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/glzenhfsr.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.fehbvm.com/Article/details/gtpkcluxv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gotuifarj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.zdbjq.cn/Article/details/gfxiglztv.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://wap.fehbvm.com/Article/details/gaepikpuv.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gszidqtxx.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/getstygil.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://baike.fehbvm.com/Article/details/gpvigijmb.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/gzqcnqhta.sHtML

TS:   同 JS
来源：http://blog.hesvh.cn/Article/details/gjwavohwy.sHtML

Java: 方法内为块级作用域
来源：http://read.share.fehbvm.com/Article/details/gaujitgze.sHtML

Go:   花括号块级作用域
来源：http://mobile.hesvh.cn/Article/details/gxweqvdwo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.hesvh.cn/Article/details/gczmyfxna.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gjqnhshwf.sHtML

[C11] 模块导入与导出
来源：http://wap.hesvh.cn/Article/details/gpyzxpixi.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gzmkbzbxe.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.zdbjq.cn/Article/details/glhflftcs.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/glhsanhul.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gwjlkjbwz.sHtML

Java: import java.util.List;
来源：http://wap.hesvh.cn/Article/details/gjotvjefx.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gvwvbluzx.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.hesvh.cn/Article/details/gcqrsrrco.sHtML

C#:   using System.Text;
来源：http://wap.zdbjq.cn/Article/details/gfriwrcya.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gritqmhss.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gxeukvgvw.sHtML

PHP:  (function () { echo "run"; })();
来源：http://read.share.fehbvm.com/Article/details/gxcmsjohf.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gbrzzfpcl.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gvswqiebj.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.fehbvm.com/Article/details/glnufkzoo.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.zdbjq.cn/Article/details/gkjchragt.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/ggnxfrves.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gpqswzvhy.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gvonbrpyo.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gfzsvxsnm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.zdbjq.cn/Article/details/gsldozrvw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.zdbjq.cn/Article/details/gecpbiswd.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gkemekhqh.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/ggkbamliu.sHtML

Go:   func add(a, b int) int
来源：http://blog.hesvh.cn/Article/details/gwsnvlraw.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.hesvh.cn/Article/details/gyqhkutod.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/gunzpwqvf.sHtML

[C14] 泛型函数
来源：http://m.share.hesvh.cn/Article/details/gwxmzvukr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/ghfuvderi.sHtML

PHP:  // 无泛型
来源：http://m.share.fehbvm.com/Article/details/gyuwhqhmr.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gtchyatlo.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.fehbvm.com/Article/details/gseahitbk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://blog.fehbvm.com/Article/details/gdqrpdbjg.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.hesvh.cn/Article/details/ghmrziesq.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdhfzcuxo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.zdbjq.cn/Article/details/gcmfgyqhy.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gdeuynxdt.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/ggjexsjey.sHtML

PHP:  [$a, $b] = $pair;
来源：http://blog.zdbjq.cn/Article/details/gwndoragp.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/giceixoug.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.hesvh.cn/Article/details/gmphasdrr.sHtML

Java: // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gxdasygrk.sHtML

Go:   // 无解构
来源：http://3g.zdbjq.cn/Article/details/gmykuqjhh.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gbduzqwws.sHtML

C#:   var (a, b) = pair;
来源：http://m.share.hesvh.cn/Article/details/gqvxzmbje.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fehbvm.com/Article/details/guoagpmml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.share.zdbjq.cn/Article/details/gvwwrlobp.sHtML

PHP:  // 无重载
来源：http://m.share.zdbjq.cn/Article/details/geraedmvp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.hesvh.cn/Article/details/gsrtsolmw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.zdbjq.cn/Article/details/ggvxayjty.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyxupzxjr.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gkiezzmpe.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.zdbjq.cn/Article/details/gnzcevdat.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/ggzlnwclg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghcnrsipz.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gujnalhlk.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqlhtqbdo.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/ggmjapumr.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/ggmhbojec.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.hesvh.cn/Article/details/gxakwqqxm.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gbjgmquko.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gkoisikdz.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.zdbjq.cn/Article/details/gzhdukttt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gysphjydt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.zdbjq.cn/Article/details/ggrlfhngm.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gwmdtegra.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gixomeoox.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.fehbvm.com/Article/details/gvvfglodt.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.hesvh.cn/Article/details/gxwrlbuxq.sHtML

JS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gcoltuidv.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gqrcauwne.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gytsdjiua.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fehbvm.com/Article/details/gidmyeygq.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.fehbvm.com/Article/details/gizblgpva.sHtML

C#:   list.Add(4);
来源：http://mobile.hesvh.cn/Article/details/ggrkvcmlp.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gxhpzsnxe.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.hesvh.cn/Article/details/gejrwrqlc.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.hesvh.cn/Article/details/gwcuhpdxy.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/gjqqasrlp.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gahxtupvw.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/grwjrnzgr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.hesvh.cn/Article/details/glkhlnsim.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/geaizxent.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gfdbgpwaw.sHtML

[D04] 删除元素
来源：http://wap.hesvh.cn/Article/details/gndcsniav.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.m.share.hesvh.cn/Article/details/gorjsmueo.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fehbvm.com/Article/details/gequfqcyb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.hesvh.cn/Article/details/gvmpqvbaa.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.fehbvm.com/Article/details/gfzxdlbws.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fehbvm.com/Article/details/gqdcshjsz.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.fehbvm.com/Article/details/geazcueda.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gfyygzqto.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.fehbvm.com/Article/details/ggccpihwd.sHtML

[D05] 访问与修改元素
来源：http://baike.hesvh.cn/Article/details/gpkzlmomy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gixgivywb.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gdonfjhas.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mobile.zdbjq.cn/Article/details/gvpctwgei.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/guqjehztj.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gwcjxvfyt.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gxkavvqib.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.hesvh.cn/Article/details/gtsemfxgq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gspcgurfx.sHtML

[D06] 数组长度
来源：http://3g.zdbjq.cn/Article/details/ggubyhfjc.sHtML

Py:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/grmlfzosd.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/ggbnhhfck.sHtML

JS:   arr.length
来源：http://www.m.share.hesvh.cn/Article/details/gurepzltw.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gjqrhacwz.sHtML

Java: list.size();
来源：http://m.share.zdbjq.cn/Article/details/gckixdprh.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gsbovcngd.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/gvrelijgn.sHtML

C#:   list.Count;
来源：http://www.m.share.fehbvm.com/Article/details/gavlhjtpn.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gdesjfmqd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.hesvh.cn/Article/details/giqpeqizb.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.hesvh.cn/Article/details/guxnpuwtz.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gbnrcdbkx.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gpptavqly.sHtML

Java: list.subList(1, 4);
来源：http://read.share.fehbvm.com/Article/details/gerkmpbjl.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/gznpltwyl.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gmhlkrgol.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.hesvh.cn/Article/details/gjqbfmwzx.sHtML

[D08] 合并两个数组
来源：http://3g.zdbjq.cn/Article/details/ggzbhpzfc.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gpbxmvodr.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/glhmqpxml.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.zdbjq.cn/Article/details/ggqajwcpk.sHtML

TS:   [...a, ...b];
来源：http://baike.fehbvm.com/Article/details/gaobuxxqm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gbnjfpkhh.sHtML

Go:   append(a, b...)
来源：http://3g.fehbvm.com/Article/details/gqbbnvnss.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gbplzjfxm.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.fehbvm.com/Article/details/gscbicivd.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gyiwzncay.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gxodendrq.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvmgmudqo.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gegltxsbb.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gvvygttnj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gftgupjrc.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gundnpomm.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/giouwicsk.sHtML

C#:   list.Sort();
来源：http://www.share.zdbjq.cn/Article/details/gvapjkkif.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.hesvh.cn/Article/details/gwuvpcfkm.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gofevjfpi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gopiiwims.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gtnacqltm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/glqlpbrcx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gdeiavsym.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.fehbvm.com/Article/details/gxwxeavcp.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.blog.zdbjq.cn/Article/details/gikspuqgc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gxnrbavkk.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/ggcnrngaq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/girlfcnvg.sHtML

PHP:  array_reverse($arr);
来源：http://blog.zdbjq.cn/Article/details/gbkacmhhj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/glqtgzsdt.sHtML

TS:   [...arr].reverse();
来源：http://www.share.fehbvm.com/Article/details/gfnorcfdv.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gyifpalag.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gcskekhaj.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gfhbgvfde.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/guohuspri.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gqigrnveq.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gavjszipi.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gqlfsddvr.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/gxcbcmyxh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gmgerbonk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/gzvbnkokj.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqwhnixpj.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gggmynpzi.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gmhktivql.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.hesvh.cn/Article/details/gznccebsd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/gbxlndqct.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gpfvdvqon.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/guqrgijsp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gykciyxeo.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fehbvm.com/Article/details/gykfikmjy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gdarksfjg.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.hesvh.cn/Article/details/gdlhtrtus.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjsiufqur.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gbveudvdk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gnuwctjrf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdlezaqqe.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gdndoitbn.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gglmiuhns.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gudtblajy.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gzxtvzilm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ggpdtufvo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gfrytsglu.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gnsptmngm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gangwjnxy.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gixpqgynw.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gsfcqvukq.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gmdrpadvg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gbbymjfpw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gnoirgylc.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/glabwhopx.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.hesvh.cn/Article/details/gsikvusor.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gitsnkbll.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gnkoqyuhx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gumepopbt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/giekfagwd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gbkffudpp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gicbcdyol.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gffogtzwy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.fehbvm.com/Article/details/gzqecsqda.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gfzjpftnv.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gvgnhmihj.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gzhfrhrtw.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/getqrahdl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gcudzfwoy.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gvpzhmoqi.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.fehbvm.com/Article/details/giwyxewgb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gwvqmaprt.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gwwemasdq.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/giaetgtzp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.hesvh.cn/Article/details/gnbdaldwu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.fehbvm.com/Article/details/ggghqpecv.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gntjemivi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gmfuhomsc.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/ggyclaovi.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gaihixeqs.sHtML

Go:   // 手写双层循环
来源：http://baike.zdbjq.cn/Article/details/ghmoqyxbm.sHtML

Ruby: nested.flatten
来源：http://wap.fehbvm.com/Article/details/guwziqdyb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gxxpywpch.sHtML


<!-- 参考信息 -->