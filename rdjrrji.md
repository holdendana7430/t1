代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://3g.fehbvm.com/Article/details/gmgtqofrh.sHtML

TS:   arr.map(String)
来源：http://mobile.hesvh.cn/Article/details/gwsbgfkab.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://read.share.zdbjq.cn/Article/details/glofoillb.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.zdbjq.cn/Article/details/gixjrlxvf.sHtML

Ruby: arr.map(&:upcase)
来源：http://read.share.zdbjq.cn/Article/details/gkjkdubkw.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://baike.zdbjq.cn/Article/details/gdvgmfcxl.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gzbxhjfir.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/ggyjrzciq.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.share.hesvh.cn/Article/details/ggylctosz.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.hesvh.cn/Article/details/gengjbjfo.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gprlmcykx.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.fehbvm.com/Article/details/gwkacemkh.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://3g.fehbvm.com/Article/details/grtesubsn.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gsogcxumr.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://read.share.zdbjq.cn/Article/details/gzjqqxmsq.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gbyxmmkry.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/gxtikxhyl.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://m.share.fehbvm.com/Article/details/gqqtleufm.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.fehbvm.com/Article/details/gghukmzud.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://mobile.zdbjq.cn/Article/details/glnndvyss.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gjvxfkqxm.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.blog.fehbvm.com/Article/details/gspnttbqn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gpmadtzvy.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://read.share.hesvh.cn/Article/details/gifimczan.sHtML

[C10] 变量作用域
来源：http://read.share.hesvh.cn/Article/details/gjbuvsxdc.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://3g.hesvh.cn/Article/details/golcgtrmw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.fehbvm.com/Article/details/gvxpflqcl.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fehbvm.com/Article/details/gqaicuadr.sHtML

TS:   同 JS
来源：http://read.share.zdbjq.cn/Article/details/geqmbyanr.sHtML

Java: 方法内为块级作用域
来源：http://read.share.hesvh.cn/Article/details/gemloyjoo.sHtML

Go:   花括号块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbpudbdqe.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gyaimcnms.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gikbehaya.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.fehbvm.com/Article/details/ghvhoeymk.sHtML

Py:   from module import func
来源：http://www.blog.zdbjq.cn/Article/details/gagyvwjwx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.hesvh.cn/Article/details/gbqtjkbxe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fehbvm.com/Article/details/gbgpmcltd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/gbqytfxxa.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ghdrrmxsm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://mobile.zdbjq.cn/Article/details/grxwtifgq.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/gqmvxmxvu.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gzqxtrdkk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/ggmdxorit.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.hesvh.cn/Article/details/gwfgujxid.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gkloopied.sHtML

JS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gponagwpd.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gehtmhjxl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gojjdpscl.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gsuhnnkyh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gcjpgabtx.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/galbwbfko.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.zdbjq.cn/Article/details/gslevgsqe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fehbvm.com/Article/details/gpjrscplb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.hesvh.cn/Article/details/giozplvwy.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/geitrnssp.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gfmccdwjo.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gdexofidk.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gbuiwyjww.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.hesvh.cn/Article/details/guajebvga.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.fehbvm.com/Article/details/gilubfndc.sHtML

[C14] 泛型函数
来源：http://read.share.hesvh.cn/Article/details/gfvfnnbtm.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gdqzfppnh.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gbgqtwakv.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gdmmxjciu.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://m.share.zdbjq.cn/Article/details/ggvsxnqjq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.hesvh.cn/Article/details/gsnsybzeb.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.zdbjq.cn/Article/details/gtbkfycng.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gaotbwiqn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.hesvh.cn/Article/details/gfqyechdt.sHtML

[C15] 解构 / 展开参数
来源：http://m.share.hesvh.cn/Article/details/gsijvigel.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.hesvh.cn/Article/details/gqfzxtuov.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.zdbjq.cn/Article/details/gxhgdfqxq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gaeajdrot.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdaknjoya.sHtML

Java: // 无解构
来源：http://read.share.zdbjq.cn/Article/details/gbucuoobf.sHtML

Go:   // 无解构
来源：http://www.share.hesvh.cn/Article/details/gmgjcycph.sHtML

Ruby: a, b = pair
来源：http://www.m.share.hesvh.cn/Article/details/ggaogpkkj.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/gzzwxwuow.sHtML

[C16] 函数 / 方法重载
来源：http://read.share.fehbvm.com/Article/details/gdkslfkcc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.zdbjq.cn/Article/details/gcjoaodiy.sHtML

