代发 wailian999

TS:   同 JS
来源：http://www.blog.fehbvm.com/Article/details/gfrsjzkru.sHtML

Java: 方法内为块级作用域
来源：http://3g.zdbjq.cn/Article/details/gdzmzcihd.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gwqbydhur.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/ghxbqzdxi.sHtML

C#:   块级作用域
来源：http://m.share.zdbjq.cn/Article/details/gdsmdbrof.sHtML

[C11] 模块导入与导出
来源：http://m.share.fehbvm.com/Article/details/givoafmsr.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gxzmxdvpi.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.m.share.hesvh.cn/Article/details/gdhgswbaj.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.fehbvm.com/Article/details/gpwxueltd.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.fehbvm.com/Article/details/gljjcebep.sHtML

Java: import java.util.List;
来源：http://baike.fehbvm.com/Article/details/gxyfqrxzp.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gcsxbfkob.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.zdbjq.cn/Article/details/guticjpjt.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gevxhvvyk.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.hesvh.cn/Article/details/ghtkywjbw.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.zdbjq.cn/Article/details/gekeeajbm.sHtML

PHP:  (function () { echo "run"; })();
来源：http://3g.hesvh.cn/Article/details/gulczdjgs.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.hesvh.cn/Article/details/gsxjkioxx.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.fehbvm.com/Article/details/gecfetxxk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://blog.zdbjq.cn/Article/details/gaprrrutq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.zdbjq.cn/Article/details/gcxkwpzgh.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/gtehbyrkh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gpubcufjx.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.hesvh.cn/Article/details/ghcnmoian.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.zdbjq.cn/Article/details/gdamadfke.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/gzbwznyej.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.m.share.hesvh.cn/Article/details/ghnjkcyvi.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gbbbumotx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gpkjwdubk.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gzzbmnisg.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gvedmefkw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fehbvm.com/Article/details/gamykyaqu.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gwyguthon.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.blog.zdbjq.cn/Article/details/gxffxpjkx.sHtML

PHP:  // 无泛型
来源：http://3g.fehbvm.com/Article/details/gwwgammfd.sHtML

JS:   // 无泛型
来源：http://blog.zdbjq.cn/Article/details/geynzikpi.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fehbvm.com/Article/details/geoksyory.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://mobile.fehbvm.com/Article/details/gtibojfgh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.hesvh.cn/Article/details/gcokehdbl.sHtML

Ruby: # 无泛型
来源：http://m.share.hesvh.cn/Article/details/gqchymrqh.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.fehbvm.com/Article/details/gmtwwbgnu.sHtML

[C15] 解构 / 展开参数
来源：http://blog.zdbjq.cn/Article/details/gsmwvgpgs.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gxnkvncxn.sHtML

PHP:  [$a, $b] = $pair;
来源：http://baike.fehbvm.com/Article/details/gxmukhlbq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gwrjblohh.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.hesvh.cn/Article/details/gfgnqeppm.sHtML

Java: // 无解构
来源：http://mobile.hesvh.cn/Article/details/gzrkpthjy.sHtML

Go:   // 无解构
来源：http://wap.fehbvm.com/Article/details/geprdymdb.sHtML

Ruby: a, b = pair
来源：http://www.m.share.zdbjq.cn/Article/details/gogfvyupq.sHtML

C#:   var (a, b) = pair;
来源：http://blog.zdbjq.cn/Article/details/guejobxck.sHtML

[C16] 函数 / 方法重载
来源：http://www.m.share.fehbvm.com/Article/details/guvxlhcwe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/gdmldbsjd.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/grsdxtnfj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.zdbjq.cn/Article/details/gxggvenrx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://m.share.fehbvm.com/Article/details/gyufijyyv.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.hesvh.cn/Article/details/gsdqciqlt.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.share.zdbjq.cn/Article/details/gqxvdbaod.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.share.zdbjq.cn/Article/details/gxdenkbxi.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fehbvm.com/Article/details/gjxpuhuao.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggmyjjgsb.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.hesvh.cn/Article/details/gbnxawtuv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggakoxqoa.sHtML

[D01] 创建数组 / 列表
来源：http://baike.fehbvm.com/Article/details/grqaporiv.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fehbvm.com/Article/details/glbrrqaxm.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/ggayostgv.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://wap.fehbvm.com/Article/details/gppnyefsw.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.fehbvm.com/Article/details/gcfzahrjj.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://m.share.fehbvm.com/Article/details/gtwlskdfs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gecqudxak.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/gcsgmsikf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.m.share.zdbjq.cn/Article/details/gaycbiloe.sHtML

