代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://blog.hesvh.cn/Article/details/gpwtiqxwx.sHtML

TS:   arr.map(String)
来源：http://baike.fehbvm.com/Article/details/gpkwpqmic.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://baike.zdbjq.cn/Article/details/gjoidelnh.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://m.share.zdbjq.cn/Article/details/gukwevccy.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.hesvh.cn/Article/details/gbvddsuxk.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://wap.hesvh.cn/Article/details/grvpmvxlv.sHtML

[C08] 闭包
来源：http://wap.fehbvm.com/Article/details/gpeezeood.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://wap.zdbjq.cn/Article/details/gctxkeobt.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/goysrkmep.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.share.hesvh.cn/Article/details/gtzwstkls.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.blog.fehbvm.com/Article/details/gdfhpleuv.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.zdbjq.cn/Article/details/grbkaaqad.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.share.hesvh.cn/Article/details/gsniaultv.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://blog.hesvh.cn/Article/details/gxcmfxked.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/gxiqitsrh.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gmxdavbxr.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://m.share.zdbjq.cn/Article/details/gkgmmffto.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://baike.fehbvm.com/Article/details/gyyoybdgg.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gauyumvin.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gfamhaajk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://blog.hesvh.cn/Article/details/gljobxhrv.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.fehbvm.com/Article/details/getvbllpd.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gzrgzmzmm.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gkgqefvzg.sHtML

[C10] 变量作用域
来源：http://read.share.fehbvm.com/Article/details/gzglnlrzj.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.fehbvm.com/Article/details/glzmyloqy.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.hesvh.cn/Article/details/gxgstjhye.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.m.share.zdbjq.cn/Article/details/glkwtejnw.sHtML

TS:   同 JS
来源：http://baike.fehbvm.com/Article/details/ggwsinrnf.sHtML

Java: 方法内为块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ggituvqrg.sHtML

Go:   花括号块级作用域
来源：http://m.share.zdbjq.cn/Article/details/glpaircln.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.fehbvm.com/Article/details/gdcvdcipj.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gywrpxklz.sHtML

[C11] 模块导入与导出
来源：http://mobile.zdbjq.cn/Article/details/gopaugsct.sHtML

Py:   from module import func
来源：http://m.share.zdbjq.cn/Article/details/gjqqvyrce.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gobjenbhf.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gigayqqvp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/geuvdhsgt.sHtML

Java: import java.util.List;
来源：http://www.blog.zdbjq.cn/Article/details/gmlelnqzk.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/gjsbjawbe.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://mobile.hesvh.cn/Article/details/gepmvimqd.sHtML

C#:   using System.Text;
来源：http://read.share.zdbjq.cn/Article/details/gyhofyycd.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gbrkabvpq.sHtML

Py:   (lambda: print("run"))()
来源：http://www.share.fehbvm.com/Article/details/gcunqdkkn.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.hesvh.cn/Article/details/glbvkdndp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gqnbvtkqc.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/glhezzyty.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/gvqzejoie.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/godkllphk.sHtML

Ruby: -> { puts "run" }.call
来源：http://read.share.hesvh.cn/Article/details/gigswajzd.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/gjwdqyawm.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.hesvh.cn/Article/details/gpxddmfrc.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gqojbzdoo.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fehbvm.com/Article/details/gnxbyesyr.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fehbvm.com/Article/details/gdpqdenqr.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.hesvh.cn/Article/details/gntjqqsjf.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.fehbvm.com/Article/details/gusqvlaar.sHtML

Go:   func add(a, b int) int
来源：http://www.share.hesvh.cn/Article/details/ggmmambmq.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.zdbjq.cn/Article/details/gkrmvxqdi.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://m.share.hesvh.cn/Article/details/gvnljhnsu.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gflwdclea.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gaeuimkun.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gebwtqedj.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gibdxswmg.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.fehbvm.com/Article/details/gtnesrxbb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.fehbvm.com/Article/details/ghsvphaly.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.blog.zdbjq.cn/Article/details/gulwklyyo.sHtML

Ruby: # 无泛型
来源：http://3g.hesvh.cn/Article/details/gzkhsqrue.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gvdaiqqef.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gghxbyjcv.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.blog.fehbvm.com/Article/details/glahenllt.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.hesvh.cn/Article/details/gsdeaxnuf.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.zdbjq.cn/Article/details/gepimlqkn.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://read.share.hesvh.cn/Article/details/gnyfhlxjl.sHtML

Java: // 无解构
来源：http://wap.fehbvm.com/Article/details/gindhyctp.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gxqengicg.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gofknrrlx.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gqfqtjjse.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.zdbjq.cn/Article/details/gvxmhqtbt.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://baike.fehbvm.com/Article/details/gphkjzmdp.sHtML

