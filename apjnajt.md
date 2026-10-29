代发 wailian999

[C10] 变量作用域
来源：http://mobile.fehbvm.com/Article/details/gpbaqkiha.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.blog.zdbjq.cn/Article/details/glhtvyife.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://blog.hesvh.cn/Article/details/gvyrdfjcc.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.hesvh.cn/Article/details/gsexnpiuc.sHtML

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gidhteouw.sHtML

Java: 方法内为块级作用域
来源：http://m.share.hesvh.cn/Article/details/gkcrrrkgj.sHtML

Go:   花括号块级作用域
来源：http://wap.fehbvm.com/Article/details/gxfgotwfo.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fehbvm.com/Article/details/gdyytwija.sHtML

C#:   块级作用域
来源：http://m.share.hesvh.cn/Article/details/gdeeilnql.sHtML

[C11] 模块导入与导出
来源：http://wap.zdbjq.cn/Article/details/gwbznfwjg.sHtML

Py:   from module import func
来源：http://www.m.share.zdbjq.cn/Article/details/gshlpfjva.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.fehbvm.com/Article/details/gnfhjskip.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.zdbjq.cn/Article/details/gmjildens.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.hesvh.cn/Article/details/gyecdntnd.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gqrpsdzto.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.share.hesvh.cn/Article/details/gttazzhqn.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gfqyhzyot.sHtML

C#:   using System.Text;
来源：http://mobile.fehbvm.com/Article/details/gkscmkrmp.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.m.share.zdbjq.cn/Article/details/gjsbjslot.sHtML

Py:   (lambda: print("run"))()
来源：http://www.blog.hesvh.cn/Article/details/gfzwhqvye.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fehbvm.com/Article/details/glmtgskng.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.zdbjq.cn/Article/details/gyyyaerqm.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.fehbvm.com/Article/details/gjgzdyzyq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://m.share.fehbvm.com/Article/details/gkkkfarnj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://3g.fehbvm.com/Article/details/gyjrtpews.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gjltzpjti.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://read.share.fehbvm.com/Article/details/grfnxkoys.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.fehbvm.com/Article/details/gxbkyzimf.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/gtjnhozkn.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gkfadprep.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gofpjxqib.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gdhtavvbu.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gharfuitk.sHtML

Go:   func add(a, b int) int
来源：http://www.share.fehbvm.com/Article/details/gjjzjtklu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://3g.zdbjq.cn/Article/details/gcavuwkft.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://3g.zdbjq.cn/Article/details/gibbpdcsn.sHtML

[C14] 泛型函数
来源：http://3g.zdbjq.cn/Article/details/gtwiietvt.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://baike.hesvh.cn/Article/details/grdclqdyd.sHtML

PHP:  // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gvcepamdn.sHtML

JS:   // 无泛型
来源：http://3g.zdbjq.cn/Article/details/gyfsnkkcl.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.zdbjq.cn/Article/details/grbnirgcc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gjvwznhhz.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://wap.hesvh.cn/Article/details/gnkggyoqo.sHtML

Ruby: # 无泛型
来源：http://wap.zdbjq.cn/Article/details/gvkfendzy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://wap.fehbvm.com/Article/details/gioscfapy.sHtML

[C15] 解构 / 展开参数
来源：http://read.share.zdbjq.cn/Article/details/gsimjwliw.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.hesvh.cn/Article/details/gddkfiiss.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fehbvm.com/Article/details/gyzojmxcy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.fehbvm.com/Article/details/gvuoefjiz.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/giszjxttj.sHtML

Java: // 无解构
来源：http://m.share.zdbjq.cn/Article/details/gwghvlrpz.sHtML

Go:   // 无解构
来源：http://blog.zdbjq.cn/Article/details/guowrtpvf.sHtML

Ruby: a, b = pair
来源：http://baike.zdbjq.cn/Article/details/gtfmqxyha.sHtML

