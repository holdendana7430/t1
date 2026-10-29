代发 wailian999

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gmmhhwgru.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.fehbvm.com/Article/details/geovkasuy.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.fehbvm.com/Article/details/gbovqiamw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/glvlfytyi.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gqmqhwpbp.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.hesvh.cn/Article/details/gtnnwljoz.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.fehbvm.com/Article/details/gywyvwxrc.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gdbnulhyc.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gogbnbofk.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.zdbjq.cn/Article/details/gddirycyl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gpapnijyn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gdowjnrhi.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.hesvh.cn/Article/details/gbtduvkdl.sHtML

[C03] 可变参数
来源：http://www.m.share.fehbvm.com/Article/details/gitfooqtw.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.zdbjq.cn/Article/details/gezonspiz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gnpzxqtvd.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://mobile.fehbvm.com/Article/details/ggiwdinsw.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/govcawvje.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.fehbvm.com/Article/details/ggfblxrio.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.share.hesvh.cn/Article/details/gqfymwbfu.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gfisnuvqw.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.hesvh.cn/Article/details/gxgqbghst.sHtML

[C04] 命名参数 / 关键字参数
来源：http://wap.zdbjq.cn/Article/details/gsscbbfuc.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/govpjumii.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.share.zdbjq.cn/Article/details/gbbtjhrnt.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gdtywxmlf.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gxnukiivz.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://wap.zdbjq.cn/Article/details/gsrvjkxwn.sHtML

Go:   // 无：用配置结构体参数
来源：http://www.m.share.hesvh.cn/Article/details/gzuybsnxr.sHtML

Ruby: f(a: 1, b: 2)
来源：http://www.share.fehbvm.com/Article/details/gphktgjgl.sHtML

C#:   f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/grrylxsey.sHtML

[C05] 返回多个值
来源：http://www.m.share.zdbjq.cn/Article/details/gpwrxwtdo.sHtML

Py:   return a, b
来源：http://www.blog.fehbvm.com/Article/details/gfhxpulbg.sHtML

PHP:  return [$a, $b];
来源：http://read.share.zdbjq.cn/Article/details/grtewhomq.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/gryuinprz.sHtML

TS:   return { a, b };
来源：http://3g.fehbvm.com/Article/details/gcxdbguvr.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.hesvh.cn/Article/details/gpqnoavwa.sHtML

Go:   return a, b
来源：http://www.m.share.zdbjq.cn/Article/details/gjlgahmya.sHtML

Ruby: return a, b
来源：http://read.share.fehbvm.com/Article/details/gglmfwtny.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://blog.fehbvm.com/Article/details/gyqcpzjve.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gncmvfglg.sHtML

Py:   square = lambda x: x * x
来源：http://mobile.zdbjq.cn/Article/details/gbssurgpy.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://m.share.fehbvm.com/Article/details/gxfkfmhzk.sHtML

JS:   const square = x => x * x;
来源：http://wap.hesvh.cn/Article/details/gsoyselqi.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://3g.zdbjq.cn/Article/details/gjnmmdseg.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://baike.zdbjq.cn/Article/details/guygufoen.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.zdbjq.cn/Article/details/gzqgeskrp.sHtML

Ruby: square = ->(x) { x * x }
来源：http://wap.fehbvm.com/Article/details/gmunpxxok.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://www.m.share.fehbvm.com/Article/details/glwravvgs.sHtML

[C07] 把函数作为参数传入
来源：http://3g.hesvh.cn/Article/details/gkqzbivbm.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://m.share.fehbvm.com/Article/details/gpympunmk.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://mobile.hesvh.cn/Article/details/gjaccegvc.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.fehbvm.com/Article/details/gbpcyfbxp.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gywgndsnn.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.share.zdbjq.cn/Article/details/gcneuihsp.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.fehbvm.com/Article/details/ggywknrqb.sHtML

Ruby: arr.map(&:upcase)
来源：http://3g.fehbvm.com/Article/details/gjfjtuvay.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gwezannkk.sHtML

[C08] 闭包
来源：http://www.blog.hesvh.cn/Article/details/gqjfbhtzm.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.fehbvm.com/Article/details/grgneaozg.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fehbvm.com/Article/details/gejobyfko.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://m.share.fehbvm.com/Article/details/grfnhjnqa.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/gdwjbiybz.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.share.fehbvm.com/Article/details/gbdseovvh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gdemjvvhj.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.blog.zdbjq.cn/Article/details/gpxqjhgif.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gsxvocwjz.sHtML

[C09] 递归
来源：http://www.share.zdbjq.cn/Article/details/glyknlnnj.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gdksuflax.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://3g.fehbvm.com/Article/details/gupswywwf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gqhpfebyn.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fehbvm.com/Article/details/ggqqnvmuz.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.zdbjq.cn/Article/details/gwqamdagd.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/gzuyfrsnj.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwfhmywqm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.zdbjq.cn/Article/details/gqzkzzckg.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/ggprotzlc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.hesvh.cn/Article/details/gkgsfibja.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.hesvh.cn/Article/details/gwjjmnjso.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.hesvh.cn/Article/details/gvvpclpwg.sHtML

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gtbcisbxf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gjwbonepr.sHtML