PHP:  // 无重载
来源：http://mobile.hesvh.cn/Article/details/gvjhckzxs.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.hesvh.cn/Article/details/guzofazvw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.fehbvm.com/Article/details/grpqkrzpt.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://mobile.fehbvm.com/Article/details/gkfpdkpzw.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gggksxotq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gnxbhepjd.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.zdbjq.cn/Article/details/godrtcmnk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gngghprdi.sHtML

D. 数组 / 列表 / 集合
来源：http://www.m.share.fehbvm.com/Article/details/geeeezqya.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnjidczte.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.hesvh.cn/Article/details/gptesaclb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.zdbjq.cn/Article/details/glbmniwei.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://m.share.hesvh.cn/Article/details/gklagiswa.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/gzrdclfip.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.m.share.fehbvm.com/Article/details/gygjyvgjy.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.zdbjq.cn/Article/details/grfqewsno.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.hesvh.cn/Article/details/gibhackgc.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/glfzflejq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fehbvm.com/Article/details/ggjurzybo.sHtML

[D02] 追加元素到末尾
来源：http://wap.hesvh.cn/Article/details/gisawlcvr.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://blog.zdbjq.cn/Article/details/ggihbzvrv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.hesvh.cn/Article/details/gvmthxusn.sHtML

JS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghldbuyvg.sHtML

TS:   arr.push(4);
来源：http://3g.hesvh.cn/Article/details/gatqlkrsc.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gpbgyrgxr.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.fehbvm.com/Article/details/gwihinqas.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.hesvh.cn/Article/details/gjpfhmjdl.sHtML

C#:   list.Add(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gwuwhqmrt.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/ghixkowuh.sHtML

Py:   arr.insert(0, 0)
来源：http://m.share.hesvh.cn/Article/details/gjpoknkuj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://read.share.zdbjq.cn/Article/details/gvdlwjyfe.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.zdbjq.cn/Article/details/gsfzpnczh.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.hesvh.cn/Article/details/guzzzwpct.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gkzqlpezx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.fehbvm.com/Article/details/grprolbyq.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/ghezpvcyq.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/goltyjubq.sHtML

[D04] 删除元素
来源：http://3g.hesvh.cn/Article/details/giezhbfaa.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.fehbvm.com/Article/details/gpgsdekio.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.share.hesvh.cn/Article/details/grahmefsx.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gtycwbdht.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fehbvm.com/Article/details/ghlhddwjs.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mobile.zdbjq.cn/Article/details/grwahfkxu.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.blog.fehbvm.com/Article/details/gqbygehrd.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.zdbjq.cn/Article/details/grvcchpvj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.fehbvm.com/Article/details/gbaokggjd.sHtML

[D05] 访问与修改元素
来源：http://3g.fehbvm.com/Article/details/gpkbtzbrq.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gmktjimvu.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gkgdlpebz.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gaqmnnvkc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.hesvh.cn/Article/details/ghdaumkdg.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.zdbjq.cn/Article/details/ggsfdfwbv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.share.hesvh.cn/Article/details/gwpglznmg.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/govixtgxu.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://m.share.fehbvm.com/Article/details/gylikemzs.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gkqexcios.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gxnzarxrw.sHtML

PHP:  count($arr);
来源：http://baike.zdbjq.cn/Article/details/gbciokxfa.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gxxumauyl.sHtML

TS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gpbbvkiei.sHtML

Java: list.size();
来源：http://m.share.fehbvm.com/Article/details/gtmcabtvb.sHtML

