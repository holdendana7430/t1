代发 wailian999

TS:   同 JS
来源：http://mobile.fehbvm.com/Article/details/gqnebpibv.sHtML

Java: 方法内为块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/ghkfnvjmr.sHtML

Go:   花括号块级作用域
来源：http://baike.fehbvm.com/Article/details/glaakvcyi.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://baike.zdbjq.cn/Article/details/ghdcbjcxm.sHtML

C#:   块级作用域
来源：http://mobile.zdbjq.cn/Article/details/gsvsbhebu.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gquxlgpum.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/gfresgicj.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://m.share.hesvh.cn/Article/details/gkufncmyc.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fehbvm.com/Article/details/gqcdwqwgs.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gacvywhpg.sHtML

Java: import java.util.List;
来源：http://www.share.hesvh.cn/Article/details/ggiquuhac.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fehbvm.com/Article/details/gdtnmujgr.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://m.share.zdbjq.cn/Article/details/gxwgorkro.sHtML

C#:   using System.Text;
来源：http://baike.zdbjq.cn/Article/details/gaczsobjn.sHtML

[C12] 立即执行函数 IIFE
来源：http://www.share.zdbjq.cn/Article/details/gzycaibdr.sHtML

Py:   (lambda: print("run"))()
来源：http://read.share.fehbvm.com/Article/details/gbuvsgevk.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/grzqywktj.sHtML

JS:   (() => { console.log("run"); })();
来源：http://blog.hesvh.cn/Article/details/grjrxkrpo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.hesvh.cn/Article/details/gimidevrq.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/grdqkmzgm.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://wap.zdbjq.cn/Article/details/gwalxvkhg.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.zdbjq.cn/Article/details/gmankjppb.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fehbvm.com/Article/details/ghjrffhzw.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gxydiqrht.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://blog.hesvh.cn/Article/details/gopoaiemf.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://m.share.zdbjq.cn/Article/details/gwjudjymp.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.blog.fehbvm.com/Article/details/gxhfwkqbu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gusriignw.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ghffulleu.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gbumtpcfv.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fehbvm.com/Article/details/gdgnzymam.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.hesvh.cn/Article/details/gtevtanrs.sHtML

[C14] 泛型函数
来源：http://blog.fehbvm.com/Article/details/gfwgnlxmo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.fehbvm.com/Article/details/gejvxbtnh.sHtML

PHP:  // 无泛型
来源：http://wap.hesvh.cn/Article/details/gzmfwjuxx.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gjuhonifk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.zdbjq.cn/Article/details/gaazehtje.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://wap.hesvh.cn/Article/details/gwnemmvbh.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://mobile.fehbvm.com/Article/details/gdflxyyrm.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gtfgmbtfg.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/giqvifnqz.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gszvcljdz.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://3g.fehbvm.com/Article/details/gfhudfydf.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.fehbvm.com/Article/details/gcaxdskzj.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/gjgflzlql.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gzygmepky.sHtML

Java: // 无解构
来源：http://www.m.share.zdbjq.cn/Article/details/gzdfkgjew.sHtML

Go:   // 无解构
来源：http://blog.hesvh.cn/Article/details/gyzmbwlma.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gnlurjqyt.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.hesvh.cn/Article/details/gzcvxuxrz.sHtML

[C16] 函数 / 方法重载
来源：http://baike.fehbvm.com/Article/details/gzgmdspyv.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gzlkbtgcg.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gvmrbfdhn.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.hesvh.cn/Article/details/gwuterwrx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://wap.hesvh.cn/Article/details/gozwkzptz.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.hesvh.cn/Article/details/galtqydqy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.m.share.zdbjq.cn/Article/details/gkryegwzf.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.m.share.hesvh.cn/Article/details/gjpzfovff.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggaxlxhvw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfeaazpsu.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.fehbvm.com/Article/details/gqzsftlff.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gngfhydwe.sHtML

[D01] 创建数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gyclvacyb.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.zdbjq.cn/Article/details/gekbfiwxa.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://read.share.zdbjq.cn/Article/details/gqwlxvbej.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fehbvm.com/Article/details/gurljwvnc.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://mobile.fehbvm.com/Article/details/gugugkfdq.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.zdbjq.cn/Article/details/guesnmihb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.zdbjq.cn/Article/details/gfyiuevdo.sHtML

Ruby: arr = [1, 2, 3]
来源：http://blog.zdbjq.cn/Article/details/gmtzwkcxc.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.share.fehbvm.com/Article/details/ggdddyqoa.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.hesvh.cn/Article/details/gbreqmhxe.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.hesvh.cn/Article/details/gfutxnlxv.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://mobile.hesvh.cn/Article/details/gmfbrkuwv.sHtML

