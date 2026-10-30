代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://www.share.hesvh.cn/Article/details/gbxjhtkky.sHtML

Ruby: f(a: 1, b: 2)
来源：http://read.share.hesvh.cn/Article/details/gfaqtybyz.sHtML

C#:   f(a: 1, b: 2)
来源：http://m.share.fehbvm.com/Article/details/gmojmusbv.sHtML

[C05] 返回多个值
来源：http://3g.hesvh.cn/Article/details/gielsnlrj.sHtML

Py:   return a, b
来源：http://wap.zdbjq.cn/Article/details/gahazllkt.sHtML

PHP:  return [$a, $b];
来源：http://m.share.zdbjq.cn/Article/details/gmompstwx.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://baike.fehbvm.com/Article/details/guegipjzo.sHtML

TS:   return { a, b };
来源：http://www.m.share.zdbjq.cn/Article/details/ggxoglokl.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.blog.zdbjq.cn/Article/details/gdiygogzr.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gbdhtwvfq.sHtML

Ruby: return a, b
来源：http://m.share.zdbjq.cn/Article/details/ggyyswrsu.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.blog.hesvh.cn/Article/details/ghblmxvkn.sHtML

[C06] 匿名函数 / lambda
来源：http://blog.zdbjq.cn/Article/details/gfenucszj.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/ggohfjpqc.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.m.share.hesvh.cn/Article/details/gabkqgith.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gfetygyvm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://blog.fehbvm.com/Article/details/ggzhmyluk.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.blog.zdbjq.cn/Article/details/glutmhvkl.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/grkavczjq.sHtML

Ruby: square = ->(x) { x * x }
来源：http://3g.fehbvm.com/Article/details/gbpikwnee.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gixsozhhx.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/gcrszwsty.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.share.hesvh.cn/Article/details/ggjpsxqme.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.blog.hesvh.cn/Article/details/ghikhlxki.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://read.share.zdbjq.cn/Article/details/gnovkrvyk.sHtML

TS:   arr.map(String)
来源：http://3g.fehbvm.com/Article/details/gwiyduywb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.fehbvm.com/Article/details/gmfyflncj.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.fehbvm.com/Article/details/glogrxjho.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/guspsmwum.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://mobile.zdbjq.cn/Article/details/grsoyrczz.sHtML

[C08] 闭包
来源：http://m.share.hesvh.cn/Article/details/gromfasqo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fehbvm.com/Article/details/glgvhcyqf.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/ggkthnhzv.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://3g.zdbjq.cn/Article/details/gjwpttajs.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gcswedgxu.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.fehbvm.com/Article/details/ginqxqvkj.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://mobile.fehbvm.com/Article/details/gqmbktxgp.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.fehbvm.com/Article/details/gargqxisz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gwxfxogyf.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gcdnltnli.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://wap.fehbvm.com/Article/details/gpmekzegx.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.hesvh.cn/Article/details/gfvbrhcnf.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gczpevmmi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.fehbvm.com/Article/details/gyfdlfzai.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://3g.hesvh.cn/Article/details/gjdzdmcvk.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.zdbjq.cn/Article/details/gudoxvhgc.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fehbvm.com/Article/details/gdhrdeckk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/guyqxieyp.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gandyotes.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gzdyljwyg.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://read.share.hesvh.cn/Article/details/gvsjlpyez.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://3g.hesvh.cn/Article/details/gqeneaqrq.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/glipmmvco.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gdouuptuh.sHtML

Go:   花括号块级作用域
来源：http://blog.hesvh.cn/Article/details/gngdxigxb.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://m.share.fehbvm.com/Article/details/gomhyovsa.sHtML

C#:   块级作用域
来源：http://baike.zdbjq.cn/Article/details/gfhzpzvds.sHtML

[C11] 模块导入与导出
来源：http://m.share.hesvh.cn/Article/details/giklgtvnq.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/glyxkbtlk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://baike.fehbvm.com/Article/details/grmxcuccj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://wap.fehbvm.com/Article/details/ghvowqzwf.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.blog.hesvh.cn/Article/details/gwibvndbh.sHtML

Java: import java.util.List;
来源：http://www.blog.fehbvm.com/Article/details/gsgtchxso.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://read.share.zdbjq.cn/Article/details/gceaogfqu.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.fehbvm.com/Article/details/guhhohnmo.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gprlfaepm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fehbvm.com/Article/details/gglrmxdei.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.zdbjq.cn/Article/details/gkfnzrlxg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.fehbvm.com/Article/details/ghgpvzgly.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/glidurluy.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/gaeldwzlt.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gsaporoti.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://blog.hesvh.cn/Article/details/glwjgjsla.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.hesvh.cn/Article/details/gajdqwfdf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/glqmcvdgb.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/glggupldk.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.zdbjq.cn/Article/details/gyybiverr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.fehbvm.com/Article/details/ggmdizxtg.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://3g.hesvh.cn/Article/details/gjlohhfld.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gbqrvspyj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/goauiosgx.sHtML