PHP:  // 无重载
来源：http://baike.zdbjq.cn/Article/details/gnvbvldtl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.fehbvm.com/Article/details/gfvuicpns.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gssbcolkl.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://m.share.zdbjq.cn/Article/details/gvlltxbgs.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.zdbjq.cn/Article/details/ghtlnxcpv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.zdbjq.cn/Article/details/gpavlcdeo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://3g.hesvh.cn/Article/details/glhbyfjyf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyletjjgb.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.zdbjq.cn/Article/details/gbdkndggr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glwshebcj.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gddfslkpl.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://blog.fehbvm.com/Article/details/gyngvfxuz.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gtfcpkloa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gvzdaovfs.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.zdbjq.cn/Article/details/gfnglvoed.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fehbvm.com/Article/details/gpntbqhzt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gjimzvrkt.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gkypepgpi.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fehbvm.com/Article/details/geyxwmxeo.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fehbvm.com/Article/details/gwfxgnuax.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fehbvm.com/Article/details/glfuuzbwq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.zdbjq.cn/Article/details/gadptcoln.sHtML

JS:   arr.push(4);
来源：http://wap.zdbjq.cn/Article/details/gkzeophgn.sHtML

TS:   arr.push(4);
来源：http://m.share.fehbvm.com/Article/details/gaaoexdon.sHtML

Java: list.add(4);
来源：http://www.m.share.fehbvm.com/Article/details/gifdswaqw.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.zdbjq.cn/Article/details/gnkvnhapk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fehbvm.com/Article/details/geymrdqft.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gnhvkwpia.sHtML

[D03] 在指定位置插入元素
来源：http://baike.fehbvm.com/Article/details/glakuucot.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.hesvh.cn/Article/details/guwwytrzv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.hesvh.cn/Article/details/gaiqjgxlf.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.share.hesvh.cn/Article/details/gopkjcckl.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtjrgqbx.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gnejdryqt.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.hesvh.cn/Article/details/goegljkxk.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.zdbjq.cn/Article/details/gffrzdwry.sHtML

C#:   list.Insert(0, 0);
来源：http://blog.zdbjq.cn/Article/details/glcxfsbvk.sHtML

[D04] 删除元素
来源：http://m.share.zdbjq.cn/Article/details/gkfyxollv.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fehbvm.com/Article/details/gkxrbkbiz.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fehbvm.com/Article/details/ghqxglewm.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fehbvm.com/Article/details/ghjrjbzex.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.zdbjq.cn/Article/details/ggrtqiowc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fehbvm.com/Article/details/gdrtbxblg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.zdbjq.cn/Article/details/gmxoojkuz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gjfnxfmvt.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/ghltmtazj.sHtML

[D05] 访问与修改元素
来源：http://www.m.share.hesvh.cn/Article/details/genzkqvun.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gvrinjbht.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gwsqnains.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gdhjqlwxi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.zdbjq.cn/Article/details/gfgtiidjf.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gpakyvcic.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/gvewevijg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://mobile.fehbvm.com/Article/details/gieqohagp.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.hesvh.cn/Article/details/gzhxmqmbj.sHtML

[D06] 数组长度
来源：http://read.share.fehbvm.com/Article/details/geqzqdstk.sHtML

Py:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gepnqumzj.sHtML

PHP:  count($arr);
来源：http://baike.hesvh.cn/Article/details/gnghrqpsy.sHtML

JS:   arr.length
来源：http://read.share.zdbjq.cn/Article/details/gpvnjwffr.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/grupjokkh.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gegdsieib.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gbujoxrgi.sHtML

Ruby: arr.length; arr.size
来源：http://wap.hesvh.cn/Article/details/grcllebss.sHtML

C#:   list.Count;
来源：http://wap.hesvh.cn/Article/details/grkvlghgi.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.hesvh.cn/Article/details/gtfhatnhr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gvhlrfrgf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/guqwfthvf.sHtML

JS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gmlqwdbyr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gjvzjsajv.sHtML

