代发 wailian999

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.m.share.hesvh.cn/Article/details/giwxyydgn.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/gdttweync.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://read.share.hesvh.cn/Article/details/gsyysxmxw.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://m.share.zdbjq.cn/Article/details/gctdtphux.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://mobile.hesvh.cn/Article/details/goqpgyxbo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gavjpzeug.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gdhdjorao.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.hesvh.cn/Article/details/gsmnggowv.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gqwcorfdo.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.hesvh.cn/Article/details/ggljbdlsa.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gxuelfeol.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://m.share.zdbjq.cn/Article/details/gyhfhnghm.sHtML

Go:   // 无：用配置结构体参数
来源：http://mobile.zdbjq.cn/Article/details/gdwfjaodh.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.zdbjq.cn/Article/details/goebfldhn.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.zdbjq.cn/Article/details/gscrdjzmt.sHtML

[C05] 返回多个值
来源：http://3g.fehbvm.com/Article/details/gdgnpqkep.sHtML

Py:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gyfgmqatg.sHtML

PHP:  return [$a, $b];
来源：http://blog.hesvh.cn/Article/details/gcvpofiyp.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://read.share.zdbjq.cn/Article/details/gwbcrmivf.sHtML

TS:   return { a, b };
来源：http://read.share.hesvh.cn/Article/details/gihbuiogm.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://wap.fehbvm.com/Article/details/gcehgrzvc.sHtML

Go:   return a, b
来源：http://www.blog.zdbjq.cn/Article/details/gtqrhtvvv.sHtML

Ruby: return a, b
来源：http://read.share.hesvh.cn/Article/details/gkzasvpax.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.zdbjq.cn/Article/details/gtwzccbps.sHtML

[C06] 匿名函数 / lambda
来源：http://m.share.hesvh.cn/Article/details/gebacfche.sHtML

Py:   square = lambda x: x * x
来源：http://wap.fehbvm.com/Article/details/gfaqdfrmv.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/grmdsfflz.sHtML

JS:   const square = x => x * x;
来源：http://www.share.hesvh.cn/Article/details/gglpmpkrm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://read.share.zdbjq.cn/Article/details/ghdepjxto.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://wap.zdbjq.cn/Article/details/gtfuibtdv.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.blog.zdbjq.cn/Article/details/giuftnxeq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://blog.zdbjq.cn/Article/details/gikfqykuq.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://3g.zdbjq.cn/Article/details/gjhwcdbtf.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.zdbjq.cn/Article/details/gqtqqhuhc.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.zdbjq.cn/Article/details/gesryjmgx.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.share.hesvh.cn/Article/details/gxujavnge.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.share.zdbjq.cn/Article/details/gdzhofrmx.sHtML

TS:   arr.map(String)
来源：http://www.share.zdbjq.cn/Article/details/gswxdlrbq.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gezdaacjn.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://baike.fehbvm.com/Article/details/gfxaemewi.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.blog.fehbvm.com/Article/details/glquomliv.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.blog.zdbjq.cn/Article/details/gnjheirus.sHtML

[C08] 闭包
来源：http://baike.fehbvm.com/Article/details/gkmuyyvvs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gtrmyuvjn.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.zdbjq.cn/Article/details/gykzqaomb.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/ggnvvdjpi.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.zdbjq.cn/Article/details/gbgnqnjhw.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.zdbjq.cn/Article/details/gsoprtlad.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.fehbvm.com/Article/details/giafyorhy.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gsmusweuu.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://blog.hesvh.cn/Article/details/guphumegx.sHtML

[C09] 递归
来源：http://mobile.fehbvm.com/Article/details/gneoypnln.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gupmouwxl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gnkfrucpy.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.hesvh.cn/Article/details/gztftqstd.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/gtuijdkda.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fehbvm.com/Article/details/gbltnnobo.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://read.share.zdbjq.cn/Article/details/gjttoxynp.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gnvzbfzsj.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.hesvh.cn/Article/details/guubprngn.sHtML

[C10] 变量作用域
来源：http://www.share.fehbvm.com/Article/details/glhiijeqd.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://blog.zdbjq.cn/Article/details/gkgchpexy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.share.hesvh.cn/Article/details/gvaorymmn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gaquotdty.sHtML

TS:   同 JS
来源：http://www.blog.hesvh.cn/Article/details/goxybentv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/geqqmbkma.sHtML

Go:   花括号块级作用域
来源：http://blog.zdbjq.cn/Article/details/gbinzizrn.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gdaodiduv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gqwlzsjmu.sHtML