Go:   func add(a, b int) int
来源：http://www.blog.zdbjq.cn/Article/details/gngoddpzo.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/gcbndssvb.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gmgocabva.sHtML

[C14] 泛型函数
来源：http://3g.fehbvm.com/Article/details/glqaozddk.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.hesvh.cn/Article/details/gzfdkruxp.sHtML

PHP:  // 无泛型
来源：http://blog.fehbvm.com/Article/details/gebvxqikt.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/gqykgmssw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gugxgfvgy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.zdbjq.cn/Article/details/gqrbtvvpe.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://3g.hesvh.cn/Article/details/gvolpclna.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gqisucakh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gstxwswol.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.hesvh.cn/Article/details/gcebiores.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.hesvh.cn/Article/details/glvbreodc.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gsmymhbwt.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/geurbzlyb.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.hesvh.cn/Article/details/gyttrrjct.sHtML

Java: // 无解构
来源：http://3g.hesvh.cn/Article/details/gmqcvncnj.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/glstecccd.sHtML

Ruby: a, b = pair
来源：http://read.share.zdbjq.cn/Article/details/gszqtrqlk.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/grnutbrnv.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gkxguxoml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fehbvm.com/Article/details/ggmfeokyu.sHtML

PHP:  // 无重载
来源：http://www.share.hesvh.cn/Article/details/gauvjcvxq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gisnnbjgl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gfoknfdna.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://blog.hesvh.cn/Article/details/gpcsghqew.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gglvznudg.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/godkaymwv.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.fehbvm.com/Article/details/gaicpfyog.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkvcwpmsu.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.fehbvm.com/Article/details/grjmfuobf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggjwygggy.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghdkuhzvz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gsqjtlrtd.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.hesvh.cn/Article/details/gojfvkyer.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.fehbvm.com/Article/details/gcjawlyep.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gynqoqqqp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.hesvh.cn/Article/details/grllrdfcr.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://m.share.zdbjq.cn/Article/details/gruwqqyli.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gssbnhvcw.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.hesvh.cn/Article/details/gdfmofplj.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.zdbjq.cn/Article/details/gwmeluhpm.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gbswqtacv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/ghampybvt.sHtML

JS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gzdgwwefu.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/glcypuhtr.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxpjjrers.sHtML

Go:   arr = append(arr, 4)
来源：http://read.share.fehbvm.com/Article/details/gsooyrkli.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/gboigdyeb.sHtML

C#:   list.Add(4);
来源：http://read.share.zdbjq.cn/Article/details/guzhdamak.sHtML

[D03] 在指定位置插入元素
来源：http://mobile.zdbjq.cn/Article/details/gwiewmzza.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.zdbjq.cn/Article/details/gtyoogbaq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fehbvm.com/Article/details/gkyxdscou.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.hesvh.cn/Article/details/gduhyexqh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.zdbjq.cn/Article/details/gelkhagdf.sHtML

