代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrlsceoh.sHtML

TS:   arr.map(String)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxijgkki.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdenrmay.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudxqtmme.sHtML

Ruby: arr.map(&:upcase)
来源：http://baike.fanxiaobao.xyz/Article/details/gbxvmjkjk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.fanxiaobao.xyz/Article/details/gsiauqlny.sHtML

[C08] 闭包
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guyeuahrs.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.fanxiaobao.xyz/Article/details/geplfepad.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpzxltvr.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeywfuzk.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggawzvavl.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.fanxiaobao.xyz/Article/details/gnanxzwgp.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://blog.fanxiaobao.xyz/Article/details/gchqixboa.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.fanxiaobao.xyz/Article/details/gjxanmadz.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzhpnnztn.sHtML

[C09] 递归
来源：http://3g.fanxiaobao.xyz/Article/details/gvacgczfy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gcnmaceei.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.fanxiaobao.xyz/Article/details/gxuhxkfwo.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://m.share.fanxiaobao.xyz/Article/details/gmivyvoqi.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fanxiaobao.xyz/Article/details/gnummjxnq.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxstcgqlj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyfwvmhq.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/girrqksnq.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbanduhy.sHtML

[C10] 变量作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvdfxtqb.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://read.share.fanxiaobao.xyz/Article/details/grkinhyaj.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmpkvsve.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwknvdvzh.sHtML

TS:   同 JS
来源：http://3g.fanxiaobao.xyz/Article/details/goomhdren.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfcbhlje.sHtML

Go:   花括号块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmyyaegx.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.fanxiaobao.xyz/Article/details/gjnllodye.sHtML

C#:   块级作用域
来源：http://blog.fanxiaobao.xyz/Article/details/gyaqlfqdo.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfofujhe.sHtML

Py:   from module import func
来源：http://baike.fanxiaobao.xyz/Article/details/gvnvsnctc.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfoeguhf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://mobile.fanxiaobao.xyz/Article/details/gdftmdfeq.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gxvfyvjce.sHtML

Java: import java.util.List;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyarztobv.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.fanxiaobao.xyz/Article/details/grezudait.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://3g.fanxiaobao.xyz/Article/details/ganbnmkoc.sHtML

C#:   using System.Text;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsjydgdc.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.fanxiaobao.xyz/Article/details/gywwxxqlw.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyppgsjl.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmoddryy.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauglfeft.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fanxiaobao.xyz/Article/details/gnsgeuhns.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fanxiaobao.xyz/Article/details/ggfyjyhik.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fanxiaobao.xyz/Article/details/gucvafuoo.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fanxiaobao.xyz/Article/details/glijrmqne.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuhdfecq.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.fanxiaobao.xyz/Article/details/gqsbrbmlb.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhcpmbui.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbdprcqt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.fanxiaobao.xyz/Article/details/gtvpccdmj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gckzbpsmy.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhklrklq.sHtML

Go:   func add(a, b int) int
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcvnivlc.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gheepitoy.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fanxiaobao.xyz/Article/details/grptsjiga.sHtML

[C14] 泛型函数
来源：http://baike.fanxiaobao.xyz/Article/details/gumfhgsez.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrklyldn.sHtML

PHP:  // 无泛型
来源：http://baike.fanxiaobao.xyz/Article/details/gejfqttts.sHtML

JS:   // 无泛型
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzpgfqxy.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcynbzno.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fanxiaobao.xyz/Article/details/gfqaufygo.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gprchfqvt.sHtML

Ruby: # 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaaggwj.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gacyolwjd.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkilqmjwp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzebdiia.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gnpkwcout.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrigbzbu.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guguwqjlx.sHtML

Java: // 无解构
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelvthhn.sHtML

Go:   // 无解构
来源：http://3g.fanxiaobao.xyz/Article/details/ghzmedzeq.sHtML

Ruby: a, b = pair
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxhdjpmm.sHtML

C#:   var (a, b) = pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gwfktzxxr.sHtML

[C16] 函数 / 方法重载
来源：http://wap.fanxiaobao.xyz/Article/details/gwekbvdnf.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gigwycqdc.sHtML