JS:   arr.push(4);
来源：http://blog.fehbvm.com/Article/details/gvtvljufc.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gkglnfrxn.sHtML

Java: list.add(4);
来源：http://3g.hesvh.cn/Article/details/gktjqbqnt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gdnbasijx.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.hesvh.cn/Article/details/gkxinxtca.sHtML

C#:   list.Add(4);
来源：http://baike.hesvh.cn/Article/details/gxzsztjmp.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fehbvm.com/Article/details/gmoajjxzh.sHtML

Py:   arr.insert(0, 0)
来源：http://www.share.fehbvm.com/Article/details/gpndotvxk.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.share.zdbjq.cn/Article/details/gsrbyjqrv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.zdbjq.cn/Article/details/gbyacwrba.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/grymgdgys.sHtML

Java: list.add(0, 0);
来源：http://read.share.zdbjq.cn/Article/details/gryrqhkpk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gbhocnejr.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfcgbea.sHtML

C#:   list.Insert(0, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzqgzhqbx.sHtML

[D04] 删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gglyrjibr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://3g.zdbjq.cn/Article/details/guxoymrfe.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gpqbatvzw.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gcqnptjzp.sHtML

TS:   arr.splice(0, 1);
来源：http://www.blog.zdbjq.cn/Article/details/ggotgxfiv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gjlqjzzyl.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.m.share.hesvh.cn/Article/details/gkbtkmufx.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.zdbjq.cn/Article/details/gojgcbwuj.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.zdbjq.cn/Article/details/gxqcqxeig.sHtML

[D05] 访问与修改元素
来源：http://blog.zdbjq.cn/Article/details/gmtyujcdz.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.zdbjq.cn/Article/details/grggkywhf.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fehbvm.com/Article/details/gxbradckn.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/glevyytzm.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gwjgsxhoz.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://mobile.fehbvm.com/Article/details/gzxvfbtdo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gxyvruirm.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gwlzlxkpy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.zdbjq.cn/Article/details/gjiqbfqke.sHtML

[D06] 数组长度
来源：http://wap.fehbvm.com/Article/details/grrwxhcyh.sHtML

Py:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gjkyyufyy.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gvbtraqra.sHtML

JS:   arr.length
来源：http://3g.zdbjq.cn/Article/details/guictycfo.sHtML

TS:   arr.length
来源：http://wap.fehbvm.com/Article/details/gxnudeiqv.sHtML

Java: list.size();
来源：http://blog.hesvh.cn/Article/details/gnmpahwzq.sHtML

Go:   len(arr)
来源：http://baike.hesvh.cn/Article/details/gmfejrrqi.sHtML

Ruby: arr.length; arr.size
来源：http://mobile.hesvh.cn/Article/details/gecrgdtqn.sHtML

C#:   list.Count;
来源：http://3g.fehbvm.com/Article/details/gmawyhjry.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.hesvh.cn/Article/details/gzvsurmmj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://read.share.hesvh.cn/Article/details/gdzsvlpxp.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://m.share.fehbvm.com/Article/details/gxprbugzv.sHtML

JS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gceoobgvg.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gilrnlrvc.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gmzhikoxu.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fehbvm.com/Article/details/gvtibzwgo.sHtML

Ruby: arr[1, 3]
来源：http://3g.hesvh.cn/Article/details/gzqidvktx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gakjtjwns.sHtML

[D08] 合并两个数组
来源：http://www.share.fehbvm.com/Article/details/gifwwtuhm.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gevjtdonb.sHtML

PHP:  array_merge($a, $b);
来源：http://baike.fehbvm.com/Article/details/glxfblyhi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gvxuknofe.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/gaaifwtyl.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.zdbjq.cn/Article/details/gugouekdk.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gfhyzmsiq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fehbvm.com/Article/details/gsgdhtejy.sHtML

C#:   a.Concat(b).ToList()
来源：http://mobile.fehbvm.com/Article/details/gzvrcjhcn.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gqlszbiei.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gbxwlzonf.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gnzzltgdx.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gpckrqdhj.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://baike.fehbvm.com/Article/details/gyuuaprmw.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gjnxomqdb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gilndyxgi.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gxlxeoydi.sHtML

C#:   list.Sort();
来源：http://read.share.hesvh.cn/Article/details/gudtxkbyf.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gpvywgsqn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.zdbjq.cn/Article/details/gtiihbrwd.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmtgejzf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.zdbjq.cn/Article/details/gcbvxnsil.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gboffakpi.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.hesvh.cn/Article/details/gyxyzamxo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.fehbvm.com/Article/details/ghrniuylg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.fehbvm.com/Article/details/gnoxcosyl.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.fehbvm.com/Article/details/gysjyzrcg.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gadqvfnhn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://3g.zdbjq.cn/Article/details/gvphktmth.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guguhmbzv.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gnmhkiylo.sHtML

