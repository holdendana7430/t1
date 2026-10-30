代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/gscmnvjga.sHtML

[C07] 把函数作为参数传入
来源：http://read.share.hesvh.cn/Article/details/gjvoemlsy.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://baike.fehbvm.com/Article/details/gkyznkigd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/ggcwygkre.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/gqouepazr.sHtML

TS:   arr.map(String)
来源：http://www.blog.hesvh.cn/Article/details/gpbhsdegj.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://mobile.zdbjq.cn/Article/details/gvfqhgfqd.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://wap.fehbvm.com/Article/details/ghnxjailu.sHtML

Ruby: arr.map(&:upcase)
来源：http://mobile.fehbvm.com/Article/details/gskxehwhq.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/giwmuudnj.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/gxtyfopdo.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://read.share.hesvh.cn/Article/details/ggcejpvlw.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.zdbjq.cn/Article/details/gtljaxfmk.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gfsyupzip.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://mobile.hesvh.cn/Article/details/gmgrirxds.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://blog.fehbvm.com/Article/details/ggtnbyqrq.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.m.share.hesvh.cn/Article/details/gbqsbkhki.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://wap.hesvh.cn/Article/details/gtdaqwuuw.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.fehbvm.com/Article/details/gppjimtlm.sHtML

[C09] 递归
来源：http://3g.fehbvm.com/Article/details/gifwrdwgy.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.hesvh.cn/Article/details/gheofyijy.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/guholoift.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.hesvh.cn/Article/details/gukouzudy.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.zdbjq.cn/Article/details/giegewqwm.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.blog.zdbjq.cn/Article/details/guxvpsroj.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/gdwfllriw.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gcrupblxp.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://blog.zdbjq.cn/Article/details/giiedbozm.sHtML

[C10] 变量作用域
来源：http://blog.fehbvm.com/Article/details/ghsvctgzi.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.fehbvm.com/Article/details/godxrimnf.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.hesvh.cn/Article/details/gzvhqzigw.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gefymzovz.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gmsrukqfk.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.hesvh.cn/Article/details/ghzzeqlun.sHtML

Go:   花括号块级作用域
来源：http://www.blog.hesvh.cn/Article/details/gqvhssnkg.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gfnjankbp.sHtML

C#:   块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggwudmtte.sHtML

[C11] 模块导入与导出
来源：http://www.blog.hesvh.cn/Article/details/gnjvcesro.sHtML

Py:   from module import func
来源：http://www.share.zdbjq.cn/Article/details/gbkxmhgej.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fehbvm.com/Article/details/gxkyjldtq.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gsobiftmp.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gocedygxw.sHtML

Java: import java.util.List;
来源：http://3g.hesvh.cn/Article/details/gquayojte.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gxpojimof.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.hesvh.cn/Article/details/gmwjbeobu.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gaztwmnym.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.fehbvm.com/Article/details/ghrqvkdaw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gwamsinyf.sHtML

PHP:  (function () { echo "run"; })();
来源：http://wap.hesvh.cn/Article/details/gqcagouhp.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.fehbvm.com/Article/details/gwyzeyvgx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/gtdactfzn.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/girxnwwim.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.share.zdbjq.cn/Article/details/glmsneamk.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gskucasmo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.fehbvm.com/Article/details/gpdiczvjr.sHtML

[C13] 类型声明 / 类型注解
来源：http://blog.zdbjq.cn/Article/details/gpwpifdle.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://mobile.fehbvm.com/Article/details/gezmufxom.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gnsfssuzm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/grncfbyaa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gfsgqagtl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gptnsknjd.sHtML

Go:   func add(a, b int) int
来源：http://www.share.zdbjq.cn/Article/details/gobndrfpg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://baike.fehbvm.com/Article/details/gfhoqbpzs.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.zdbjq.cn/Article/details/gmorlgazp.sHtML

[C14] 泛型函数
来源：http://wap.zdbjq.cn/Article/details/gokkfrigo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.zdbjq.cn/Article/details/ghepoudap.sHtML

PHP:  // 无泛型
来源：http://m.share.hesvh.cn/Article/details/gofpglnxf.sHtML

JS:   // 无泛型
来源：http://www.m.share.fehbvm.com/Article/details/gzngrdisk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.zdbjq.cn/Article/details/gmyiishbd.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gjlyhbutj.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.share.hesvh.cn/Article/details/gyrxlguqg.sHtML

Ruby: # 无泛型
来源：http://baike.zdbjq.cn/Article/details/guoaexdyp.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://3g.zdbjq.cn/Article/details/gidomcjqj.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/goitayque.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.hesvh.cn/Article/details/gqyahlelp.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gihvtehhy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fehbvm.com/Article/details/gwpleltey.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fehbvm.com/Article/details/gfcofgmgj.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/gmgffzhoc.sHtML

Go:   // 无解构
来源：http://baike.hesvh.cn/Article/details/gjsciifpl.sHtML