Go:   花括号块级作用域
来源：http://mobile.fehbvm.com/Article/details/gnrngqnde.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gbrfbzdzy.sHtML

C#:   块级作用域
来源：http://www.m.share.hesvh.cn/Article/details/grwvjddwl.sHtML

[C11] 模块导入与导出
来源：http://read.share.zdbjq.cn/Article/details/gapzkbaee.sHtML

Py:   from module import func
来源：http://www.blog.hesvh.cn/Article/details/gawawueuq.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.blog.zdbjq.cn/Article/details/gaodgkoes.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gjzvezoxm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://blog.hesvh.cn/Article/details/giwiqgore.sHtML

Java: import java.util.List;
来源：http://baike.zdbjq.cn/Article/details/gnqqmeyhq.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.fehbvm.com/Article/details/gfspcqjyn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gjdescyxg.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/gshosbrte.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gpsjgqdhd.sHtML

Py:   (lambda: print("run"))()
来源：http://www.m.share.zdbjq.cn/Article/details/gnptcwzrq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gmbbkltqk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gmqbsgelu.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gzzdbrimz.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.hesvh.cn/Article/details/gruzibkub.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.zdbjq.cn/Article/details/gnpcxbdwp.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/giqcktatb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.hesvh.cn/Article/details/gywdafwhw.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.zdbjq.cn/Article/details/gdxevuqvi.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/grbrwrtai.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.hesvh.cn/Article/details/gugccgtur.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.fehbvm.com/Article/details/gusfxnbro.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gisdgxbyx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/gzmebnwib.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/gpaqozlgx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.fehbvm.com/Article/details/gwwfnfdqf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.fehbvm.com/Article/details/gujrxwexe.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/ghfxmatww.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gltrwkvrt.sHtML

PHP:  // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gfoqwyfjv.sHtML

JS:   // 无泛型
来源：http://baike.fehbvm.com/Article/details/grmwpyfsa.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpjklbh.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.hesvh.cn/Article/details/gkfzyfnzm.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.fehbvm.com/Article/details/gijdbuswi.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/guckckdit.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gnxhkgkjc.sHtML

[C15] 解构 / 展开参数
来源：http://3g.hesvh.cn/Article/details/gdpwpartg.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.share.zdbjq.cn/Article/details/gzbbadlge.sHtML

PHP:  [$a, $b] = $pair;
来源：http://read.share.fehbvm.com/Article/details/gnmhbfzjt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gmxteskxu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gtukrczoc.sHtML

Java: // 无解构
来源：http://3g.zdbjq.cn/Article/details/goglcmqjn.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gmnhlcjzd.sHtML

Ruby: a, b = pair
来源：http://blog.fehbvm.com/Article/details/gzxnpfsyx.sHtML

C#:   var (a, b) = pair;
来源：http://3g.hesvh.cn/Article/details/gjdjlnxry.sHtML

[C16] 函数 / 方法重载
来源：http://wap.zdbjq.cn/Article/details/gjcqksvgz.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.hesvh.cn/Article/details/goxmhdwbb.sHtML

PHP:  // 无重载
来源：http://3g.zdbjq.cn/Article/details/gfnyzozaq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/ggvfegjuh.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/geanuqity.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.zdbjq.cn/Article/details/gwnmxixir.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gppxzbege.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/gjakaaacc.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gurrecsgt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbuvlgkjk.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/gqoybcjar.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzpbrrznz.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gyuybclul.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://m.share.hesvh.cn/Article/details/ggykexfoj.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gcvzmcewv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.hesvh.cn/Article/details/ghhembvku.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.hesvh.cn/Article/details/ghlhzgspj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gmodzmjsv.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.zdbjq.cn/Article/details/gcoeruggx.sHtML

Ruby: arr = [1, 2, 3]
来源：http://3g.zdbjq.cn/Article/details/gzckpuqld.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/gkvlqgshp.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gzgfmxbnw.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gkzoanfbd.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/ggfdfrcof.sHtML

JS:   arr.push(4);
来源：http://www.blog.fehbvm.com/Article/details/ggfihrnya.sHtML

TS:   arr.push(4);
来源：http://blog.hesvh.cn/Article/details/gmmmikoxn.sHtML

Java: list.add(4);
来源：http://baike.hesvh.cn/Article/details/ghbzpquvq.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gmctflefz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/gmtxagcgo.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gbkareobc.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.fehbvm.com/Article/details/gkzmyfosu.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpuzurkoy.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gxlqeexat.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gwkxodjme.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.zdbjq.cn/Article/details/grnevxxgv.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gowqwgcaf.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.fehbvm.com/Article/details/gsbulfxgw.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gwghemdfx.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.hesvh.cn/Article/details/ggcsbnxbj.sHtML