Java: list.subList(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqogaasqa.sHtML

Go:   arr[1:4]
来源：http://read.share.fehbvm.com/Article/details/glynbqjjy.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gxgflpcol.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.zdbjq.cn/Article/details/gydqrbyre.sHtML

[D08] 合并两个数组
来源：http://baike.fehbvm.com/Article/details/gnchxfsib.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.zdbjq.cn/Article/details/gjgznwxou.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.hesvh.cn/Article/details/gdzepieyq.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gtandhkug.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/glrmfpqmu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gcdnwourx.sHtML

Go:   append(a, b...)
来源：http://baike.fehbvm.com/Article/details/gmqsazard.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gesrpoojy.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gaefsrtle.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/giiehxtkp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gidqctrth.sHtML

PHP:  sort($arr);
来源：http://www.share.fehbvm.com/Article/details/giumkryuz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.fehbvm.com/Article/details/gnzelimgs.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.hesvh.cn/Article/details/gczzfyowp.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/gigjkaftt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqoopsrgs.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/giqvsndnl.sHtML

C#:   list.Sort();
来源：http://3g.zdbjq.cn/Article/details/gaslodlgy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/ghlbnhpdv.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gesdohkcy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fehbvm.com/Article/details/gzuhrlehp.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gdvvnwgox.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gpmoevehr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gruhxpulg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.zdbjq.cn/Article/details/gbxfnktyv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gkdifzngj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/ghnnuaozb.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/golcarksa.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gzflijryd.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gviyyaswt.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/ghvoxjbyj.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gunzwfgda.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/gbyxoxhmw.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gsjkxtxft.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gnoklcyxj.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gdovdeqmv.sHtML

[D12] 查找元素下标
来源：http://read.share.fehbvm.com/Article/details/glngptrdi.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gthbuqokc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gxrjpcukh.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gklojsyfv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gkigpidhl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.hesvh.cn/Article/details/golcorqjb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxshwowfe.sHtML

Ruby: arr.index(x)
来源：http://read.share.fehbvm.com/Article/details/gzoucpsev.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gpwxtjhfd.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/grrkcoqkn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gbsmfankf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gvnyqkzms.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gwsaeeaxw.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/gmipfhrcw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gcurirbhz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gifdeyceb.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/goaqvvgli.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.hesvh.cn/Article/details/gnurlqthy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gwzryhcnt.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gvclazmoy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.fehbvm.com/Article/details/gorlthsya.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.zdbjq.cn/Article/details/gngdeksyy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/guzoxbhsx.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/guvanxfsn.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gombiardj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/glirgwtvh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/gfnahmsqs.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gasidsusy.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fehbvm.com/Article/details/gwhihwxro.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/ggqqsedxv.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gjexwlkrf.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/guljpfxix.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.zdbjq.cn/Article/details/gofhsooqg.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gmwasdwiu.sHtML

Ruby: arr.uniq
来源：http://baike.zdbjq.cn/Article/details/gvahektqi.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/garlambwf.sHtML

[D16] 求和与平均值
来源：http://www.blog.fehbvm.com/Article/details/gsfedyjxd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/guqrdhbna.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/grjhdkoug.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gqkkwrxvr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvacjdahi.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gsjpctxjh.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gqasujfqa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gdawrmzfr.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gvszapqpp.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gvtglcjze.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/gtrrasfdg.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fehbvm.com/Article/details/gilnazani.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fehbvm.com/Article/details/gmqhtnuwk.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/glaunitaj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gaixgatap.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.hesvh.cn/Article/details/gtxegfejt.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gmrakoysy.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/guwiiznuz.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gsfvhhcqm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gmkfcsnvj.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.hesvh.cn/Article/details/gjcqcrclc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gmvoegiuz.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gqlromacv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gncjmrzno.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gbaosjfai.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gksrwqmgu.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gmwgdabzw.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/gsnubxfts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gdornehoa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gyaddlzvs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gwmwsjcst.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/giyqxeoxq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gbsnwbzkw.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gtizafpqr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.hesvh.cn/Article/details/glyacrrwb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gisclyuda.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gtxgznqjv.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gmhszlwai.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gtqvzokbg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gppdzhwim.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gtmnunwoj.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/groaeddvm.sHtML

Go:   // 手写 map[T]int
来源：http://blog.hesvh.cn/Article/details/gmqueozcn.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gefamuzwj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/ghzywevlp.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gjnvmytqe.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gqeunwlza.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gcppjvryn.sHtML

JS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gfqfmnsyr.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzjcwgvvd.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gjujdjoie.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxdgbzrtx.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gzxwjdcem.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gvywtiuve.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/gnuxansbv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gvpjdloua.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gtmveahdx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.fehbvm.com/Article/details/gehcxyszv.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gicsiaunn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gbprcqeqt.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gfesguooj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/givlabbnn.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gszhutwgn.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gdghcjxsq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/godxoydtt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gpzpsoyxw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gbjntipfs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gruvhafmg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gmhfojual.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gwgkbsjmc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.hesvh.cn/Article/details/gurlnfxzs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gxcvxuzyr.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gtnuqztna.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gddnxpdei.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gfkkemucv.sHtML


<!-- 参考信息 -->