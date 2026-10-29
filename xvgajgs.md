代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://read.share.hesvh.cn/Article/details/gtisnmezn.sHtML

[C07] 把函数作为参数传入
来源：http://www.blog.fehbvm.com/Article/details/ghirggfra.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://blog.fehbvm.com/Article/details/ggldruhja.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gfjtndyru.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.fehbvm.com/Article/details/gxsuvzlbg.sHtML

TS:   arr.map(String)
来源：http://www.m.share.fehbvm.com/Article/details/guuozkiwb.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gqcyftjoe.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://read.share.zdbjq.cn/Article/details/gqkijimdp.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.hesvh.cn/Article/details/ghtbtdvxo.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://www.share.fehbvm.com/Article/details/gdvmpwhix.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/gexyvbnim.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://3g.hesvh.cn/Article/details/grtypzuob.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://3g.zdbjq.cn/Article/details/gwxnhgmef.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/ggeqzhuyv.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.zdbjq.cn/Article/details/gquflllen.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/goyvwoztl.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://m.share.zdbjq.cn/Article/details/gvyeoredf.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.zdbjq.cn/Article/details/gwxxwcbmp.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.hesvh.cn/Article/details/gwrshzqbj.sHtML

[C09] 递归
来源：http://baike.zdbjq.cn/Article/details/gwmtegkvr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fehbvm.com/Article/details/gsdbdlowk.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gnvqkrgsl.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.m.share.hesvh.cn/Article/details/gerbhdalz.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.zdbjq.cn/Article/details/gckaxouia.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.zdbjq.cn/Article/details/gixphzafy.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://wap.fehbvm.com/Article/details/gqrnqwdgh.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.zdbjq.cn/Article/details/gaxunvjmk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://3g.fehbvm.com/Article/details/godgujggb.sHtML

[C10] 变量作用域
来源：http://www.blog.zdbjq.cn/Article/details/gqzwnwjaj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/gdedmvluw.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fehbvm.com/Article/details/gyoqaxghv.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://m.share.fehbvm.com/Article/details/gkgnqnezn.sHtML

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gdlujluxd.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gaboemyjd.sHtML

Go:   花括号块级作用域
来源：http://3g.fehbvm.com/Article/details/gqrqljhqc.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.hesvh.cn/Article/details/gqkjkioed.sHtML

C#:   块级作用域
来源：http://blog.fehbvm.com/Article/details/gkxmzjgci.sHtML

[C11] 模块导入与导出
来源：http://blog.hesvh.cn/Article/details/gqgrrmdch.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gwwcxgtjw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gixtjubwu.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gyqsbzdae.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.hesvh.cn/Article/details/gdpxklfrn.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gishwwieu.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/giddywyvh.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gqxtcxcjp.sHtML

C#:   using System.Text;
来源：http://baike.hesvh.cn/Article/details/guluvtvha.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.blog.hesvh.cn/Article/details/guoxpalwz.sHtML

Py:   (lambda: print("run"))()
来源：http://3g.zdbjq.cn/Article/details/gbuludzlg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/gspopwjxk.sHtML

JS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/glzcqthgr.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.hesvh.cn/Article/details/gplqdnqiu.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gmjoeuqdu.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.zdbjq.cn/Article/details/gznhtxepk.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.zdbjq.cn/Article/details/ggtrxmrww.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.zdbjq.cn/Article/details/gdagncxtt.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.m.share.hesvh.cn/Article/details/gwgsjzzgd.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gaobeciqm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gifqweprr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.zdbjq.cn/Article/details/gswitfcjo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxnltaljm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/guraunxpg.sHtML

Go:   func add(a, b int) int
来源：http://mobile.zdbjq.cn/Article/details/gqbfbtrmr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.zdbjq.cn/Article/details/gwbqkyexf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gumpoolpn.sHtML

[C14] 泛型函数
来源：http://m.share.zdbjq.cn/Article/details/gvzzecoaz.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/grvbniabz.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gufibctmt.sHtML

JS:   // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gdlzbqgmr.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://read.share.fehbvm.com/Article/details/geervbpeq.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://m.share.hesvh.cn/Article/details/gztneobwl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/glwuzrlwr.sHtML

Ruby: # 无泛型
来源：http://m.share.fehbvm.com/Article/details/gdscamroi.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://m.share.fehbvm.com/Article/details/gtvvhxeic.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gzjihrwoo.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/gnuqrwzkz.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.hesvh.cn/Article/details/gowtrstoy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.fehbvm.com/Article/details/gycwngfal.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/grqvwrztj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/glwahbuke.sHtML

Go:   // 无解构
来源：http://mobile.hesvh.cn/Article/details/gtxfsudzy.sHtML

