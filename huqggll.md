代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://baike.fanxiaobao.xyz/Article/details/goquedkrl.sHtML

TS:   arr.map(String)
来源：http://www.share.fanxiaobao.xyz/Article/details/grdyxfdqv.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gfhyvjnfd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://3g.fanxiaobao.xyz/Article/details/ggvnqbykv.sHtML

Ruby: arr.map(&:upcase)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqbshhev.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtqwxnrr.sHtML

[C08] 闭包
来源：http://baike.fanxiaobao.xyz/Article/details/ggrytnotu.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.fanxiaobao.xyz/Article/details/gfzvvsfyt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzkilpufy.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghmdicygu.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfuqmbbh.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/ggeebtdqw.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://wap.fanxiaobao.xyz/Article/details/gpyzwmyrx.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gndzjnrlf.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcrfntdcd.sHtML

[C09] 递归
来源：http://blog.fanxiaobao.xyz/Article/details/gnrqzdwkc.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmtysuqjm.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://blog.fanxiaobao.xyz/Article/details/gjebxwaci.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fanxiaobao.xyz/Article/details/gwboaptie.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.fanxiaobao.xyz/Article/details/gbsjwawce.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbdwlqoi.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmsympaan.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmkjbidr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtcqdxyp.sHtML

[C10] 变量作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gwrmegasw.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkykwbsp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://m.share.fanxiaobao.xyz/Article/details/grqnzdojn.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://baike.fanxiaobao.xyz/Article/details/giyvtgihj.sHtML

TS:   同 JS
来源：http://www.share.fanxiaobao.xyz/Article/details/gpjdtrvaf.sHtML

Java: 方法内为块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gcnidhbhv.sHtML

Go:   花括号块级作用域
来源：http://wap.fanxiaobao.xyz/Article/details/gxsrmxrxz.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fanxiaobao.xyz/Article/details/gogqeeoko.sHtML

C#:   块级作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtzyhlcv.sHtML

[C11] 模块导入与导出
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkdmevin.sHtML

Py:   from module import func
来源：http://www.share.fanxiaobao.xyz/Article/details/gytaxuopf.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznmejlqy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvuvqfnm.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gqwhhpcyf.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmrdmzor.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjrdattk.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://wap.fanxiaobao.xyz/Article/details/gwrnxbcdv.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkusolamm.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fanxiaobao.xyz/Article/details/gqptikpty.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.fanxiaobao.xyz/Article/details/gxnzzkiqq.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.fanxiaobao.xyz/Article/details/gxlvrdghz.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvdnxqag.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjfmvocc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.fanxiaobao.xyz/Article/details/glinlzmxf.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gppbgekiy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmebntyb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/grppbqqle.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fanxiaobao.xyz/Article/details/gwicggvcg.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnsefnyn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/geeyuixcu.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/glqnqwzsb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtckacse.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbcrwqiao.sHtML

Go:   func add(a, b int) int
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwazlzcj.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://wap.fanxiaobao.xyz/Article/details/gkdswkgdg.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.fanxiaobao.xyz/Article/details/gymicibjt.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gunuyqkgl.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gkqezfdcs.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gseaxujhn.sHtML

JS:   // 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gystlwodp.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtckfxnfp.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gczzsoxnk.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/ghlyflakr.sHtML

Ruby: # 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyogvuwai.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fanxiaobao.xyz/Article/details/gywfkqyjr.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fanxiaobao.xyz/Article/details/gdrhzixhm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbzwkzup.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gkylqduue.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gecenouyk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzovbggoj.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjijeifa.sHtML

Go:   // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grotmnzci.sHtML

Ruby: a, b = pair
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsctdnevg.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnpkpggy.sHtML

[C16] 函数 / 方法重载
来源：http://blog.fanxiaobao.xyz/Article/details/glluwhmcw.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gylyanhvs.sHtML