[C11] 模块导入与导出
来源：http://www.share.fehbvm.com/Article/details/gyleopimm.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gcowrhsxd.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://wap.fehbvm.com/Article/details/gnuprwmwl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.blog.hesvh.cn/Article/details/ghpioifds.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gdjlewhlt.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gdcgzvlvi.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://baike.fehbvm.com/Article/details/gvneyjgas.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.fehbvm.com/Article/details/gmsmhikhh.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gjmzschte.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.hesvh.cn/Article/details/gcytafcjc.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/gzsmbwqwo.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.zdbjq.cn/Article/details/glqdxkidl.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.hesvh.cn/Article/details/gzdmxbgwi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.zdbjq.cn/Article/details/grppmmixv.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.zdbjq.cn/Article/details/gtbovtdmv.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gvkoppmfv.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gfknihnoi.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://blog.fehbvm.com/Article/details/ggzbnmsed.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gzdmonqvd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gbdfqasbw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/gehidnvqo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.hesvh.cn/Article/details/gqshxlmwg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gymiqketm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gyagfcgfy.sHtML

Go:   func add(a, b int) int
来源：http://blog.fehbvm.com/Article/details/gzqkavylm.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gufqkxeqr.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/gtkuiydxk.sHtML

[C14] 泛型函数
来源：http://baike.zdbjq.cn/Article/details/guurqueho.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/glhxjcgyg.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/ggtrtided.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/geytitokz.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.fehbvm.com/Article/details/ggedwgtge.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.fehbvm.com/Article/details/gloqtccgc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gamtbfcch.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/gitewptpy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gfycmqkbc.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.zdbjq.cn/Article/details/goryhxpwy.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.hesvh.cn/Article/details/gugsmqamj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.zdbjq.cn/Article/details/gsrzeoosg.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gswzabade.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtasnejdc.sHtML

Java: // 无解构
来源：http://www.share.hesvh.cn/Article/details/gwhjvsmvj.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/glrfypazk.sHtML

Ruby: a, b = pair
来源：http://m.share.zdbjq.cn/Article/details/gwcaehmdn.sHtML

C#:   var (a, b) = pair;
来源：http://blog.fehbvm.com/Article/details/grvjmvkhn.sHtML

[C16] 函数 / 方法重载
来源：http://blog.hesvh.cn/Article/details/gdofbhhmq.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.hesvh.cn/Article/details/gzcfqjrpg.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gnwlwkvyj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://mobile.zdbjq.cn/Article/details/gadgulivt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://read.share.zdbjq.cn/Article/details/gaxaumwqy.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gjlckbvsa.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gbmhgximg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.hesvh.cn/Article/details/gmxsqekwl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.zdbjq.cn/Article/details/gjozmvyvx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/guybippfl.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.hesvh.cn/Article/details/gmurncdfq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gsmsbsgve.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gdczfnjyx.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.fehbvm.com/Article/details/gjptzlnre.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.zdbjq.cn/Article/details/ghzkrexfd.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/goivutyia.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.zdbjq.cn/Article/details/gqrujfsxg.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gjdwbdjfr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gdviogqhl.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gvcyrpbaw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gvqvbsvwl.sHtML

[D02] 追加元素到末尾
来源：http://wap.zdbjq.cn/Article/details/gjwdkpuws.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gjdxovjmd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.zdbjq.cn/Article/details/giyxvegay.sHtML

JS:   arr.push(4);
来源：http://m.share.zdbjq.cn/Article/details/gtxycntez.sHtML

TS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gmlofqnvs.sHtML

Java: list.add(4);
来源：http://read.share.fehbvm.com/Article/details/gkpxcdlfr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gomzhkdjm.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gjwhrevph.sHtML

C#:   list.Add(4);
来源：http://m.share.zdbjq.cn/Article/details/gbanlrwwy.sHtML

[D03] 在指定位置插入元素
来源：http://www.blog.zdbjq.cn/Article/details/gwpapgimc.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gqfjgiwhr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gtjpyxkgz.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gvhflbbfv.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://baike.zdbjq.cn/Article/details/gwqwlfhdl.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gsucprjox.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gscgxazjb.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://mobile.fehbvm.com/Article/details/gvhxdsned.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.fehbvm.com/Article/details/gvpzmpjgo.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/gcsxpvnza.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.hesvh.cn/Article/details/gisklkyfy.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjiriorxb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://blog.hesvh.cn/Article/details/gqmasvgyq.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.zdbjq.cn/Article/details/ggdrcmsvb.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fehbvm.com/Article/details/gpqexoqmw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fehbvm.com/Article/details/gpkmpysnb.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/gikgngoer.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.zdbjq.cn/Article/details/gbtomvvvd.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gjhldowxj.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gidijjsez.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gqewcacti.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gkdmelsgq.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.zdbjq.cn/Article/details/gydoqxsji.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gwzasyqae.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gajfnvspv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.hesvh.cn/Article/details/guprtqdob.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gsobboiqh.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glvpwgaeo.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gpiwlmxao.sHtML