Ruby: a, b = pair
来源：http://m.share.fehbvm.com/Article/details/grmaibzgf.sHtML

C#:   var (a, b) = pair;
来源：http://www.m.share.hesvh.cn/Article/details/gltjlzfha.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fehbvm.com/Article/details/gfhvalppo.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.zdbjq.cn/Article/details/gplqiestc.sHtML

PHP:  // 无重载
来源：http://blog.fehbvm.com/Article/details/gjegnjwgg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.zdbjq.cn/Article/details/gyhgphlrk.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.fehbvm.com/Article/details/gygtkyapx.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://read.share.fehbvm.com/Article/details/grfdwlxvw.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/gnzlxognl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.zdbjq.cn/Article/details/ghiltkqkj.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/getwiyvlr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyhwfwnyv.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.fehbvm.com/Article/details/grvxtkkte.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gxrfmvboi.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.hesvh.cn/Article/details/ghcbhledc.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.m.share.fehbvm.com/Article/details/gndpoyxzu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.fehbvm.com/Article/details/gfidlujvl.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gfmnfzahh.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gjhfvkcgp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.hesvh.cn/Article/details/gfazfvwjz.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gyfopcmji.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.share.zdbjq.cn/Article/details/glixryuwb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/ggdinmavx.sHtML

[D02] 追加元素到末尾
来源：http://read.share.zdbjq.cn/Article/details/gssodhraj.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.fehbvm.com/Article/details/gywicqgvk.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/glgkalqid.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gxlzqiyqt.sHtML

TS:   arr.push(4);
来源：http://www.share.hesvh.cn/Article/details/gnzvtzaqu.sHtML

Java: list.add(4);
来源：http://3g.zdbjq.cn/Article/details/glowipcbn.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/ggtfvpjlk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fehbvm.com/Article/details/glpbebqvx.sHtML

C#:   list.Add(4);
来源：http://read.share.hesvh.cn/Article/details/gzqqowepx.sHtML

[D03] 在指定位置插入元素
来源：http://www.share.hesvh.cn/Article/details/gleaccsnd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gnqmrfxwd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.hesvh.cn/Article/details/gfmvzfoll.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.zdbjq.cn/Article/details/ghdivwgml.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/gdqrgkheo.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/giltshzoi.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.zdbjq.cn/Article/details/ggtekrzzh.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gqmzxszjf.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.fehbvm.com/Article/details/gparaywki.sHtML

[D04] 删除元素
来源：http://3g.zdbjq.cn/Article/details/gtmqwoouz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.zdbjq.cn/Article/details/gfouofisr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/gnecnmnym.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.zdbjq.cn/Article/details/ggznbfkgc.sHtML

TS:   arr.splice(0, 1);
来源：http://blog.fehbvm.com/Article/details/gfcubzsid.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.fehbvm.com/Article/details/gnfnwurst.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gkoawqhwf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.zdbjq.cn/Article/details/gbuduwlbp.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gtqqpvrgc.sHtML

[D05] 访问与修改元素
来源：http://www.blog.zdbjq.cn/Article/details/goexjxlrl.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gworuqnbm.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/gmcqkfxxc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gyqrxfccf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.zdbjq.cn/Article/details/gwjlwalni.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.zdbjq.cn/Article/details/gwowvfwgi.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fehbvm.com/Article/details/gprouckwg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/gckruzcqg.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fehbvm.com/Article/details/gfyavmcvv.sHtML

[D06] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gsabdouur.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gckhswsyp.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gghdnsaye.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gaazknbfb.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gleqmfkuq.sHtML

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/grgohgyac.sHtML

Go:   len(arr)
来源：http://3g.hesvh.cn/Article/details/gpokojbkw.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gwazhpyvc.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gfsqnfaib.sHtML

[D07] 切片 / 取子数组
来源：http://read.share.fehbvm.com/Article/details/gxvyjtxhb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/ghhbcbkmu.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://baike.hesvh.cn/Article/details/gbpixkpyr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gfyansxpn.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.zdbjq.cn/Article/details/gncajbztz.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gcxiilqmo.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/glfgpdgii.sHtML

Ruby: arr[1, 3]
来源：http://mobile.zdbjq.cn/Article/details/gjheygnko.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gvwrbhvqz.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/gymrbxkta.sHtML

Py:   a + b;  a.extend(b)
来源：http://baike.hesvh.cn/Article/details/gevbrmbmn.sHtML