C#:   var (a, b) = pair;
来源：http://wap.fehbvm.com/Article/details/gibwdcmqv.sHtML

[C16] 函数 / 方法重载
来源：http://wap.hesvh.cn/Article/details/gscjusszy.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/glyjaokfv.sHtML

PHP:  // 无重载
来源：http://www.share.fehbvm.com/Article/details/gwoasgtbi.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.hesvh.cn/Article/details/gxeynbjtp.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.hesvh.cn/Article/details/gjxiiikar.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.share.hesvh.cn/Article/details/gcugsuzdm.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gywhvigle.sHtML

Ruby: # 无重载：靠动态参数
来源：http://read.share.fehbvm.com/Article/details/gcnhdvily.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.zdbjq.cn/Article/details/gltsktcql.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goznqhqsi.sHtML

D. 数组 / 列表 / 集合
来源：http://mobile.zdbjq.cn/Article/details/gwfuyldoh.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guuqdzyfv.sHtML

[D01] 创建数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gngmtlofz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.hesvh.cn/Article/details/gdtynvufs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://3g.hesvh.cn/Article/details/gtvbywqrf.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://m.share.hesvh.cn/Article/details/glqchaheb.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.hesvh.cn/Article/details/gmqyxxiot.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.share.hesvh.cn/Article/details/gzpcatjch.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.share.hesvh.cn/Article/details/gcbqfcnyq.sHtML

Ruby: arr = [1, 2, 3]
来源：http://wap.fehbvm.com/Article/details/gyckfhfnq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.blog.hesvh.cn/Article/details/ghhkzbqyb.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/guhluesyu.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.hesvh.cn/Article/details/gqpwymeks.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.blog.fehbvm.com/Article/details/ggxjrsfbh.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gkgaoljqb.sHtML

TS:   arr.push(4);
来源：http://www.m.share.fehbvm.com/Article/details/gixztrkko.sHtML

Java: list.add(4);
来源：http://3g.fehbvm.com/Article/details/gtpqzfygb.sHtML

Go:   arr = append(arr, 4)
来源：http://www.blog.hesvh.cn/Article/details/gaqobgmxu.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://baike.zdbjq.cn/Article/details/gceohwbnu.sHtML

C#:   list.Add(4);
来源：http://wap.fehbvm.com/Article/details/gvitzdpfw.sHtML

[D03] 在指定位置插入元素
来源：http://read.share.fehbvm.com/Article/details/guotoobbb.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggqlnmbjd.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://baike.fehbvm.com/Article/details/goprvnoeh.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.fehbvm.com/Article/details/gldcqekli.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.hesvh.cn/Article/details/grwfxdzot.sHtML

Java: list.add(0, 0);
来源：http://baike.fehbvm.com/Article/details/gaommjxti.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.zdbjq.cn/Article/details/ghhejjmke.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gshvvvvfk.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gbntvnxgk.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/guewxmxxy.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gnukotjif.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.fehbvm.com/Article/details/grxdnrvkj.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.fehbvm.com/Article/details/gcjbgndig.sHtML

TS:   arr.splice(0, 1);
来源：http://read.share.hesvh.cn/Article/details/gaojbttpp.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.share.fehbvm.com/Article/details/gcmzvblhx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.zdbjq.cn/Article/details/glkwuwecf.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://read.share.fehbvm.com/Article/details/gckcuvxzx.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.blog.zdbjq.cn/Article/details/gexrornir.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gsxkqcomn.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.zdbjq.cn/Article/details/gsabjmmfl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://m.share.zdbjq.cn/Article/details/govmkupuj.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://3g.hesvh.cn/Article/details/gxbeqitpz.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.hesvh.cn/Article/details/gkdnupjct.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.fehbvm.com/Article/details/gnwpqdyyq.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://baike.fehbvm.com/Article/details/gxngrajea.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/grzqugche.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gxqkpfejv.sHtML

