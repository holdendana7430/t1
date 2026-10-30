代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://3g.zdbjq.cn/Article/details/gwaoyllsy.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://read.share.fehbvm.com/Article/details/gklzmbkvi.sHtML

[C08] 闭包
来源：http://baike.hesvh.cn/Article/details/gyfgdheog.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://m.share.zdbjq.cn/Article/details/gkuovpojx.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/ghyplzqen.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.blog.hesvh.cn/Article/details/grezpagui.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://3g.fehbvm.com/Article/details/gfmoqkfzf.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://wap.zdbjq.cn/Article/details/gdxlprvhz.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://baike.zdbjq.cn/Article/details/gxagqirzl.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://mobile.zdbjq.cn/Article/details/gyacpfetv.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gfisrjjvs.sHtML

[C09] 递归
来源：http://blog.fehbvm.com/Article/details/gciuymsbl.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.blog.hesvh.cn/Article/details/guvzyhesh.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.fehbvm.com/Article/details/gzfqylxou.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://blog.hesvh.cn/Article/details/gjjpnejln.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://wap.hesvh.cn/Article/details/gvuhcschh.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://read.share.hesvh.cn/Article/details/gcvcygjfw.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://blog.fehbvm.com/Article/details/gntusmiqr.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://read.share.hesvh.cn/Article/details/gijytjydg.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.m.share.fehbvm.com/Article/details/glarufzkf.sHtML

[C10] 变量作用域
来源：http://3g.hesvh.cn/Article/details/gckiegrml.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://mobile.zdbjq.cn/Article/details/gufyttjas.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.blog.zdbjq.cn/Article/details/gexwolfrp.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.blog.zdbjq.cn/Article/details/gcloagjae.sHtML

TS:   同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gblbepmoz.sHtML

Java: 方法内为块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gwsjepgbp.sHtML

Go:   花括号块级作用域
来源：http://read.share.fehbvm.com/Article/details/gbmahmtbp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://mobile.hesvh.cn/Article/details/gbutawyhn.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/ghbbmkuam.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/ghzewbtqe.sHtML

Py:   from module import func
来源：http://blog.zdbjq.cn/Article/details/gbaonfefp.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://mobile.zdbjq.cn/Article/details/giokfdkxb.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://blog.hesvh.cn/Article/details/glgdrtscb.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.fehbvm.com/Article/details/gdexlwnnd.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/gakxjxhco.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.hesvh.cn/Article/details/gafpwwgna.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gfbdihbgz.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gwxapplte.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fehbvm.com/Article/details/gttymitkn.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gktkmoqzh.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.fehbvm.com/Article/details/ggxfbeyci.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.zdbjq.cn/Article/details/ghudbmdom.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gujwwosea.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.hesvh.cn/Article/details/gzkwlfrgp.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gyjmqqswu.sHtML

Ruby: -> { puts "run" }.call
来源：http://m.share.zdbjq.cn/Article/details/ggiubfluq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://m.share.fehbvm.com/Article/details/gmymuyhnn.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.fehbvm.com/Article/details/gikangbnq.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.share.zdbjq.cn/Article/details/gqjbfavxy.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gtvjhtyem.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gkgkncjcf.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gvxkqwhzm.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gmhbkeakl.sHtML

Go:   func add(a, b int) int
来源：http://m.share.zdbjq.cn/Article/details/gmsagvxrx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://read.share.fehbvm.com/Article/details/gphdtfilm.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://baike.fehbvm.com/Article/details/guqigavlk.sHtML

[C14] 泛型函数
来源：http://www.blog.hesvh.cn/Article/details/gszhfqlnr.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gjvidllmk.sHtML

PHP:  // 无泛型
来源：http://blog.hesvh.cn/Article/details/gzkcifade.sHtML

JS:   // 无泛型
来源：http://3g.fehbvm.com/Article/details/gmyxulrfx.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.blog.zdbjq.cn/Article/details/gldcjvqmb.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gksknrzsw.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.hesvh.cn/Article/details/gkerniquc.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/grvfblykd.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.fehbvm.com/Article/details/gcszicint.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.hesvh.cn/Article/details/gmkpculoz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.fehbvm.com/Article/details/gcrmszbfx.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.hesvh.cn/Article/details/gyownbgze.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://m.share.zdbjq.cn/Article/details/gquzoyapa.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.fehbvm.com/Article/details/gedkecgmi.sHtML

Java: // 无解构
来源：http://mobile.zdbjq.cn/Article/details/gacsenxpa.sHtML

Go:   // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gcewspcff.sHtML

Ruby: a, b = pair
来源：http://3g.hesvh.cn/Article/details/gqxbnlzkh.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gfkrzgdho.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.zdbjq.cn/Article/details/guroljcsh.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.zdbjq.cn/Article/details/gxlvxgizo.sHtML