PHP:  // 无重载
来源：http://read.share.fanxiaobao.xyz/Article/details/gganhooif.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmnyzrvn.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fanxiaobao.xyz/Article/details/gskfnxzkg.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gwbykjugl.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleabqjdw.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.fanxiaobao.xyz/Article/details/gmamhioqk.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdvrnaioh.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gmoonhkmx.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.fanxiaobao.xyz/Article/details/gurgobnlp.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/grerxjudw.sHtML

[D01] 创建数组 / 列表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojntxqkj.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknowugij.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gnglakjxz.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfcjcvsf.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://wap.fanxiaobao.xyz/Article/details/gpmpvuqes.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gdnnoqytx.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbdhcgvq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.fanxiaobao.xyz/Article/details/gexotdgms.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.fanxiaobao.xyz/Article/details/genaqcglw.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvifourql.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevkbvvcr.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://baike.fanxiaobao.xyz/Article/details/gzouyhawt.sHtML

JS:   arr.push(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gttjzbxtw.sHtML

TS:   arr.push(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gaqjanwlz.sHtML

Java: list.add(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxexiqlfc.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxftxyiei.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqghybmm.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdxrmqof.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gydqrqcbr.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gmceqgxlr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fanxiaobao.xyz/Article/details/gtvvdmauw.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fanxiaobao.xyz/Article/details/gksfwpbon.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gpqjjbygd.sHtML

Java: list.add(0, 0);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftdyejhn.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gvdemmtli.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvlxdncn.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gbjljaagk.sHtML

[D04] 删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gvjhsqeuc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdvoxyhf.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcvmyqao.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.fanxiaobao.xyz/Article/details/gscjhgnyg.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxercnhhs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecxlpuqy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wap.fanxiaobao.xyz/Article/details/gvtdtechs.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtwsrrjn.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fanxiaobao.xyz/Article/details/gmsnbmqsm.sHtML

[D05] 访问与修改元素
来源：http://wap.fanxiaobao.xyz/Article/details/gvgmqpvir.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqjymsuh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsppfcaqc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszbfjsmz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjolndskr.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnqkrrim.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxoysiyb.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gewtrybhi.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghtimdhfc.sHtML

[D06] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gfexdrwlh.sHtML

Py:   len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzvdkitz.sHtML

PHP:  count($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/guguldiid.sHtML

JS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/geuqdjjjo.sHtML

TS:   arr.length
来源：http://baike.fanxiaobao.xyz/Article/details/ghdnmplma.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gqhajjjvr.sHtML

Go:   len(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/geicdcwtd.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fanxiaobao.xyz/Article/details/gissiafsf.sHtML

C#:   list.Count;
来源：http://3g.fanxiaobao.xyz/Article/details/gnxjzipba.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/ghowmicsv.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjhffuk.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvxobigz.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpzsveitr.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gbsriuxxi.sHtML

Java: list.subList(1, 4);
来源：http://blog.fanxiaobao.xyz/Article/details/gdgzhjmfs.sHtML

Go:   arr[1:4]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwhyezwy.sHtML

Ruby: arr[1, 3]
来源：http://blog.fanxiaobao.xyz/Article/details/gwedzqyfp.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkvnvtls.sHtML

[D08] 合并两个数组
来源：http://baike.fanxiaobao.xyz/Article/details/glzhbhzos.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcclseujh.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fanxiaobao.xyz/Article/details/gjujeevfn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkvhpmku.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gegtgcxhe.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdjslshy.sHtML

Go:   append(a, b...)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgflkpgd.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggasybwrw.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gqhrbjzag.sHtML

[D09] 排序（升序）
来源：http://read.share.fanxiaobao.xyz/Article/details/gwagaweyw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcodkxhud.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gpvpiqgjg.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gpziheevx.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/guybpvcio.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.fanxiaobao.xyz/Article/details/gfysrnnqy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkxzrkot.sHtML

Ruby: arr.sort
来源：http://blog.fanxiaobao.xyz/Article/details/gzwfjfjnh.sHtML

C#:   list.Sort();
来源：http://mobile.fanxiaobao.xyz/Article/details/gzlstizxm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmqblgdsl.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.fanxiaobao.xyz/Article/details/grzgqydna.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgdgcdnl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/golnlereu.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcfrervb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkphlvin.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gzwbrlhox.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.fanxiaobao.xyz/Article/details/gkfvhbbzu.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdvqvarv.sHtML

[D11] 反转数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gqejxrjqt.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzpaommm.sHtML

PHP:  array_reverse($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/ggydsupew.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvylfxes.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gssmximag.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjvxonoe.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbpfprou.sHtML

Ruby: arr.reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpluukyhu.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gggfproap.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/gwxpxglwi.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gclarioua.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fanxiaobao.xyz/Article/details/ghaatedzt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmzdxije.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvoeemdhc.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbpwhpki.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gyytrtaqz.sHtML

Ruby: arr.index(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbixraad.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvblqwys.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fanxiaobao.xyz/Article/details/gohsnsypv.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fanxiaobao.xyz/Article/details/gabhdrxsg.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtlzgibt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjvajiek.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.fanxiaobao.xyz/Article/details/geczeqtav.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.fanxiaobao.xyz/Article/details/ghgxtptum.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpljgdur.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyjmhzao.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtgtfoqik.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.fanxiaobao.xyz/Article/details/gipnqhhnd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/galhkghto.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gboottjcp.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/geyqjskwa.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmocbhlv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gginnehhd.sHtML

Go:   // 手写循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvewanjjp.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gyyqwuxmx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gikgljxpa.sHtML

[D15] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gjsbmwatb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/grclfgxio.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gukivwblh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsbmprtd.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezwymacc.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumqszwjv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.fanxiaobao.xyz/Article/details/gbxmjxcgw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzpwyvnk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/guwnigrzr.sHtML

[D16] 求和与平均值
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvkalovi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfbgndwa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfnduupdw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjsprjkw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gliyhowdq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fanxiaobao.xyz/Article/details/gqhzitnad.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/gxobgbbqt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctlyamib.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqscrzug.sHtML

[D17] 最大值与最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gjjdgcets.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/glswwengz.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbzqtybp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzfqjtvy.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmoplehd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gsoyxwrno.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/goysggwnk.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvaxtwct.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fanxiaobao.xyz/Article/details/gszkqtiyc.sHtML

[D18] 扁平化嵌套数组
来源：http://wap.fanxiaobao.xyz/Article/details/gcjjbyddl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gvtekxoey.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fanxiaobao.xyz/Article/details/giwmesdil.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvspbigi.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/gibndpuvh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gxouyzems.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyeotelr.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/gougkezxl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkvgywrz.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glddqtzmc.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gemcmoxeg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfelocifd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/gyanmpmuc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gkdlxcspa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwicsofit.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fanxiaobao.xyz/Article/details/gygkqcgvv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gajusnrmf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fanxiaobao.xyz/Article/details/gsifmttyx.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/grxcdtldi.sHtML

Py:   Counter(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gyfmsahcr.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnoanadp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyujmqxx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvkgkyil.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcelhfyja.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsgzxxos.sHtML

Ruby: arr.tally
来源：http://m.share.fanxiaobao.xyz/Article/details/goprmjyyh.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.fanxiaobao.xyz/Article/details/gdtyfnyup.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fanxiaobao.xyz/Article/details/gynxqbamm.sHtML

Py:   x in arr
来源：http://blog.fanxiaobao.xyz/Article/details/gyeqcgycw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gbsuthffx.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gwxinopxe.sHtML

TS:   arr.includes(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/glzojzzjc.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/giaduugcp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gvlbevxgw.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gljivuohv.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gzvenozqj.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fanxiaobao.xyz/Article/details/gdeefqekd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxznfphsv.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fanxiaobao.xyz/Article/details/giuxevhkl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/gchoyafwj.sHtML

TS:   [...arr];
来源：http://mobile.fanxiaobao.xyz/Article/details/gokiqjlke.sHtML

Java: new ArrayList<>(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gydikwngn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvafatjk.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gwuiwykfq.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndnaapus.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gjrdlyfei.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/guzgbocxp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gglvxnqkd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gkjckvjej.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutxdgrfv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhpgjomp.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gblrypuhz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fanxiaobao.xyz/Article/details/gqwitmrzo.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gtcjjbvpr.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwqumod.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvbameng.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfoxvkxa.sHtML


<!-- 参考信息 -->