[D06] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gsslemgnm.sHtML

Py:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gjtvgenuw.sHtML

PHP:  count($arr);
来源：http://m.share.hesvh.cn/Article/details/gotrxcwcc.sHtML

JS:   arr.length
来源：http://m.share.fehbvm.com/Article/details/glqdumayb.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gfievmffj.sHtML

Java: list.size();
来源：http://baike.zdbjq.cn/Article/details/gajyyegru.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/gpathbrbi.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gfivlocqq.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/gakeqdzws.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gqkgofzfb.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.zdbjq.cn/Article/details/gifmaigaj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.zdbjq.cn/Article/details/gukhtgstr.sHtML

JS:   arr.slice(1, 4);
来源：http://www.m.share.fehbvm.com/Article/details/gjhaxnoxz.sHtML

TS:   arr.slice(1, 4);
来源：http://wap.hesvh.cn/Article/details/gbzljntfj.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gzcunikcd.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gwbnofsfl.sHtML

Ruby: arr[1, 3]
来源：http://www.share.fehbvm.com/Article/details/giinrddri.sHtML

C#:   list.GetRange(1, 3);
来源：http://m.share.hesvh.cn/Article/details/gxezodgik.sHtML

[D08] 合并两个数组
来源：http://www.m.share.fehbvm.com/Article/details/gjabgtarw.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gbhpjhjmh.sHtML

PHP:  array_merge($a, $b);
来源：http://www.share.hesvh.cn/Article/details/guakhagcy.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.hesvh.cn/Article/details/ghlubvkzg.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/gfkiqevzt.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gehsxvhiq.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gmeopuqlv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://read.share.fehbvm.com/Article/details/ghigoogon.sHtML

C#:   a.Concat(b).ToList()
来源：http://m.share.fehbvm.com/Article/details/goylpqbtq.sHtML

[D09] 排序（升序）
来源：http://www.m.share.fehbvm.com/Article/details/glxsufhaw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gvjcoehup.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gkmuavixx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.fehbvm.com/Article/details/gfkatunny.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://read.share.fehbvm.com/Article/details/gjrvpyyen.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gmskhvfij.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gcylbndoe.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gflgekwkg.sHtML

C#:   list.Sort();
来源：http://www.m.share.fehbvm.com/Article/details/gxsfzgasc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gkohupdki.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.zdbjq.cn/Article/details/gpwrucdpv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://baike.fehbvm.com/Article/details/gctdtvhyg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gipyqxslk.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gxcocsxof.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.zdbjq.cn/Article/details/gzwksbnvo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gtewcyxlj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/gdeyxuilc.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://baike.hesvh.cn/Article/details/gotkccvxs.sHtML

[D11] 反转数组
来源：http://3g.zdbjq.cn/Article/details/gdybbpofo.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gxdnumyau.sHtML

PHP:  array_reverse($arr);
来源：http://3g.zdbjq.cn/Article/details/giyltjhfj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/gfmqfguaw.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gmnmhrovf.sHtML

Java: Collections.reverse(list);
来源：http://baike.fehbvm.com/Article/details/gpiwdovkd.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.hesvh.cn/Article/details/gpboappcs.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gzgbqjbig.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gdbahhbqb.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gxrvgcpah.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gazdkmofz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.hesvh.cn/Article/details/gdwsobgsx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gswkqjcuk.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gixrsuyjp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gchevsuxu.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.fehbvm.com/Article/details/giqwqxngi.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/giwrsdnmf.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/glejrfblc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.hesvh.cn/Article/details/gniyhrrqw.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gkdzpzkyz.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.zdbjq.cn/Article/details/gzhdptbdz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gxuvsewcq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.hesvh.cn/Article/details/gszjahntl.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://3g.fehbvm.com/Article/details/grwjdffvb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.fehbvm.com/Article/details/gwmygikhp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gfmardyvl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.fehbvm.com/Article/details/gsjbfwbob.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.hesvh.cn/Article/details/gjiwojfym.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gqvqkanwr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gprbugnkq.sHtML