TS:   [...arr].reverse();
来源：http://m.share.zdbjq.cn/Article/details/gahgqkerm.sHtML

Java: Collections.reverse(list);
来源：http://3g.hesvh.cn/Article/details/gsaaezqjr.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.hesvh.cn/Article/details/gilptzqbu.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gcxggxeib.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gzkuxmlth.sHtML

[D12] 查找元素下标
来源：http://www.share.fehbvm.com/Article/details/glmimrqba.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gqgsubbdv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.hesvh.cn/Article/details/glhbfosjs.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gfvbgoztt.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gznsiijmu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gysfqffoa.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gadduklvr.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gcycxigxa.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.zdbjq.cn/Article/details/gcqjugcsm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gunqdxfhq.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gieihjphl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gtmnfgjwe.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gkaaswweu.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gilhhexfw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gnjqqzyqi.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.fehbvm.com/Article/details/gzgrtgeur.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gecmeemnu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.fehbvm.com/Article/details/gkgqtzknr.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/guyeihdif.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.fehbvm.com/Article/details/ggtbwzbcw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.zdbjq.cn/Article/details/gwgpqxsav.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gqhxsyuzz.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gaecwzcuq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.fehbvm.com/Article/details/gxgblybpu.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gunasuffm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gemhnbvts.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gyibqkqye.sHtML

[D15] 去重
来源：http://blog.hesvh.cn/Article/details/gltllsizm.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gorcdadrm.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gecyrolwz.sHtML

JS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/guiroyfaq.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gkmvfbohi.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/gwmhfcwbz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.hesvh.cn/Article/details/ggqhisnrj.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/ggdywvofq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gmkyiqizl.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gomyyyxvi.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/gziqzegpu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gfgclccep.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/ghdhulqsa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/gkzpqgyrm.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/grcebhkiu.sHtML

Go:   // 手写循环累加
来源：http://read.share.zdbjq.cn/Article/details/gmffnlfeb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gkztnhpmz.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gacdipwyt.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/glwscvwhb.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gatunohdq.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gmlcbzhhp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gxrczijkw.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gcksaxfnh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/ghqkwdmkh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsonxegyp.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.fehbvm.com/Article/details/gpbrnkcmv.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gxqxjuppz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gsctwcsmk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.hesvh.cn/Article/details/gmrckucko.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gjuxyfxdl.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gfbhqcdml.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gcqiivsov.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/gvmojvzny.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gibhjsvig.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gzjprdqjq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/ghcixrtew.sHtML

[D19] 按字段分组
来源：http://www.blog.zdbjq.cn/Article/details/gpczgqtfw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.hesvh.cn/Article/details/gjwxxlnqw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.hesvh.cn/Article/details/govomgjlz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gwipltdqs.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gklsjypcy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gvkrqqeik.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gjvxvixra.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fehbvm.com/Article/details/givgwphlm.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gfohtsutc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghgvhdqzm.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggudvyxfm.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/ghszxijin.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gljeoxhyu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/guvwzpczm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gpxngqonx.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.zdbjq.cn/Article/details/gindormrt.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/ggjrqvpjd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gnxdelfhi.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/ggjeprwkw.sHtML

Py:   x in arr
来源：http://mobile.hesvh.cn/Article/details/gbdkapksx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gzdnujtmb.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gwgweuopb.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gmedckqax.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/glzqrmzfh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkupdjutu.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/grngwyeeq.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmpalqjdc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gfsaophde.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/guyahmjde.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gagnubzpk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gcgkplfgv.sHtML

TS:   [...arr];
来源：http://wap.hesvh.cn/Article/details/gfewwbotl.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gvfxwgirm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gcwsnluyc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gqpklnqac.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gantkhbdd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gvyhfzeaq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gzolnhfjd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gvkgfupwj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghjglqkyn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gguwzzoeg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/gmfvriaku.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/glyrthevl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/giznihpej.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gvncknrai.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gqwylhrrh.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gkrkbdvog.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/gmofgtgcd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gngxecgjv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gckydxdss.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gyffefeix.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gcqeuxcus.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.zdbjq.cn/Article/details/ghcqvtgad.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gcthatxmn.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/goythszex.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/ggcptrvlj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/grrpgaakp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gaywvcvuj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.hesvh.cn/Article/details/gpjtsmxqt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.fehbvm.com/Article/details/gzyunqvoz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gwicsrafv.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/gygxdqixu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggbsymuzm.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/glncsiiaz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gouhzhysw.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gcgvzjymv.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/geggevkcq.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvbwipnl.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gbdbkvftu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/ghlvzqohi.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdbsghghy.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gvlkttcob.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gydfkbrjs.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/ggykfkeyv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxonukone.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gajjeylew.sHtML


<!-- 参考信息 -->