Ruby: a, b = pair
来源：http://wap.fehbvm.com/Article/details/gnetbptoe.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.hesvh.cn/Article/details/gwcineozc.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.fehbvm.com/Article/details/gblhxxdfr.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.hesvh.cn/Article/details/gckaitocd.sHtML

PHP:  // 无重载
来源：http://blog.zdbjq.cn/Article/details/gywocpeky.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gjizztihd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.hesvh.cn/Article/details/gytiqzlxe.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.fehbvm.com/Article/details/gwixavpmy.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/govzecyfl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://blog.hesvh.cn/Article/details/gyshyqcdo.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://mobile.hesvh.cn/Article/details/gogihgxpg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gacvysywj.sHtML

D. 数组 / 列表 / 集合
来源：http://m.share.zdbjq.cn/Article/details/gpzdnkchu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghruykhtw.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/guldzwhoy.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gsmwkcrfu.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/ggpunxlnh.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://baike.hesvh.cn/Article/details/gpxfqxroz.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gvrkysgup.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://read.share.fehbvm.com/Article/details/ghyuuirkt.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gbuwbvqej.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gnweolfke.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://baike.zdbjq.cn/Article/details/gwnhbbtux.sHtML

[D02] 追加元素到末尾
来源：http://3g.fehbvm.com/Article/details/gsrbqpqva.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://baike.hesvh.cn/Article/details/gbuwnmanq.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wap.fehbvm.com/Article/details/gxsdulpnq.sHtML

JS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gauueyjzv.sHtML

TS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gdhdzzwlj.sHtML

Java: list.add(4);
来源：http://blog.zdbjq.cn/Article/details/ghfpeeywk.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.fehbvm.com/Article/details/gughvkqxh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gnwtoobxz.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gffuafwje.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gplbvmcev.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/grjcvszvg.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://m.share.fehbvm.com/Article/details/glmbpggph.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.hesvh.cn/Article/details/gucdvyejn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://blog.fehbvm.com/Article/details/gzimojeqz.sHtML

Java: list.add(0, 0);
来源：http://wap.hesvh.cn/Article/details/gragmqchr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://baike.hesvh.cn/Article/details/gbqdldjij.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://3g.zdbjq.cn/Article/details/golsewdps.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.fehbvm.com/Article/details/gpwmjdscc.sHtML

[D04] 删除元素
来源：http://www.share.zdbjq.cn/Article/details/gnosfltnu.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.fehbvm.com/Article/details/gzlyiurub.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.zdbjq.cn/Article/details/gzrsvjjhk.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://baike.zdbjq.cn/Article/details/getbdawyz.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.hesvh.cn/Article/details/gcyxextuq.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gfchflsrb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://blog.hesvh.cn/Article/details/gsrtihegy.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.m.share.zdbjq.cn/Article/details/ggydnzxwc.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://read.share.hesvh.cn/Article/details/gujnzexoe.sHtML

[D05] 访问与修改元素
来源：http://www.share.hesvh.cn/Article/details/gjdcnmjuk.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gkntvxbjf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfupebqsa.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gyvtpvdty.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/gzfisrivi.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.hesvh.cn/Article/details/grphcgprs.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gjeysmzya.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/ggzljnnvy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.zdbjq.cn/Article/details/gzndecytl.sHtML

[D06] 数组长度
来源：http://mobile.fehbvm.com/Article/details/gzoqyylys.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbinaqsag.sHtML

PHP:  count($arr);
来源：http://mobile.hesvh.cn/Article/details/gikohiskm.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/ggxcrokvt.sHtML

TS:   arr.length
来源：http://blog.hesvh.cn/Article/details/gvbjxwqtv.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gbujrmqwg.sHtML

Go:   len(arr)
来源：http://baike.zdbjq.cn/Article/details/gvnflvwhs.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.fehbvm.com/Article/details/gdikzlkqw.sHtML

C#:   list.Count;
来源：http://www.m.share.zdbjq.cn/Article/details/glbiuggxl.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.fehbvm.com/Article/details/gxblnumut.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.hesvh.cn/Article/details/gnvupdraf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gfjggsnlc.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.zdbjq.cn/Article/details/gkacacryr.sHtML