JS:   arr.map(x => x * 2)
来源：http://m.share.hesvh.cn/Article/details/gayinuerm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfqnfxzsm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gvoyhqyva.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gacphkwem.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/gjvxbzxbi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.zdbjq.cn/Article/details/gqrjhkdlr.sHtML

[D15] 去重
来源：http://mobile.fehbvm.com/Article/details/gkvunrawf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gizxbfcuw.sHtML

PHP:  array_unique($arr);
来源：http://mobile.hesvh.cn/Article/details/gyrnnqobh.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gnpxplauz.sHtML

TS:   [...new Set(arr)]
来源：http://3g.fehbvm.com/Article/details/goskhuzai.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/ghagbcskv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gcdpjgauh.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gdxlvywyr.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gebpktqxm.sHtML

[D16] 求和与平均值
来源：http://baike.zdbjq.cn/Article/details/gynohyxnu.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.zdbjq.cn/Article/details/gntxsriuw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.fehbvm.com/Article/details/ghodntulv.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gbxkkqqjl.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/ggvkkilzp.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gxlfdvooi.sHtML

Go:   // 手写循环累加
来源：http://wap.fehbvm.com/Article/details/gxwbpjvmk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/ggqugknxe.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/godmndxok.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gsrkubfoh.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/geanavvti.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gdzrlgncg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/ghcvpwanv.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gihgkogsh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfmcbyayy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ggdwcohgu.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fehbvm.com/Article/details/gpvnenwmi.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gaztssacp.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/ggbeurfny.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gfdjknfkv.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gnotdqyde.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gwakxwsyp.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/gasuncvkp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/guyznygfe.sHtML

Go:   // 手写双层循环
来源：http://m.share.fehbvm.com/Article/details/gwyunmbue.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gcolotrsf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gtprrogrf.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gaqpoghim.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gyjzhbazf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gkzphggua.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/glwvcaveg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gxfkzkeka.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gfdnkujnv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/glcexxqbg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgawvjmo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/guztmehgq.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gjwkfydbr.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/grmqiegre.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gqyqamitq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fehbvm.com/Article/details/gcuvjthmz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gqdgtwrgg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.zdbjq.cn/Article/details/ghatnrylt.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gojsjsggp.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gljtmrrsq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gjwgzbgqh.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gqdmnjjwr.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gzluutyor.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gntshpflt.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/goewfjlrp.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkczmvblx.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqhsiipov.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gkuachmgv.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gfloypkum.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gwrfawums.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/glcmbpfzm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gxiaiulpj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gpgopixfr.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxffnyxuu.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gouzhwzao.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gfsrdypkf.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gbrfjzisz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/ghxalumwq.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gccqsdtno.sHtML

[D23] reduce 累积计算
来源：http://mobile.hesvh.cn/Article/details/gymvsloam.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gdvmujikc.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gklqbuzrj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gdcedutut.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/gteetkamu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.fehbvm.com/Article/details/gtzetevve.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/ggsynpmtb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gbtwutinx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/grfyryhnc.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gkzkitmov.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gpchpauby.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gsjxeafzt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/gblaxnwxk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gvdnjyjcf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gdvzqgghi.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gxfvlxbyo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/geyaelydk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/grcpblnqs.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gitvgxdna.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/ghqgqxtxv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gjoeencvd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/gkovdfzjg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gjaguyuhq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/gkcmxvlvy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gkrdefhjt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/gpzbzcjpa.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/gyqjjtfvl.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/grmirajbm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/guhfbptwf.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gnpazqbgo.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gcyxqgthc.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gcppqrckj.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gefljrwaj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gjjahamvb.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gjjautljy.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gsgkvqvah.sHtML


<!-- 参考信息 -->