PHP:  // 无重载
来源：http://blog.fanxiaobao.xyz/Article/details/grvababca.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.fanxiaobao.xyz/Article/details/gehmowtzw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmeplxhee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdmgadbi.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjpojffq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gztjhuzjg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcufntncc.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbhpvjtg.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutybolaa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlnchoww.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/giuomxonh.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlimnken.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wap.fanxiaobao.xyz/Article/details/gtsduuahl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudszvxvl.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/gnnarssya.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.fanxiaobao.xyz/Article/details/gstykxyvi.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.fanxiaobao.xyz/Article/details/gmggedkfs.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/garlesoar.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/glcmffibs.sHtML

[D02] 追加元素到末尾
来源：http://3g.fanxiaobao.xyz/Article/details/gfginlyzl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.fanxiaobao.xyz/Article/details/gcddmhvje.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyovzaibp.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruzpuuna.sHtML

TS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfkmzdpg.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmjkenns.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fanxiaobao.xyz/Article/details/gmdathwqs.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbfhblrix.sHtML

C#:   list.Add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaxnjeel.sHtML

[D03] 在指定位置插入元素
来源：http://wap.fanxiaobao.xyz/Article/details/gptvgsxwr.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gyexjcufa.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuufkrey.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaicozbu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gebqqqdcm.sHtML