TS:   arr.slice(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gxpooxuuz.sHtML

Java: list.subList(1, 4);
来源：http://wap.fehbvm.com/Article/details/gkdzhzsps.sHtML

Go:   arr[1:4]
来源：http://www.share.zdbjq.cn/Article/details/gwlxfljgx.sHtML

Ruby: arr[1, 3]
来源：http://read.share.fehbvm.com/Article/details/gyhpqvhfw.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gxapecvms.sHtML

[D08] 合并两个数组
来源：http://3g.fehbvm.com/Article/details/ghtnwzvpm.sHtML

Py:   a + b;  a.extend(b)
来源：http://3g.zdbjq.cn/Article/details/gdfbhklct.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gzopaxrdv.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.share.zdbjq.cn/Article/details/glfolovdb.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gskupgmsf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.hesvh.cn/Article/details/gpcuvwqgj.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gysqzuudq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/gyjwlrtza.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.zdbjq.cn/Article/details/gybuqwvzg.sHtML

[D09] 排序（升序）
来源：http://mobile.hesvh.cn/Article/details/grfxesehk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gplfeonsi.sHtML

PHP:  sort($arr);
来源：http://read.share.hesvh.cn/Article/details/gwkhylyhl.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.fehbvm.com/Article/details/gzznsjuwu.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.zdbjq.cn/Article/details/gzabidtuq.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://m.share.hesvh.cn/Article/details/gmftztsnr.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gzcblrmgs.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gyuuuhtpu.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gzewgchvi.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gnzejluze.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fehbvm.com/Article/details/gzkcanylg.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.hesvh.cn/Article/details/gbqjemwvz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gvudokouf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.hesvh.cn/Article/details/gzuuvsafk.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.hesvh.cn/Article/details/guqaykqss.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.zdbjq.cn/Article/details/gsmlgpbur.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gokaiiijs.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.zdbjq.cn/Article/details/gwtqllaap.sHtML

[D11] 反转数组
来源：http://baike.fehbvm.com/Article/details/ghqmulncq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.hesvh.cn/Article/details/gaepngbnw.sHtML

PHP:  array_reverse($arr);
来源：http://baike.fehbvm.com/Article/details/gwywtdzpv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gynkfheno.sHtML

TS:   [...arr].reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gccingeku.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gbawfukvd.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.fehbvm.com/Article/details/gqzeiwtrm.sHtML

Ruby: arr.reverse
来源：http://www.blog.fehbvm.com/Article/details/gerutavfs.sHtML

C#:   list.Reverse();
来源：http://blog.hesvh.cn/Article/details/gkptyjxur.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gijywiuaz.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gapwzpvjg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gxhpofwlw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gpmkugqnm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gjhsfzeax.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gqnynebri.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqxmrfxjv.sHtML

Ruby: arr.index(x)
来源：http://www.share.zdbjq.cn/Article/details/ghzowasrz.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.zdbjq.cn/Article/details/gbpvlmnag.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.zdbjq.cn/Article/details/ghkziyyon.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gjvqododx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gfpvxxtqi.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gttyjcfvd.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gnhyxdjln.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gwoqhoppm.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gtgvuuyqk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gbwywxibj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gwgxfvcfj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/gxfqjdzrs.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/guklxvwbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/gzojgyoni.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gfrvixovq.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gikihazah.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gnbqisrkb.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/geahyfnff.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.zdbjq.cn/Article/details/gfaybcxlb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/gzwxuseke.sHtML

[D15] 去重
来源：http://baike.zdbjq.cn/Article/details/gwgifjnsn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gvatwjppu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/guibnvfiy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gfluqsmzp.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gbvbekjro.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gaznccmuj.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/geurvvhiw.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gymwqffnl.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.zdbjq.cn/Article/details/ghoalbhba.sHtML

[D16] 求和与平均值
来源：http://read.share.fehbvm.com/Article/details/grwwsbvzq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glfulfpsd.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/gpcmxjzpk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gkogouhkx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/giydlygho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gfpxgdwec.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gkhaaeedv.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/goonssmxh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gdiyctkrx.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gkkcezacr.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.hesvh.cn/Article/details/gwbwwdrdm.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/graolrptl.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gcryluuvp.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gbxdlbsja.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/guumrjiog.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/guswohpvl.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/gwfrxnhdu.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/geqtxrkzn.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fehbvm.com/Article/details/gzyiolpgk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/guksdauon.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gmukhpfwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gxzfgkoni.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/gcrrqjnde.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gmgghdxse.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/gqfrzhopx.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gcpmucxji.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/grejmiaog.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gupxzbrmx.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gbqfdakyo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gtfeihvho.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gdvjxdhsp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gkxxauwyl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gfzbhtjyl.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gzqpnsiww.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gdixpereg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gselcuyyw.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gwrjcaagk.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gbeeknzkh.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gvurxinyh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gesivxsys.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gvnamzfvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/giuaoctpd.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gzwyqxhcy.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gxlotxrte.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ghbalccge.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/guhxgwdxh.sHtML

Py:   x in arr
来源：http://3g.hesvh.cn/Article/details/gqtwhuqrk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/gaaqlybla.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gqpwobjow.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/ggdqjxcot.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghusitvhp.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gfadpgsag.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gakahympi.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/geyyotfpg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gsadjmqgf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.zdbjq.cn/Article/details/gdnxgvdkc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/goukinyky.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gyoiotata.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gegytxycs.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gdnavettx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fehbvm.com/Article/details/gbujsocar.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gdlvlnasb.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gvfyfueid.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gmtrffblq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/grejowbsv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/glhfrebux.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gfpaartoe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gzcmihdkk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gvlkwstfc.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gnuhxucar.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gharmgsbd.sHtML


<!-- 参考信息 -->