Go:   len(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcqpitgal.sHtML

Ruby: arr.length; arr.size
来源：http://baike.fehbvm.com/Article/details/gvphnrdai.sHtML

C#:   list.Count;
来源：http://m.share.zdbjq.cn/Article/details/guswzpqvd.sHtML

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gazwzspwa.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gojbpirkj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/ggjftzone.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.fehbvm.com/Article/details/gyczycpfn.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gwjiuzlhk.sHtML

Java: list.subList(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gwbpsgugg.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gnowtlgpu.sHtML

Ruby: arr[1, 3]
来源：http://www.m.share.zdbjq.cn/Article/details/gyxtbocjw.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.fehbvm.com/Article/details/gwdptvgga.sHtML

[D08] 合并两个数组
来源：http://www.share.zdbjq.cn/Article/details/giriazhwj.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fehbvm.com/Article/details/gzbindgvp.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.zdbjq.cn/Article/details/gvrfzvwxt.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gjqrjdtvc.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/grpwxnqvd.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.hesvh.cn/Article/details/gggmamfes.sHtML

Go:   append(a, b...)
来源：http://read.share.hesvh.cn/Article/details/gpgmeflpm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://baike.hesvh.cn/Article/details/grkxgaqds.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/glsojejar.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gkyhbjpwp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gjazexpxw.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gcmqlzuov.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.hesvh.cn/Article/details/glrtfrdgm.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gvudadwmf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gtylksujs.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gftmvnwch.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gkqguxswp.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gcwmbvbhv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gnqrwcdya.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gmtrxcruz.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.zdbjq.cn/Article/details/gwxrpijsx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gkwokodms.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.zdbjq.cn/Article/details/gskbhltsz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gvrqnhhok.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.fehbvm.com/Article/details/gymtzahyd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhbqwmxo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/ggzgnpzst.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/grblyvpiz.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gfohnslnv.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giggyxnog.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/guubnnfaz.sHtML

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gvpwhtvpt.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gsqbagskw.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gnljmoeuw.sHtML

Ruby: arr.reverse
来源：http://baike.hesvh.cn/Article/details/gzilovnal.sHtML

C#:   list.Reverse();
来源：http://www.blog.fehbvm.com/Article/details/gmjlhcngl.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/gwnrlhgmu.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/goppygami.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/glcyulpjt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.zdbjq.cn/Article/details/glpyrzawt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.zdbjq.cn/Article/details/gxtgyjoyf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/grnssexsv.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gkjijdsby.sHtML

Ruby: arr.index(x)
来源：http://blog.fehbvm.com/Article/details/gkcuqsbpt.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.hesvh.cn/Article/details/gjofpmpjy.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.hesvh.cn/Article/details/ggigvpxnk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/geijqltkc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gexzxoepu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.hesvh.cn/Article/details/gdghhtbat.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gvbehwhcj.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.zdbjq.cn/Article/details/gkpkeaoph.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.hesvh.cn/Article/details/gnmmmfidk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.zdbjq.cn/Article/details/geluyoydq.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gcjygmayq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/guhmqfzab.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gqkxnqryc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/gyoztoduf.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gpzfxtyun.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fehbvm.com/Article/details/gskcikikr.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gnwmhypwi.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gyarzvxvy.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gsiyugesx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/glmbgfpgz.sHtML

[D15] 去重
来源：http://read.share.hesvh.cn/Article/details/ghxsmxith.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gyjvskglx.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/ghhljcowc.sHtML

JS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/gzndqssdb.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ghcmuhqeh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gzapcqvzi.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gnxmxaxfh.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gncsrcojm.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gozpmwfga.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gdharhkdl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gceqkwzlz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gvskrwvzp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdsmbokkj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/gtyacydnw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gglfcmljm.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gvoqjznwm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/guxxqrczp.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gasxlxjvb.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/ggpzemgvq.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gblrlnzmu.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gutcjiazz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gfxkcpupo.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/grnqsjgeh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gbpjmbnmj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gvxicivtc.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.fehbvm.com/Article/details/gpwoittel.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gesoldwbo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/ghtptfqdu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.fehbvm.com/Article/details/gfbghpimy.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.hesvh.cn/Article/details/gzjqkpccu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gifiyfotb.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gxqoorsnj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.hesvh.cn/Article/details/gevrxyzcf.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gxmehqmsz.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/glzykmujo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.fehbvm.com/Article/details/gqvvgqjuc.sHtML

[D19] 按字段分组
来源：http://3g.hesvh.cn/Article/details/ghbwvjlcl.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gyhvjbnbs.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/guvgxdhno.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gfssjxlrt.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gtnwkdhmb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gyfneykny.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.hesvh.cn/Article/details/gyjfpmkcb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gjnlxjdsu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gyiixpxly.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gysketuiv.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gxocirmku.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/grlbkzqwg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gwsohhkxv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gsvyqzowd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.hesvh.cn/Article/details/gajxqqtpp.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gwbnkpnbh.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/geqkutlsf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gqvicgsjx.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/ghyarnenf.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/graukfqok.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gqjiawshf.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gvcekwbjd.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gwlwkzwtb.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/grqpajucb.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/grprkuyrq.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gfaihhfxc.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gufpunarl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gusxvbztj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gyssjqdzn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gahhwkkoc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gnmmhbwxf.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gqpjuxbgz.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gfqzydmmc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.fehbvm.com/Article/details/gxuwysvyr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gdlyzgstw.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gyvtncjqy.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gmztvzhuw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gnszugimd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gbnftcxoi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gqchjzvet.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gkdricnpy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gxvxnvtna.sHtML

Go:   // 手写循环
来源：http://www.blog.zdbjq.cn/Article/details/gdppsursa.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gcyhwpoct.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gfzcgfffv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.fehbvm.com/Article/details/geyapbmeq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/gwrfzoano.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gufeggcro.sHtML


<!-- 参考信息 -->