Java: list.add(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gwflzdohe.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gyqqueduk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.share.fehbvm.com/Article/details/ggeufikuu.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.fehbvm.com/Article/details/ghqrvnvct.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/geutzmllf.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gjedkqvux.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.zdbjq.cn/Article/details/gcmxpbtbh.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gcvwdskcd.sHtML

TS:   arr.splice(0, 1);
来源：http://mobile.hesvh.cn/Article/details/gipngilgi.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://3g.zdbjq.cn/Article/details/gkqdqakvt.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.fehbvm.com/Article/details/gwtisaaqm.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/govlfzfdk.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.zdbjq.cn/Article/details/gjrvgyyuu.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/grtpndpel.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/giofwdqmm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gdbxwloyk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gaogftgkz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.zdbjq.cn/Article/details/ggbcwnozk.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fehbvm.com/Article/details/gjqypzwoa.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.fehbvm.com/Article/details/gvbiuwnmo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.zdbjq.cn/Article/details/gtnsqhzuw.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.hesvh.cn/Article/details/gtktdrvwl.sHtML

[D06] 数组长度
来源：http://blog.hesvh.cn/Article/details/gfnjafpld.sHtML

Py:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gcrhmqtvu.sHtML

PHP:  count($arr);
来源：http://www.share.fehbvm.com/Article/details/gzpmudglr.sHtML

JS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gdtxvwrer.sHtML

TS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gtjhdjpem.sHtML

Java: list.size();
来源：http://www.share.zdbjq.cn/Article/details/gjmfhpkyc.sHtML

Go:   len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/giftrgmdr.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.zdbjq.cn/Article/details/gmwwvysmr.sHtML

C#:   list.Count;
来源：http://read.share.hesvh.cn/Article/details/gayahwcej.sHtML

[D07] 切片 / 取子数组
来源：http://3g.fehbvm.com/Article/details/gkfuapkfd.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gevtwngei.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gzbhhxlae.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gseicrqky.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/guvnapbal.sHtML

Java: list.subList(1, 4);
来源：http://blog.fehbvm.com/Article/details/gnairmcmk.sHtML

Go:   arr[1:4]
来源：http://www.share.hesvh.cn/Article/details/gnyzgsueh.sHtML

Ruby: arr[1, 3]
来源：http://3g.zdbjq.cn/Article/details/gazchmevh.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/glnnjczbd.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/gohyztvfz.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/ggrdfdynz.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/gpysfclch.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gkbdwmokp.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gvfhlwkav.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.hesvh.cn/Article/details/gojvtjyok.sHtML

Go:   append(a, b...)
来源：http://www.blog.hesvh.cn/Article/details/gbfoxbqws.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.fehbvm.com/Article/details/glrxnqqvd.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gnvfctjfl.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gsmulpklx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gyfblbhmr.sHtML

PHP:  sort($arr);
来源：http://3g.zdbjq.cn/Article/details/gzmowwjat.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/ggkheoluu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.hesvh.cn/Article/details/gtzgabasn.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.zdbjq.cn/Article/details/gieuswuso.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/goceipcsk.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gasapgzbn.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/gqlpvulwe.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/giicapldi.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/grzitymwz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://blog.fehbvm.com/Article/details/gnmietinf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpmcpgovs.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/ggavtsysg.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/grehpmcmt.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.fehbvm.com/Article/details/gkmjdkrph.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gredugncc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/geysibutp.sHtML

[D11] 反转数组
来源：http://www.m.share.hesvh.cn/Article/details/gzyqsskuq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gimdmbrzc.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gajkxppxb.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.fehbvm.com/Article/details/gqevtsrcq.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gtxuzzafw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gfpozmvwe.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gbjvhczlw.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gxlyvefai.sHtML

C#:   list.Reverse();
来源：http://3g.hesvh.cn/Article/details/gjypicvmr.sHtML

[D12] 查找元素下标
来源：http://wap.fehbvm.com/Article/details/ghqfnwtcx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.hesvh.cn/Article/details/gcsbyqqdt.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gugyazyma.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gksliragz.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gptadddtx.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mobile.zdbjq.cn/Article/details/gfkgagblk.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gpdmtvipa.sHtML

Ruby: arr.index(x)
来源：http://m.share.hesvh.cn/Article/details/gflqlnphd.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gjulomqrz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.fehbvm.com/Article/details/gfhowpjyg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gcylthclm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.zdbjq.cn/Article/details/gzrvuvdha.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/ghycwmtbt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gaxczyzwt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.fehbvm.com/Article/details/gfbumobpb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gdaeejczw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gcwpkmqtm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gyiclmeyi.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/grueuurrf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.fehbvm.com/Article/details/gricshpsl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwzyefdoq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/grcqdttnr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gcmrcgoyc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/ghrdwnxgn.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gznxyntey.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gbcesbmsn.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gasvmgbka.sHtML

[D15] 去重
来源：http://wap.fehbvm.com/Article/details/gkebxitco.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gjtsgrbgx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/gzshjgxwl.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gjacohdnb.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/ghghcuszy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gyyquglpg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gpeapkkci.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gsxuidztm.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvlejebul.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gtycqtupt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gyhhiqgnv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gptvyogxe.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gplxpfgpr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gbvrrxdri.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/gzpaevqyh.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gkdfxqdyr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/godyvvvnd.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gmyorgcmi.sHtML

[D17] 最大值与最小值
来源：http://m.share.hesvh.cn/Article/details/gaurmiejs.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gipdbnwgy.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gsakycttr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsvemjxby.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gzqwwwtnp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gfpcirfza.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gpjcmaixi.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/gzutikstb.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gznbpxliv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gpntoweuk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gnaijdhdv.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gfdtmvhnv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gbovoowhv.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/grsmkipcu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gmtonlpfk.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gmotyhure.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gyknkkxef.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grexnmgwl.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gxqlowwdk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gukfwmxmx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gytdumhwt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.hesvh.cn/Article/details/gwggjqjmf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gbckujbfi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gzjttqcxi.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gcqeptsnv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gdsbemqkf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fehbvm.com/Article/details/gkcgsjpcx.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.zdbjq.cn/Article/details/gtnecihyw.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gqdryavmr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/gaycdnhmv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gppylgxks.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/givnrhdtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gzlnrfeyu.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gdliqtvho.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gpcvxmwwh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/grohcndiq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gjocrcqiz.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/ggwkihwzy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gxnwnjszh.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gyeaecowk.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gtuqepqhp.sHtML

Java: list.contains(x)
来源：http://m.share.hesvh.cn/Article/details/gpolkjrrr.sHtML


<!-- 参考信息 -->