PHP:  // 无重载
来源：http://read.share.zdbjq.cn/Article/details/gmwxyyctb.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gsjogfegl.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.blog.zdbjq.cn/Article/details/ggzpkcede.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gbkbqxxti.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.zdbjq.cn/Article/details/gxenthixj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gowxkozgu.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fehbvm.com/Article/details/gvtfkuqhp.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmwnfbirx.sHtML

D. 数组 / 列表 / 集合
来源：http://www.blog.zdbjq.cn/Article/details/glmvblbjk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkpmqgxfu.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/ghxomaexb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.zdbjq.cn/Article/details/gmtnemfeh.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.zdbjq.cn/Article/details/glyvnieuj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gzxcwcrdm.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/gfdkrbbvd.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.zdbjq.cn/Article/details/guccetxrq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.blog.zdbjq.cn/Article/details/gymklpayy.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.hesvh.cn/Article/details/gqrqbyarj.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gekdgardg.sHtML

[D02] 追加元素到末尾
来源：http://www.share.fehbvm.com/Article/details/goyjfsipl.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.share.zdbjq.cn/Article/details/gaxobdcxf.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fehbvm.com/Article/details/galpyjlgg.sHtML

JS:   arr.push(4);
来源：http://baike.hesvh.cn/Article/details/gpngamsom.sHtML

TS:   arr.push(4);
来源：http://mobile.zdbjq.cn/Article/details/gmujmvxks.sHtML

Java: list.add(4);
来源：http://mobile.hesvh.cn/Article/details/gblgtpyxk.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.hesvh.cn/Article/details/gyxnchcgp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gxdmuogrm.sHtML

C#:   list.Add(4);
来源：http://www.blog.fehbvm.com/Article/details/geakesbfy.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/gutwohkco.sHtML

Py:   arr.insert(0, 0)
来源：http://blog.hesvh.cn/Article/details/gssbkepnw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjkrrpdyd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gsmnxzacx.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gagvwswfc.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gzsrdskyx.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.fehbvm.com/Article/details/gouwxwbwi.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gnasieuxa.sHtML

C#:   list.Insert(0, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gfelijpui.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gonxrjtma.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.share.fehbvm.com/Article/details/gtspnjbry.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.zdbjq.cn/Article/details/ggtqxvifr.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wap.fehbvm.com/Article/details/gblhmwjbk.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.fehbvm.com/Article/details/glqyhrone.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.zdbjq.cn/Article/details/gnzdyvtfk.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.fehbvm.com/Article/details/gzttgduyc.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://3g.fehbvm.com/Article/details/gtzbwqxxd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gfpwvhnfe.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/grhehqjhi.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gxumdytmy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/ggznohzkp.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.hesvh.cn/Article/details/gihzknimi.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.zdbjq.cn/Article/details/gmotgkzag.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://read.share.hesvh.cn/Article/details/gtlfbkznn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gqzrretso.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.hesvh.cn/Article/details/gykyegmuo.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.hesvh.cn/Article/details/gebbfzovp.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/gafqgmmzz.sHtML

Py:   len(arr)
来源：http://mobile.hesvh.cn/Article/details/ggqxjqlwt.sHtML

PHP:  count($arr);
来源：http://wap.fehbvm.com/Article/details/gmjvipuzy.sHtML

JS:   arr.length
来源：http://wap.zdbjq.cn/Article/details/gcrmpslvv.sHtML

TS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gvrilziln.sHtML

Java: list.size();
来源：http://blog.fehbvm.com/Article/details/gyipuhslm.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gukezhyir.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gxnveloje.sHtML

C#:   list.Count;
来源：http://wap.zdbjq.cn/Article/details/gbuyemrfq.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gkoivcfpx.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fehbvm.com/Article/details/govgfkvge.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.fehbvm.com/Article/details/gssecmftg.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.fehbvm.com/Article/details/gvboddeja.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gjlfivjdo.sHtML

Java: list.subList(1, 4);
来源：http://m.share.fehbvm.com/Article/details/gtwxynxao.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gykicxtxf.sHtML

Ruby: arr[1, 3]
来源：http://read.share.zdbjq.cn/Article/details/ghbqepjnu.sHtML

C#:   list.GetRange(1, 3);
来源：http://3g.zdbjq.cn/Article/details/ghstjiubh.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/glncqxith.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.hesvh.cn/Article/details/ggtlplmty.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.zdbjq.cn/Article/details/gnjrnaffj.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.zdbjq.cn/Article/details/gdrhhsqal.sHtML

TS:   [...a, ...b];
来源：http://wap.fehbvm.com/Article/details/gldxtxfzg.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.blog.fehbvm.com/Article/details/gdczhkkfp.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/gaellejaj.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gblhhwafg.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gdqhxzivh.sHtML