[D02] 追加元素到末尾
来源：http://baike.fehbvm.com/Article/details/gbeuqhfim.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://3g.fehbvm.com/Article/details/gooyjegci.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.fehbvm.com/Article/details/gnlqxkceo.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/grcocdbdl.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gxypfvlkn.sHtML

Java: list.add(4);
来源：http://m.share.hesvh.cn/Article/details/gkuhbkeyq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gteaspwfr.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.zdbjq.cn/Article/details/gfrhnoimn.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/ggdzlgcqi.sHtML

[D03] 在指定位置插入元素
来源：http://wap.zdbjq.cn/Article/details/girrxnjvz.sHtML

Py:   arr.insert(0, 0)
来源：http://wap.zdbjq.cn/Article/details/gdswtyzpw.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.hesvh.cn/Article/details/gmdqygomo.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://baike.fehbvm.com/Article/details/gzniohwng.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/giutvfxhz.sHtML

Java: list.add(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gehdsdvyu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gixxgrclt.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.hesvh.cn/Article/details/ghjetifts.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gvqzbwrkj.sHtML

[D04] 删除元素
来源：http://m.share.fehbvm.com/Article/details/gavwljlco.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.blog.hesvh.cn/Article/details/gmsrwpxxr.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://mobile.fehbvm.com/Article/details/gozraufkl.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.hesvh.cn/Article/details/gqvrfqcqv.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.hesvh.cn/Article/details/geatcuyoe.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.m.share.hesvh.cn/Article/details/gztvcqipy.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.hesvh.cn/Article/details/gnwffntfk.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.share.hesvh.cn/Article/details/goipukdpg.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://3g.hesvh.cn/Article/details/gzchxdtys.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/guibwgjqp.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gyjdluesc.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.fehbvm.com/Article/details/gaxbexmna.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fehbvm.com/Article/details/gwvlvekwc.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.hesvh.cn/Article/details/gvavbmueb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/geodtreou.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gxflwyrib.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gfmnypkzm.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.hesvh.cn/Article/details/gpxkutzyy.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gajccyiku.sHtML

Py:   len(arr)
来源：http://3g.fehbvm.com/Article/details/gknlzbnwf.sHtML

PHP:  count($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvlwsyywa.sHtML

JS:   arr.length
来源：http://m.share.zdbjq.cn/Article/details/gcnodpvyt.sHtML

TS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gryrxyggp.sHtML

Java: list.size();
来源：http://mobile.zdbjq.cn/Article/details/glsgukdah.sHtML

Go:   len(arr)
来源：http://wap.fehbvm.com/Article/details/gcfrhhcuz.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.hesvh.cn/Article/details/glkywufcv.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gaawraoxc.sHtML

[D07] 切片 / 取子数组
来源：http://baike.fehbvm.com/Article/details/gzgfnxavo.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.hesvh.cn/Article/details/gfjqgldlh.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gqlhayxuh.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.hesvh.cn/Article/details/gsnoxfqhr.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gybxwbghf.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gporiindp.sHtML

Go:   arr[1:4]
来源：http://www.m.share.hesvh.cn/Article/details/gwwamnrfb.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gapllrdqn.sHtML

C#:   list.GetRange(1, 3);
来源：http://wap.zdbjq.cn/Article/details/gqrzivtav.sHtML

[D08] 合并两个数组
来源：http://wap.fehbvm.com/Article/details/gqxdnrupe.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/guisduvmz.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.fehbvm.com/Article/details/gfeixsjdl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://m.share.hesvh.cn/Article/details/gglcdsmrh.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/gtlyifzxy.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gvuxsnonc.sHtML

Go:   append(a, b...)
来源：http://mobile.fehbvm.com/Article/details/gdwsqqgcu.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gsyqvemxj.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.hesvh.cn/Article/details/gggbwssep.sHtML

[D09] 排序（升序）
来源：http://www.m.share.zdbjq.cn/Article/details/ggfshoaar.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/ggljjqbsg.sHtML

PHP:  sort($arr);
来源：http://wap.fehbvm.com/Article/details/gljjyvfbc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://read.share.fehbvm.com/Article/details/gtlqgmmsf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gxdasuicx.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gcjniofqo.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gzhtsxpce.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/geqqzwixt.sHtML

C#:   list.Sort();
来源：http://blog.fehbvm.com/Article/details/gmphxhjnv.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gdzvnmvqb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gmglpivvx.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/girzyhexu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/goxflmqdv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gammfbrhz.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gfojyrenr.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gsjloqehf.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/ghpxcixbb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.fehbvm.com/Article/details/gvwgtxpyd.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gkozyukqq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gsfcimvzh.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.hesvh.cn/Article/details/gdoniepyz.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/grvdvkkye.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gugqagjqw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gdaurhyaw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/ganeecqqx.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gbgaarwpy.sHtML

C#:   list.Reverse();
来源：http://3g.fehbvm.com/Article/details/gyeadwlmn.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gzitkunbx.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gqtiwmnof.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.hesvh.cn/Article/details/gctwhwpjl.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.hesvh.cn/Article/details/gddndrnqm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gniwjrbzt.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.zdbjq.cn/Article/details/gzxvydzqu.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.hesvh.cn/Article/details/govvqswjq.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkovqzyvn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gkzzswuhx.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/gflfvkvid.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.hesvh.cn/Article/details/gfmsuwkqr.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.zdbjq.cn/Article/details/gellrumix.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gnfuhftxf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gbndwaurd.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/gzdtcqsdu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/grehcqdfz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gqwyzvfxs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/glmldmdzh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.fehbvm.com/Article/details/gzacoeqpr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/ghgdpqkyg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gvmbfqyry.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.hesvh.cn/Article/details/grivsyopa.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gegmqbfev.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gqutwdgcs.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gjodovvnj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gwptgggyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gwlvfztsh.sHtML

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gvfgztnyn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/giyjlzjqt.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/gzbttlktg.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/ggezjqmwz.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ghkasybjk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gdyiyxnxl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gjnlgpavb.sHtML

Ruby: arr.uniq
来源：http://blog.hesvh.cn/Article/details/gkbhclgdk.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/gyqmqhagf.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/ggghqcjro.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcuntopfq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gtiwfxfca.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gyhmzypvg.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.zdbjq.cn/Article/details/gjvddhzlv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/ghxrtdvcp.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gizbaxtsj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gpnhsgmzc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gswbqakql.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gqmvwdmyw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/guxewitrh.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gnyxgdpin.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gqfavdpai.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gfqbtpost.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/gkhkkgrzx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gyvfxbikb.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gkznpbpqd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gnxjhhlbx.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gunlvjkui.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gjcoguqcv.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gsyduvpsc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gudcunbus.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gtrewercu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gtfsccmfe.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gsvgqvlvf.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gipnqkawl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.zdbjq.cn/Article/details/gvqvhyufo.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/glcaqvfhz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.zdbjq.cn/Article/details/gozetlpnw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gfdcomogz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/geyxawjrf.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/gvahmlruq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fehbvm.com/Article/details/gcokwbhwm.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gnfasgbhq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gupmvdqtk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gtxavxznf.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.hesvh.cn/Article/details/glxanawwn.sHtML

Py:   Counter(arr)
来源：http://read.share.hesvh.cn/Article/details/guyjpiavx.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/glaxonitj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzajjlqby.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gszgbfwvx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gcysklxkb.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gxykkfdhy.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gsieeavfm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gpeonupou.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/gfhtowgdn.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gdluunzoe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.hesvh.cn/Article/details/gjwsubvhr.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gywekozxu.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/glmjpmruk.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/gnejzlsfp.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gxktxajcz.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.hesvh.cn/Article/details/gksxhxgtx.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/gfitbrzlu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gvcmcyvuu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gcxungyfq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gqvvbdztc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.zdbjq.cn/Article/details/gxgdvrogb.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gbyucwmjn.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gyhruheum.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/goocumesg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/ghskwxjun.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gjdwdcqtt.sHtML

[D23] reduce 累积计算
来源：http://3g.hesvh.cn/Article/details/gaptfbfvy.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/gnlipocth.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/guajveczh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gssjnqfad.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gdveiqmvv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gigawfuwv.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gwhfameds.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gnpwyfbnl.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gkdwfqzze.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gisyjhfcs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/giefpycnh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/giyqztich.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gkuyikgcy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gnqrjfedv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.hesvh.cn/Article/details/gruatkmgy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gkgimnuhf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/girftrlcn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/ghzppggiv.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gqrbvguvu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gvkvywsdi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gotghyyrc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gjjvpcfwr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/gxwyltsne.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/gcdbclwwy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/geuvudmff.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/goelhgkdo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gmlgbzrxn.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/guvhvitre.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.fehbvm.com/Article/details/gjsvfcrxp.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gizxxiwep.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gfrukmplq.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gvtzkamjn.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gvilbegis.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gooldkzcp.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gmrthvwdf.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gjclozkbu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gavtvgifn.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gczgucnzw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxezkqfyx.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gwfdtrezk.sHtML


<!-- 参考信息 -->