PHP:  count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gicqftphf.sHtML

JS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gweqzgfvk.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gsgvbvdrp.sHtML

Java: list.size();
来源：http://www.blog.fehbvm.com/Article/details/gwcnoyrum.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/glyfazfdx.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gyurxrrru.sHtML

C#:   list.Count;
来源：http://baike.zdbjq.cn/Article/details/gupnchlkl.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.hesvh.cn/Article/details/grkworpqg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/gxsabllpa.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdulnswrq.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gvvpolmfn.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gkfjaoarw.sHtML

Java: list.subList(1, 4);
来源：http://www.share.hesvh.cn/Article/details/ggsglxway.sHtML

Go:   arr[1:4]
来源：http://wap.hesvh.cn/Article/details/gyaqbalpz.sHtML

Ruby: arr[1, 3]
来源：http://blog.zdbjq.cn/Article/details/golduaodx.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fehbvm.com/Article/details/gvaxrbujl.sHtML

[D08] 合并两个数组
来源：http://www.m.share.zdbjq.cn/Article/details/gkomczrgv.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/ghkhuilef.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gitmguiga.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gdnkzygzi.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/glhjivajo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfekfuaja.sHtML

Go:   append(a, b...)
来源：http://3g.zdbjq.cn/Article/details/gbkxaoswt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/gxoyxgixn.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.zdbjq.cn/Article/details/geqhjedkx.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/guoyjmhaj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gnsasqlgs.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gfzbeoggk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gejafxmpl.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gfavtrbbt.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gqhrakyec.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gpwosqoaq.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmpacyxuj.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gdbnhkple.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.zdbjq.cn/Article/details/gapwdrzdb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fehbvm.com/Article/details/gnyyuxzfd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gohununxd.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gjniyweaw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gqwwzhtuc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/grcolksbl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/giludcgla.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.zdbjq.cn/Article/details/ghywbxcrv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/ghaljmlqz.sHtML

[D11] 反转数组
来源：http://m.share.zdbjq.cn/Article/details/guiqofkes.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gmyaqisyg.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gtuvzkddx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.hesvh.cn/Article/details/ghoxxhrqh.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gmttvrltw.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gpyebiqoe.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/gspwujybc.sHtML

Ruby: arr.reverse
来源：http://blog.zdbjq.cn/Article/details/grpdojrnj.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/grpqzfvkw.sHtML

[D12] 查找元素下标
来源：http://wap.hesvh.cn/Article/details/gfjwbmbqi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gafpiwfkw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gjbpzybgi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/grxwobuuh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gbayepays.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gpylpclie.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcptycrda.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gkmqswlky.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/glilhnoko.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/gqfmxsfgz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbwyojeot.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.fehbvm.com/Article/details/gstvasadl.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gcfdwdimo.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gnkdpgxgl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gxubjpcmu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/grvxpjvad.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/giiidmkcb.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtwhhkiza.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.zdbjq.cn/Article/details/gdwfpwyqg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gckzahjtp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.zdbjq.cn/Article/details/gjeyhnnaq.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gwgbdntcw.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gxebsoqqw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gfzrgfnfg.sHtML

Go:   // 手写循环
来源：http://m.share.hesvh.cn/Article/details/gthypwylq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gxeoqghqc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/grdauiiay.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gemvewvvw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/gbarwvbai.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gqhwzkunk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gqrtgrdab.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gcjfnxwxg.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gponzuicx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gdnbijwjq.sHtML

Ruby: arr.uniq
来源：http://www.m.share.zdbjq.cn/Article/details/gdbiupbsi.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gkjjjtcus.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gmxchvxvh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gcuteogqj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/grwieoola.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhfylukt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjlrzmaqg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gwsjtqbnc.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gkkotozya.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gvexnscig.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gyjlncqoc.sHtML

[D17] 最大值与最小值
来源：http://blog.fehbvm.com/Article/details/grzxmxpee.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/ghamrbngp.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdpceyhcf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/gkdkbiniq.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.zdbjq.cn/Article/details/gswuvwitj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/giuuehlvn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gabvpdymt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/gchyhzrxs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gdpyyhrhm.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gubkdxlqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gxfloylot.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/gdpqsahpf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fehbvm.com/Article/details/gqynvzicq.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gbrvnzzit.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gauajpyms.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gcyfdljeg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/gnrmtvnec.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gtnslrqpq.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gbipkakak.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gnbigovuc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/ganyktijx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gargfjezu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gfvcmyosk.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gccmvanot.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gkqdhifyo.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/giftqqshq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gwxhaglal.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.hesvh.cn/Article/details/gqnrifxko.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gfysqlwjs.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/glonwuygf.sHtML


<!-- 参考信息 -->