Java: list.add(0, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gkjskwkce.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtopsyngf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfseducur.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gwgqzujcu.sHtML

[D04] 删除元素
来源：http://blog.fanxiaobao.xyz/Article/details/gpjjoazdn.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjksbmel.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gejdgwnbv.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fanxiaobao.xyz/Article/details/gzoriothp.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fanxiaobao.xyz/Article/details/grckhnwxq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvcdgnjsv.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggebjlabe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gaibmjaks.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gyergxtyd.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gzbcsodvq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gxstqwcae.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gacqofvoi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoetwhqk.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://wap.fanxiaobao.xyz/Article/details/gvdpnjafu.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/gzurnahfy.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gfctjojit.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhnmmakk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gengfxyxo.sHtML

[D06] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbhbdpfm.sHtML

Py:   len(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitocxmxy.sHtML

PHP:  count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyrqvkfe.sHtML

JS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/goicklpoi.sHtML

TS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwwdrlnf.sHtML

Java: list.size();
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbkteyot.sHtML

Go:   len(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gizooamwx.sHtML

Ruby: arr.length; arr.size
来源：http://3g.fanxiaobao.xyz/Article/details/gawkumoqd.sHtML

C#:   list.Count;
来源：http://mobile.fanxiaobao.xyz/Article/details/gamsjrjnt.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fanxiaobao.xyz/Article/details/gqcjtbfcm.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdohbujbw.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkzoixul.sHtML

JS:   arr.slice(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgwnuisr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gdhelsldx.sHtML

Java: list.subList(1, 4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdupqulpf.sHtML

Go:   arr[1:4]
来源：http://read.share.fanxiaobao.xyz/Article/details/grwoegcoj.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvwinphi.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gcpashvec.sHtML

[D08] 合并两个数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlzbkaat.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpjqckfrf.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjpjwjz.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuumpvyd.sHtML

TS:   [...a, ...b];
来源：http://www.share.fanxiaobao.xyz/Article/details/grdgjivyq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gsvygfkdu.sHtML

Go:   append(a, b...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gusbneoca.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjnypvfqe.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgzszsjo.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gxpooamfu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/giuucksvn.sHtML

PHP:  sort($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghdlccsbe.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fanxiaobao.xyz/Article/details/gxmosipny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiuvvksd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/gywxlakdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gtxvpfcqo.sHtML

Ruby: arr.sort
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhjhbfbb.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghajncvwd.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgrsetwb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnevywlbj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.fanxiaobao.xyz/Article/details/gziygctmb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gtyfnrxkf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fanxiaobao.xyz/Article/details/gemsfplsi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fanxiaobao.xyz/Article/details/gjmewlkij.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fanxiaobao.xyz/Article/details/gbdmqdqjv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fanxiaobao.xyz/Article/details/geicgwyeg.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fanxiaobao.xyz/Article/details/girpmjayf.sHtML

[D11] 反转数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvszoiurk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtbmrfjh.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnoxbkoa.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwevhfizv.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gioqgkpwr.sHtML

Java: Collections.reverse(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmtourkq.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gretkywea.sHtML

Ruby: arr.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhybxeox.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gtpeavsbz.sHtML

[D12] 查找元素下标
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbiynpdr.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gidkhqcyd.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzonygdk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gufcwrchp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxlbhcxa.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjenippos.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fanxiaobao.xyz/Article/details/gflddzbfa.sHtML

Ruby: arr.index(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gacluyxmi.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcljsyiax.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gwghadoac.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmfnorna.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gbbhhcuqt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gohkphlnr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqivofnss.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gadgsfwze.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqgzhgzo.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gextvdeoq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gwysbmvch.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebyoajmz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayscgufk.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gechodgwk.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gothtyhbc.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gzoagnhrw.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjbaoyzqq.sHtML

Go:   // 手写循环
来源：http://3g.fanxiaobao.xyz/Article/details/gchviltxa.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctloqlko.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gexocdcmf.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/giefbovez.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahnrwgly.sHtML

PHP:  array_unique($arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gumrlbjmz.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fanxiaobao.xyz/Article/details/gkrkrfjnx.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fanxiaobao.xyz/Article/details/gnrsrxenz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fanxiaobao.xyz/Article/details/gdsruuwod.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gaqondfgx.sHtML

Ruby: arr.uniq
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqhmxud.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fanxiaobao.xyz/Article/details/goincbvoa.sHtML

[D16] 求和与平均值
来源：http://3g.fanxiaobao.xyz/Article/details/gylzhxrfm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsawhjlgn.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giayjqgel.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmiqcwhdg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfangeo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdknfgcc.sHtML

Go:   // 手写循环累加
来源：http://read.share.fanxiaobao.xyz/Article/details/gjscuqxfz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/grwqujxti.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxrbbywr.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwqmfdoy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gbatdsnyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsivjmkbf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilomvcag.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmofqkken.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzzhfnhbm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbsmzarg.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fanxiaobao.xyz/Article/details/gywtcsdqy.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fanxiaobao.xyz/Article/details/goyrjhqfp.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fanxiaobao.xyz/Article/details/gnrrjrgjk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljkhmdtd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gtwiaeany.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjfbctosx.sHtML

TS:   nested.flat();
来源：http://blog.fanxiaobao.xyz/Article/details/geyfrccat.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxnpflma.sHtML

Go:   // 手写双层循环
来源：http://wap.fanxiaobao.xyz/Article/details/gtoohuaqo.sHtML

Ruby: nested.flatten
来源：http://wap.fanxiaobao.xyz/Article/details/gwlmtznrw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gtctcmfqr.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gyjmjnzwf.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gerjrhyio.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfjdekov.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gnpzfhzfy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyywpihyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/getkkcczb.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fanxiaobao.xyz/Article/details/gndxaqymi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhxfwcty.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/grbsuyqbx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glxvnjnjz.sHtML

Py:   Counter(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ggedbechs.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevhaclgv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fanxiaobao.xyz/Article/details/glrntzgyj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gfclzeuvm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fanxiaobao.xyz/Article/details/gcwcmhvaj.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gigzhlpry.sHtML

Ruby: arr.tally
来源：http://3g.fanxiaobao.xyz/Article/details/gaxxwsipl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fanxiaobao.xyz/Article/details/ghukpddov.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwsnfddny.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gtzthfywa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjnjropm.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkwpojgr.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagjmffui.sHtML

Java: list.contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gnkvybahb.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxsbjgjl.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggykfeegh.sHtML

C#:   list.Contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcbtunng.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/gprxctnkj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpsfulxh.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvjliprb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/grepdsdvw.sHtML

TS:   [...arr];
来源：http://wap.fanxiaobao.xyz/Article/details/gmvuchooc.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fanxiaobao.xyz/Article/details/gccnclwte.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/greoihapm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoakzfal.sHtML

C#:   new List<int>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gzstpbpic.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbyqfjnj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvcyvkcm.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gazvgbvpo.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblzblgjs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gvesssijq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geaccgpkx.sHtML

Go:   // 手写循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmgenzxr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fanxiaobao.xyz/Article/details/gylhctphv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdvahimg.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gkxmepdnx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gxpgeiliw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.fanxiaobao.xyz/Article/details/ghawytgsz.sHtML


<!-- 参考信息 -->