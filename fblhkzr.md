代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.zdbjq.cn/Article/details/gsmdybbxh.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://baike.fehbvm.com/Article/details/gwnmqvywd.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gvwauemoj.sHtML

[C09] 递归
来源：http://mobile.zdbjq.cn/Article/details/gqdzbvhlq.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.share.zdbjq.cn/Article/details/ggnlpdiet.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://wap.hesvh.cn/Article/details/gtlhqtihz.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gbrhvdxpa.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.share.fehbvm.com/Article/details/gtgqfxejh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://m.share.hesvh.cn/Article/details/gbqbtswoh.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://baike.zdbjq.cn/Article/details/guchlronf.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://blog.hesvh.cn/Article/details/gpmydusxk.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.hesvh.cn/Article/details/gjvqkhjuu.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gyfcuivtn.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://m.share.zdbjq.cn/Article/details/gqqtxbigm.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://mobile.zdbjq.cn/Article/details/gnxmmhrjp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gbyrsqoko.sHtML

TS:   同 JS
来源：http://baike.zdbjq.cn/Article/details/gcgtoxukh.sHtML

Java: 方法内为块级作用域
来源：http://3g.fehbvm.com/Article/details/gfqrlyhgt.sHtML

Go:   花括号块级作用域
来源：http://baike.hesvh.cn/Article/details/gkyxqlovm.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://read.share.zdbjq.cn/Article/details/gbrtimejv.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gaabpmxws.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gdrkgytlg.sHtML

Py:   from module import func
来源：http://wap.fehbvm.com/Article/details/gnqiegtzk.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.zdbjq.cn/Article/details/gsfvutago.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.zdbjq.cn/Article/details/gghtbmivo.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/gqlxkezwk.sHtML

Java: import java.util.List;
来源：http://www.m.share.fehbvm.com/Article/details/gfziemfly.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.zdbjq.cn/Article/details/gavffuomm.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gikeujqpj.sHtML

C#:   using System.Text;
来源：http://read.share.fehbvm.com/Article/details/gafgdedsa.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.zdbjq.cn/Article/details/gfspljmwx.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.fehbvm.com/Article/details/ggtldvjbp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.hesvh.cn/Article/details/gimexqsnt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gcaewjmmg.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.zdbjq.cn/Article/details/gahxphdir.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/grwrgnjlp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.m.share.fehbvm.com/Article/details/gwhkvyptf.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.fehbvm.com/Article/details/gnolxlsnj.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://3g.zdbjq.cn/Article/details/gohassuyy.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gwrqjfqdp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.zdbjq.cn/Article/details/ghuenzgle.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://baike.hesvh.cn/Article/details/gvzuvfcmk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.hesvh.cn/Article/details/gblpsmvti.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpjjmqrrj.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gllydqlqa.sHtML

Go:   func add(a, b int) int
来源：http://wap.hesvh.cn/Article/details/gbamnfqvi.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.zdbjq.cn/Article/details/gvlggynmz.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gzymfkxjf.sHtML

[C14] 泛型函数
来源：http://3g.hesvh.cn/Article/details/gedrpjauv.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://read.share.hesvh.cn/Article/details/gopcyynaa.sHtML

PHP:  // 无泛型
来源：http://baike.fehbvm.com/Article/details/gbhpoynuh.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gvryvxist.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/glozibsum.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.hesvh.cn/Article/details/gipdhhcqw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gqjaufybk.sHtML

Ruby: # 无泛型
来源：http://read.share.fehbvm.com/Article/details/gbppcgiwt.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fehbvm.com/Article/details/grsfuritq.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gvcnoxziq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.hesvh.cn/Article/details/gkqlsalag.sHtML

PHP:  [$a, $b] = $pair;
来源：http://wap.fehbvm.com/Article/details/gdbhcyuje.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gzqzbjhlf.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://mobile.fehbvm.com/Article/details/gqrtphlsy.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/getheluxo.sHtML

Go:   // 无解构
来源：http://www.share.fehbvm.com/Article/details/gpyzpabwx.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gmktbwdmg.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.fehbvm.com/Article/details/guhenbzqa.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gopkosovc.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://wap.fehbvm.com/Article/details/gbgkorwtx.sHtML

PHP:  // 无重载
来源：http://m.share.hesvh.cn/Article/details/getqjhgpn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gqsntbtqy.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/goicdukqo.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fehbvm.com/Article/details/glsfwsuhq.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.hesvh.cn/Article/details/gtnbppxdl.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gttdgbbas.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/goxszwwma.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvrexryir.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.hesvh.cn/Article/details/glvfdwjmo.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grnyxqomb.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gkaaltljo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gtfpqlzil.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.hesvh.cn/Article/details/gmzmbvlkk.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gskxuhfdk.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.zdbjq.cn/Article/details/glqirvjhn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.blog.zdbjq.cn/Article/details/gwlhoavpj.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gcmtlhkee.sHtML