PHP:  array_merge($a, $b);
来源：http://3g.zdbjq.cn/Article/details/gwvzrfitb.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.fehbvm.com/Article/details/geugivztf.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fehbvm.com/Article/details/gxbhncsmo.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/guphhbnsu.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fehbvm.com/Article/details/gjawpyjih.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fehbvm.com/Article/details/gywfkmzwx.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.hesvh.cn/Article/details/gltalmewn.sHtML

[D09] 排序（升序）
来源：http://3g.zdbjq.cn/Article/details/gejgcckax.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gaavltlcm.sHtML

PHP:  sort($arr);
来源：http://m.share.fehbvm.com/Article/details/gtupolxho.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.hesvh.cn/Article/details/gcpmlhhqw.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.hesvh.cn/Article/details/glywkrexd.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.fehbvm.com/Article/details/gfvehmxzy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbwbceukz.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gaagejffp.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gqzygmcrq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gmsefxuct.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.zdbjq.cn/Article/details/gszhkjtnl.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gcjmtwkst.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gvhvvykok.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gajmqkmws.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gccqrsyey.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gckcwzciv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.hesvh.cn/Article/details/gaxqefgqf.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.zdbjq.cn/Article/details/gpbhxnwjx.sHtML

[D11] 反转数组
来源：http://www.blog.hesvh.cn/Article/details/gfkzvxyjm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.zdbjq.cn/Article/details/gvtsuletl.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gczsrscif.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gavycvepg.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gbvgyuvgf.sHtML

Java: Collections.reverse(list);
来源：http://read.share.hesvh.cn/Article/details/gwaehauss.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/gcrubrero.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gemrztpty.sHtML

C#:   list.Reverse();
来源：http://www.blog.hesvh.cn/Article/details/gsvlwylfv.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gqnzstfva.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gmyuewzii.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/gqffgxjxa.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/golavylph.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/glzakinyr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.fehbvm.com/Article/details/gtpoycklc.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gzzmhoiio.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/ggmidftuy.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/geobxmcxw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gfkitjrux.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.fehbvm.com/Article/details/gltorvald.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gszpnkqdr.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gwmjbtryp.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gerdvrcce.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/ggvchskme.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.fehbvm.com/Article/details/gwzjyoxlv.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gtoerjwrz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/gfyvwpsgh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gqikfgvrp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gznoodafx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gmegybhtu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/ghlmsrzlw.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gxmdelilz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gdxgpqzmx.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gctmmgrxj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/goqxaqqyg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gvvttqyph.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/gijkygjzr.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gxjqfzhrh.sHtML

PHP:  array_unique($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggmvjhrxw.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gbguxzzcp.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gphpkregy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fehbvm.com/Article/details/gfajzlzmr.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gauzxqqlh.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/gqfqmezte.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gbgltgjfw.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/gdlggoppg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gpicmahmo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gkurarrcu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/grsggzkcy.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gawclqdvy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.zdbjq.cn/Article/details/govjygtyd.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gduwbiclk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gapmzccpr.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gyqvzhqsw.sHtML

[D17] 最大值与最小值
来源：http://m.share.zdbjq.cn/Article/details/grblxzjyc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.fehbvm.com/Article/details/gpdpqffkk.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/glujfldgp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gcqukufni.sHtML

TS:   Math.max(...arr);
来源：http://www.share.hesvh.cn/Article/details/gcomwnnxh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.zdbjq.cn/Article/details/gifeymozb.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gwoouwqtb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gjnnttqou.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gaxvfzcow.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gubssrhvl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gidofjhxn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gtvvbprbh.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gcrnkzvsf.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/guwnwcyqd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/grzmchikl.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gmaiuoxbf.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gvsumovea.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gxlngahmj.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gxyuvpzow.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gbfizxtbi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gttltswit.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gjazikwkl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/grfkjrxda.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/glnmtbtmn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ggtvtveke.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gghlggdas.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gssrwylxt.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gjybiylbu.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gbetbipty.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/ghunpspgo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gczesrmou.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gqfegmdgt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gtjolydnc.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/ggenlvraa.sHtML

Ruby: arr.tally
来源：http://read.share.zdbjq.cn/Article/details/gyzlandsv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.hesvh.cn/Article/details/grfgeaqud.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/grqhgslth.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gnkalozvk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gffdhqgst.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gurqlylee.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gigymnszo.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gkvigihtj.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gmoegptqm.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxcbojquz.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/glhhscbty.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gxiwwoffp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmjdgyuk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/getrcuusr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/gjpoctnys.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gwndsjqgt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gyrduibwj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/glxocomsp.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gogaecjum.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gvqgnuccv.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gjdtretus.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gehdibiod.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gjweulfgk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/gsyhkjlut.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gmwesjaam.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gvxapmyxj.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gobnhhxzp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/glvsbcjpi.sHtML


<!-- 参考信息 -->