[D04] 删除元素
来源：http://blog.fehbvm.com/Article/details/gownwdyba.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gaxqnjzjk.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwotsvdtr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gszvhjwrz.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.hesvh.cn/Article/details/gcwdocvfi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gzcpzdjvm.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/grjqqnycm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.zdbjq.cn/Article/details/gmdzwpixl.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gmarvhpaa.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/golqxbhar.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gnscimymi.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gcdgckehi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gdpesnnjx.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fehbvm.com/Article/details/gojweellq.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gpelsquvp.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/grrlkdihh.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gosqhcomw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gintugwmh.sHtML

[D06] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/gfidawgcg.sHtML

Py:   len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gylvjirvm.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gkwnynaih.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpvbtcqko.sHtML

TS:   arr.length
来源：http://www.share.hesvh.cn/Article/details/gctklqyrn.sHtML

Java: list.size();
来源：http://wap.fehbvm.com/Article/details/gmmpdbqqy.sHtML

Go:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/gwzhnxwou.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.zdbjq.cn/Article/details/ghlomkfpl.sHtML

C#:   list.Count;
来源：http://baike.fehbvm.com/Article/details/gpiyrgpqy.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gneevagna.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/grdxjcpxj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gzhzfyota.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fehbvm.com/Article/details/gkxwzxqzw.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gvglieiev.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gvwwjlmll.sHtML

Go:   arr[1:4]
来源：http://m.share.zdbjq.cn/Article/details/gksdqjixt.sHtML

Ruby: arr[1, 3]
来源：http://www.share.zdbjq.cn/Article/details/gbrbqhggm.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/grrrekrhr.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/gyovvxdvm.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/gzlkaqggq.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gwftuytxs.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://baike.fehbvm.com/Article/details/goytgljsn.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/goaskewtr.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gttsynrfz.sHtML

Go:   append(a, b...)
来源：http://blog.fehbvm.com/Article/details/grhohxrxb.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.zdbjq.cn/Article/details/glpacetrv.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.hesvh.cn/Article/details/giucprltd.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/gfdcravzy.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gdtncunpq.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gorlzmwvp.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/gzavpzrni.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.fehbvm.com/Article/details/gnybbhbfs.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.zdbjq.cn/Article/details/gksotjlir.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gjskzvxwy.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gboeubvug.sHtML

C#:   list.Sort();
来源：http://www.m.share.zdbjq.cn/Article/details/gopnqjyjm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.zdbjq.cn/Article/details/gacmnekvr.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/glxjlfgwk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.hesvh.cn/Article/details/gbrrhvrva.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gaegiiskm.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/guiozhdcc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gngtchfvv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.fehbvm.com/Article/details/gmhtxwiol.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gfslfxypu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.fehbvm.com/Article/details/ggsieekio.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/galgphftk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gvrggnucn.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.fehbvm.com/Article/details/ghczsbxud.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/gqiaequwd.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fehbvm.com/Article/details/gtmybugou.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gguolaohc.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/ghyfaddvq.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/glkdhannm.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gldacvpjz.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gslbmscol.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gacidkdke.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/ggowbxoxe.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gdgkfaycw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gtvwqdtsb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/grvxcznro.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/guhlhezcm.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/gpsfcjvkn.sHtML

C#:   list.IndexOf(x);
来源：http://wap.hesvh.cn/Article/details/gmhjcqrem.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/guwqihwum.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gvkevdouy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gqcbpznve.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gmbofayrf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/ghrlihfnf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.hesvh.cn/Article/details/gobwzuskw.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gkzsqhuuz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.hesvh.cn/Article/details/gssxflkxe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.hesvh.cn/Article/details/geledylvs.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gflwvbvsh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gbmpmijwv.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfikbuylp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gmpeaoulp.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gfoqwibpw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.hesvh.cn/Article/details/gdnypetiz.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gpkklwedn.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gruvxlshb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gqkquqkfz.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/guyoyzbxm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvkzvmizd.sHtML

PHP:  array_unique($arr);
来源：http://blog.fehbvm.com/Article/details/gzslsemze.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/gbqsebvgo.sHtML

TS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gmmkcbpvc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gcknrnlsb.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.zdbjq.cn/Article/details/gwkpviwge.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gnemkbgeg.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gzhdtqlnj.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/guzpxdhei.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.hesvh.cn/Article/details/gkhvclfpf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmccnoifl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkflzjjfa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbjnayomo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/ggdculpmw.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/ggsueeola.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gvaogltqn.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/godxafekn.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/ghwdwprcr.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmvjfpapc.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/glpatnkge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fehbvm.com/Article/details/gornbqrsf.sHtML

TS:   Math.max(...arr);
来源：http://m.share.fehbvm.com/Article/details/gdbbecubu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gnmwvpxgc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.hesvh.cn/Article/details/ginaovigv.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gurdudjxh.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/giqtcpltf.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fehbvm.com/Article/details/gmxngockl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/grlpvernh.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.fehbvm.com/Article/details/gmhzxuxnx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gycvlobgv.sHtML

TS:   nested.flat();
来源：http://mobile.hesvh.cn/Article/details/golqnhosv.sHtML


<!-- 参考信息 -->