Ruby: arr = [1, 2, 3]
来源：http://read.share.hesvh.cn/Article/details/gclzemerj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://read.share.hesvh.cn/Article/details/gxohvdlkq.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gefdjalmv.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.zdbjq.cn/Article/details/gjsrimdwa.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://m.share.hesvh.cn/Article/details/grkcmzekq.sHtML

JS:   arr.push(4);
来源：http://read.share.fehbvm.com/Article/details/gtbwrcvnk.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gcqqhgpdf.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/grisyadsp.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.zdbjq.cn/Article/details/gyhzdbzbe.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gqqsyqixi.sHtML

C#:   list.Add(4);
来源：http://www.blog.zdbjq.cn/Article/details/geszgwavx.sHtML

[D03] 在指定位置插入元素
来源：http://baike.zdbjq.cn/Article/details/gyipxhmdr.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/gjzgzifaq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.hesvh.cn/Article/details/gfhhbfyeh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://m.share.fehbvm.com/Article/details/goppdxshu.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gnkuajhnc.sHtML

Java: list.add(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gqborirfr.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fehbvm.com/Article/details/gcpfpyxrf.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gpmlakfid.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.hesvh.cn/Article/details/gsxnqpncu.sHtML

[D04] 删除元素
来源：http://www.blog.zdbjq.cn/Article/details/grofslmzw.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.zdbjq.cn/Article/details/gbotrkmns.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqwkkyhlc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://read.share.hesvh.cn/Article/details/gdvioekhl.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.fehbvm.com/Article/details/gfjtimbzv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.fehbvm.com/Article/details/gjjpljazw.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.hesvh.cn/Article/details/gcsagegum.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.hesvh.cn/Article/details/gjxvwxhqr.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gdenybmqy.sHtML

[D05] 访问与修改元素
来源：http://wap.zdbjq.cn/Article/details/gtzbklmpp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.hesvh.cn/Article/details/gcuvuuffy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gvzayybol.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gkspavqry.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.fehbvm.com/Article/details/gwhvdhgny.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://3g.fehbvm.com/Article/details/gusufxurv.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://wap.fehbvm.com/Article/details/gdwewvbvk.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gseqekiuk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.hesvh.cn/Article/details/goxmrcqct.sHtML

[D06] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gtvtrmipx.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/ggzfykbjr.sHtML

PHP:  count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gjaklvvbh.sHtML

JS:   arr.length
来源：http://www.m.share.fehbvm.com/Article/details/gntifintr.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/ggajsnglm.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gkelfydyi.sHtML

Go:   len(arr)
来源：http://read.share.hesvh.cn/Article/details/ghsppbpvr.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/gaatcqbyn.sHtML

C#:   list.Count;
来源：http://www.blog.fehbvm.com/Article/details/gggihwwmn.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gdgrjbijp.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.fehbvm.com/Article/details/gvedurxpt.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.fehbvm.com/Article/details/gisavpked.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gdwvkatyx.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/govrzmbsn.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gstwcsvuz.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gfgmeapkc.sHtML

Ruby: arr[1, 3]
来源：http://m.share.fehbvm.com/Article/details/gyuoamyob.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.fehbvm.com/Article/details/gqcracnij.sHtML

[D08] 合并两个数组
来源：http://baike.hesvh.cn/Article/details/gkotjxzcp.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gkeuetwlo.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.zdbjq.cn/Article/details/grkbkuduk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gyyrkimqe.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gdgvqgulc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.fehbvm.com/Article/details/gcskeqsxp.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/giyuktumm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.zdbjq.cn/Article/details/gsnxtuszk.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gtpxsgqwc.sHtML

[D09] 排序（升序）
来源：http://www.share.fehbvm.com/Article/details/gqapkajgv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/gmgwrbeur.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gusigyddj.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.m.share.zdbjq.cn/Article/details/guxkdslku.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.hesvh.cn/Article/details/gjzraqear.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gzetbisee.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gthmctgyo.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gbwdimodc.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/gwsbabpsw.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gfduvbfcp.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/grboasjrw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gbelzvedv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gzzwjlewd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gsqkpfwuq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gtajrllqc.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gipliamlx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/grdrbqnqx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/gbchrfptp.sHtML

[D11] 反转数组
来源：http://blog.fehbvm.com/Article/details/gktcbeqlv.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://baike.fehbvm.com/Article/details/gxprgzzab.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gnormmwaf.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.zdbjq.cn/Article/details/gmfkazbfn.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gcbxefmzw.sHtML

Java: Collections.reverse(list);
来源：http://mobile.zdbjq.cn/Article/details/gbygymovr.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/giscagldn.sHtML

Ruby: arr.reverse
来源：http://mobile.zdbjq.cn/Article/details/gtebmpfwd.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gdnxhxjvu.sHtML

[D12] 查找元素下标
来源：http://baike.zdbjq.cn/Article/details/gcnrzmvgb.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.fehbvm.com/Article/details/ghqchttyg.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.hesvh.cn/Article/details/gcgdexsuv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gxwsllbne.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gqlnhhfyl.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gqvcfwrhl.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gcjzavnyf.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gvofrngug.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/gailirzyq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/gkftuikwg.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gzccqucqm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.fehbvm.com/Article/details/gunqutfct.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/guhbcxsyb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gxglvolax.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gsipoyukk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/geeklvhzm.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.zdbjq.cn/Article/details/gfmpatlsa.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gjybwxoim.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.zdbjq.cn/Article/details/ggtjettxi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gtykepwic.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gcxklusls.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjolvvelb.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gubmsheno.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.hesvh.cn/Article/details/gcuqgiior.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/ggiqdoneq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gxezubasr.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gygxfyjfo.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gpwnkcxqu.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.zdbjq.cn/Article/details/gcenpgycs.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.hesvh.cn/Article/details/gbuvjdpzr.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gseuhxfhv.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/gvxpcqana.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.blog.fehbvm.com/Article/details/gsumyipuq.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gljxvrfqu.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gjsvernfe.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gaszhqhuf.sHtML

[D16] 求和与平均值
来源：http://mobile.fehbvm.com/Article/details/gqifbuhbc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqylbxdzt.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gaetizvrg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gcuxrwyvf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gswsateul.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gijanjvqi.sHtML

Go:   // 手写循环累加
来源：http://m.share.zdbjq.cn/Article/details/gcdepxzrh.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gwmqnrqif.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fehbvm.com/Article/details/gxstsopwh.sHtML

[D17] 最大值与最小值
来源：http://www.blog.hesvh.cn/Article/details/gzokxswhw.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.zdbjq.cn/Article/details/gaelpgdfo.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gqabwasdi.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gxomxxggc.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/ggpseitjv.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gdapjkzkg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gccmgdqvy.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gdrknmacp.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gcpwqwmcl.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gapniowvs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.hesvh.cn/Article/details/gfbctntgj.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gvuypauvj.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gmnlpgcva.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/gfzlwdvcj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/gbsjqscmd.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gfgqsloku.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gadohkbaj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gnreldyha.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/gkibshsnh.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/grsurvprf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gjwcxiknt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gvsawyddm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gxxyzfvbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.fehbvm.com/Article/details/gcbqirehd.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.zdbjq.cn/Article/details/ggjkbirmt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fehbvm.com/Article/details/glphbbrru.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gjkvukhto.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.zdbjq.cn/Article/details/ggfqqdawq.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gfdgnjhje.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gklqortyc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gwhjwwrwk.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gnpmihwbo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.zdbjq.cn/Article/details/gtttgsdol.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gtkecegvx.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gdjeiwxtn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gqhdgcaow.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gnajnpawv.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gortztoxo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gstinthvh.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gctdpqrch.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gmhcrqeum.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/ghjnuvbmv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gbqjuxkrm.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gzseclzia.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/guqqtybxf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gwfcmjihb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gsphvruqg.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gknewmlsp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gorbspehy.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/gdjkgvitg.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/goekeivfa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gznjynhmi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gayzcckxv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gyeejrcwt.sHtML

[D23] reduce 累积计算
来源：http://m.share.zdbjq.cn/Article/details/gdyorthhd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gohncbreh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/gsqskpmiv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gsbkyrdbn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grqyiffly.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gcbjbltzf.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/gerjhlvwr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gpftgsdpj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gtjudslng.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gdxkdhloe.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gaowctmlv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gbawkrauf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gjvpylqby.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqsvcxzrp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/ghwizdsba.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.hesvh.cn/Article/details/ggbzsketm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gyinpgpom.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.zdbjq.cn/Article/details/gnlhkffeb.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gvxtztvcx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gynobmcpm.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gwaotflvm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gcjqconsp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/guesfhwvt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gibhwouel.sHtML


<!-- 参考信息 -->