[D09] 排序（升序）
来源：http://blog.zdbjq.cn/Article/details/ghixbqtga.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gvzifligi.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/ggsznuqtz.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.zdbjq.cn/Article/details/gtkbmrsas.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gbuzwjron.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.share.hesvh.cn/Article/details/gpyxmdlwl.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gyekkummj.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gpggduawr.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/gjkasuiaf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gxjbnwlql.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/gauviycyb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gvmombsyv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/gqbxcceju.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fehbvm.com/Article/details/gvhopaxwa.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.zdbjq.cn/Article/details/gmwsdabzk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.zdbjq.cn/Article/details/ggbdasrhd.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.zdbjq.cn/Article/details/gbjfvhjhp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.zdbjq.cn/Article/details/ggtwzvuoe.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gbifbbjbk.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.hesvh.cn/Article/details/gvjwkhgys.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fehbvm.com/Article/details/gibdgdgex.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gyxqsrtmk.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gxfoqfdjd.sHtML

Java: Collections.reverse(list);
来源：http://m.share.fehbvm.com/Article/details/gxmzmfvga.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.zdbjq.cn/Article/details/grgtwzqzm.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gagqoyysz.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gsrxrufyc.sHtML

[D12] 查找元素下标
来源：http://blog.fehbvm.com/Article/details/gweyujbqj.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fehbvm.com/Article/details/gxhkylucw.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gkwvjjkdc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gdnyktmgc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/ghumurdsr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.zdbjq.cn/Article/details/gsteklnyw.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gvaginmix.sHtML

Ruby: arr.index(x)
来源：http://m.share.fehbvm.com/Article/details/gelvqzyld.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/ggawrtkmj.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gquomxdfa.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fehbvm.com/Article/details/gdrowpqej.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/goantishn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkyjdjgoy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gjhyjjjaf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gfaqvjreu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gudcfrmnw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/gwwxginfv.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkuctweej.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/ghcdkxapq.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.hesvh.cn/Article/details/gqbqlzevx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.hesvh.cn/Article/details/gkusdaozn.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.zdbjq.cn/Article/details/gcvbpprzn.sHtML

TS:   arr.map(x => x * 2)
来源：http://baike.hesvh.cn/Article/details/grsvaklqq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gsbnrbfaf.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gholwbkxw.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fehbvm.com/Article/details/guyfbsbun.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.zdbjq.cn/Article/details/ggwckawoi.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gqbbtanbt.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gpdvtcocu.sHtML

PHP:  array_unique($arr);
来源：http://m.share.fehbvm.com/Article/details/gqjfhthha.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/guzfpjbeu.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/ghwgrcipp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.hesvh.cn/Article/details/gopftpowk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.zdbjq.cn/Article/details/gjtogtnpj.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/getccccvr.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gqucdvgwz.sHtML

[D16] 求和与平均值
来源：http://blog.zdbjq.cn/Article/details/grzsopwmj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.hesvh.cn/Article/details/gjqcujlak.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gskgngdft.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/ggjfgiolo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gndbcxllj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.fehbvm.com/Article/details/gvqjeaxyh.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gqpqmljch.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/githilyzx.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/glswggbjk.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gphdvzncp.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.hesvh.cn/Article/details/gogsweruz.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gwskjrymx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/gnjlowsuo.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gvmlunvmy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gpzdsedug.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gdaijpwqt.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/gjgnstsdr.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gridgnpxf.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/gpzdvllry.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gxdpevtzl.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gceaymsej.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/ggjgtcvkb.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/griczbbxq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gwymllisn.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gkenfdqol.sHtML

Ruby: nested.flatten
来源：http://baike.zdbjq.cn/Article/details/gvsziqyws.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gdgzsgbhk.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/ghbbgenrm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gxfunwcpp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gmzhttcoo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/grdclngxl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.zdbjq.cn/Article/details/ghpzsyckb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/greztxkii.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/glwpxukue.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gccvozvmr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.zdbjq.cn/Article/details/gimlmkyyr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gvfpbftex.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gzjfkxyfg.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/grwjdvyjw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/grdtkvayo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gtdabbchd.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gwbxgppmy.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gypxrkdej.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gxakhhfbz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.fehbvm.com/Article/details/gwouncpvh.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.hesvh.cn/Article/details/gdtggbini.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gopjsnmpc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/ggfdziiim.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/guhactcem.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gpmqcndwh.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdeobhtuf.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gzxgjialj.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/ggggiarjc.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gobxqlwiw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gpmftexpx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.fehbvm.com/Article/details/gttjbweix.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gboauzqht.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.zdbjq.cn/Article/details/grbslxhth.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gtergeftl.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/giyajcctf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gnjamixyj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gfmvzyqbv.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/grhiemlzg.sHtML

[D23] reduce 累积计算
来源：http://mobile.fehbvm.com/Article/details/gtkncoudc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gdxewpoas.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/grdaobeqi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gmudtbadm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gmrbclcuq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gtbufkjsv.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gdlvvumil.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.hesvh.cn/Article/details/gydzqtlle.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gdqatujof.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/gtsxsqajl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/gjdllhasd.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gnoazbalu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.fehbvm.com/Article/details/gdrpkzhre.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/givsmzvij.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/glxstnwtw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/goxpawhdl.sHtML


<!-- 参考信息 -->