代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.m.share.fehbvm.com/Article/details/gvncafbmz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://3g.fehbvm.com/Article/details/gzkkzxuyz.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://baike.fehbvm.com/Article/details/gshydweqn.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://mobile.zdbjq.cn/Article/details/goknjwldu.sHtML

[C10] 变量作用域
来源：http://blog.hesvh.cn/Article/details/gbvaoikiy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.m.share.fehbvm.com/Article/details/gzefgncdz.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://wap.fehbvm.com/Article/details/gsjjjbpjy.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://mobile.fehbvm.com/Article/details/guknqvrhc.sHtML

TS:   同 JS
来源：http://www.share.zdbjq.cn/Article/details/gxlrqudgm.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fehbvm.com/Article/details/gofqntpte.sHtML

Go:   花括号块级作用域
来源：http://wap.hesvh.cn/Article/details/gqpypxbjh.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gzatrhnkv.sHtML

C#:   块级作用域
来源：http://wap.fehbvm.com/Article/details/gbxcqhwuj.sHtML

[C11] 模块导入与导出
来源：http://m.share.zdbjq.cn/Article/details/gkzaxeepe.sHtML

Py:   from module import func
来源：http://mobile.zdbjq.cn/Article/details/glmfxfgzv.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/gdqtknssy.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.hesvh.cn/Article/details/gwckggczy.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fehbvm.com/Article/details/gnmgmewoa.sHtML

Java: import java.util.List;
来源：http://www.blog.hesvh.cn/Article/details/gtmgzllbc.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://blog.zdbjq.cn/Article/details/gbozdeepb.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.m.share.zdbjq.cn/Article/details/gjbsytjii.sHtML

C#:   using System.Text;
来源：http://3g.fehbvm.com/Article/details/gsmavibbu.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.fehbvm.com/Article/details/gsnibomzw.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.zdbjq.cn/Article/details/gpkugjbhz.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gwzqovvjm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gskienaoq.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.share.hesvh.cn/Article/details/gvckwipdc.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.share.hesvh.cn/Article/details/gaigbeoln.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/ghnxoyuqh.sHtML

Ruby: -> { puts "run" }.call
来源：http://baike.hesvh.cn/Article/details/gyorakkuq.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gzoevjxqi.sHtML

[C13] 类型声明 / 类型注解
来源：http://baike.fehbvm.com/Article/details/gsnymjwwa.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.fehbvm.com/Article/details/geaymnglj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gnmvrxtfq.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.fehbvm.com/Article/details/gpfrcscch.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gixxbpegc.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gvclkands.sHtML

Go:   func add(a, b int) int
来源：http://3g.fehbvm.com/Article/details/gerqdabvn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.hesvh.cn/Article/details/gvaqwgwke.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.hesvh.cn/Article/details/gphfxauug.sHtML

[C14] 泛型函数
来源：http://read.share.zdbjq.cn/Article/details/ggiwkffvf.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gzjyjhgpj.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/gktmgxvet.sHtML

JS:   // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/gcuhbzcbm.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gsvjdzwwt.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.hesvh.cn/Article/details/gukubqzbl.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://read.share.hesvh.cn/Article/details/gttabaeep.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gyutfixbl.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://mobile.hesvh.cn/Article/details/gefmbxzcy.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fehbvm.com/Article/details/gnbulgugq.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://m.share.hesvh.cn/Article/details/gfnjptzdv.sHtML

PHP:  [$a, $b] = $pair;
来源：http://m.share.zdbjq.cn/Article/details/gistemdxq.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://mobile.hesvh.cn/Article/details/gxrjbisst.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://wap.hesvh.cn/Article/details/gsvyfemno.sHtML

Java: // 无解构
来源：http://baike.fehbvm.com/Article/details/gxrewtazf.sHtML

Go:   // 无解构
来源：http://mobile.fehbvm.com/Article/details/gvnjclrtz.sHtML

Ruby: a, b = pair
来源：http://www.m.share.fehbvm.com/Article/details/gjaetsisj.sHtML

C#:   var (a, b) = pair;
来源：http://read.share.fehbvm.com/Article/details/gezrfvbih.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.hesvh.cn/Article/details/gcgidevju.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gfugoibdn.sHtML

PHP:  // 无重载
来源：http://3g.fehbvm.com/Article/details/ganklbvsg.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://3g.fehbvm.com/Article/details/gibwqrndd.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gnxkciktk.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcfikifcy.sHtML

Go:   // 无重载：用不同函数名
来源：http://www.blog.hesvh.cn/Article/details/ggaeeftay.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fehbvm.com/Article/details/gbqqhyzwh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://baike.fehbvm.com/Article/details/gvsqunyql.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gbqwiangj.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.zdbjq.cn/Article/details/gneflyjbm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijjwpjzq.sHtML

[D01] 创建数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gttmfnqiq.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://read.share.fehbvm.com/Article/details/gmcdcethx.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.m.share.fehbvm.com/Article/details/gbqzekaey.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://3g.fehbvm.com/Article/details/ggdjpzkpy.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.share.zdbjq.cn/Article/details/gnmebxvxn.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wap.hesvh.cn/Article/details/gfwfwnnph.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://3g.zdbjq.cn/Article/details/gursadrbb.sHtML

Ruby: arr = [1, 2, 3]
来源：http://baike.hesvh.cn/Article/details/galznyooo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/glaqxijps.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gwgdaszuq.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://read.share.hesvh.cn/Article/details/gqznuhwgh.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.zdbjq.cn/Article/details/ghntvfvcy.sHtML

JS:   arr.push(4);
来源：http://www.share.fehbvm.com/Article/details/giifqezaq.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gvftiprzf.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gcznsxndj.sHtML

Go:   arr = append(arr, 4)
来源：http://3g.hesvh.cn/Article/details/griqfnyhk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://blog.zdbjq.cn/Article/details/gyoiqxhfz.sHtML

C#:   list.Add(4);
来源：http://www.share.fehbvm.com/Article/details/guzuhmtav.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gqoispzwb.sHtML

Py:   arr.insert(0, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gkigsfxyr.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.zdbjq.cn/Article/details/gwqiwgils.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/gbqfxifpq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fehbvm.com/Article/details/gyzwregsr.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gooawgcyh.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://3g.hesvh.cn/Article/details/gvjzlgeet.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://blog.hesvh.cn/Article/details/gbjvxgywb.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.fehbvm.com/Article/details/gosisysab.sHtML

[D04] 删除元素
来源：http://baike.zdbjq.cn/Article/details/ggogevdmd.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://baike.zdbjq.cn/Article/details/gtxprswny.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wap.zdbjq.cn/Article/details/gcquuhmxq.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.zdbjq.cn/Article/details/gkxoqpuqn.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gmkuckwcf.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/giazwrvdp.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fehbvm.com/Article/details/gmqhtcuze.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gxyqvlmlh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gcnaoagak.sHtML

[D05] 访问与修改元素
来源：http://3g.hesvh.cn/Article/details/gphesatau.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gdarfqagg.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.share.hesvh.cn/Article/details/gaigjfqrw.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/gnjpmwxio.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.fehbvm.com/Article/details/gnxkbxhpp.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://blog.fehbvm.com/Article/details/guewjqead.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.blog.zdbjq.cn/Article/details/gvcjwqiwv.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gplcnenfk.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://read.share.hesvh.cn/Article/details/gifehffph.sHtML

[D06] 数组长度
来源：http://www.share.fehbvm.com/Article/details/gxzkcocie.sHtML

Py:   len(arr)
来源：http://3g.zdbjq.cn/Article/details/gghxewixa.sHtML

PHP:  count($arr);
来源：http://www.share.hesvh.cn/Article/details/gunjeqbsd.sHtML

JS:   arr.length
来源：http://baike.hesvh.cn/Article/details/gvvmaxbhu.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/glitxhtqm.sHtML

Java: list.size();
来源：http://www.share.hesvh.cn/Article/details/ghbblkrrd.sHtML

Go:   len(arr)
来源：http://read.share.zdbjq.cn/Article/details/gmumkzkjh.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fehbvm.com/Article/details/gxypmxtqg.sHtML

C#:   list.Count;
来源：http://blog.zdbjq.cn/Article/details/gkrymacxj.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.hesvh.cn/Article/details/gkwltbail.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.zdbjq.cn/Article/details/gwovnxkae.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gvfzgtwki.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/grulisxrx.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.zdbjq.cn/Article/details/gybzkjtfn.sHtML

Java: list.subList(1, 4);
来源：http://www.share.zdbjq.cn/Article/details/gxpccijlv.sHtML

Go:   arr[1:4]
来源：http://3g.hesvh.cn/Article/details/gkwrsjgqu.sHtML

Ruby: arr[1, 3]
来源：http://baike.zdbjq.cn/Article/details/grxasabyw.sHtML

C#:   list.GetRange(1, 3);
来源：http://mobile.hesvh.cn/Article/details/gfddgiqnx.sHtML

[D08] 合并两个数组
来源：http://www.blog.zdbjq.cn/Article/details/gnoqnzhdy.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.hesvh.cn/Article/details/ggneuqmfo.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.fehbvm.com/Article/details/guiejyxzk.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.blog.hesvh.cn/Article/details/gymxlhiby.sHtML

TS:   [...a, ...b];
来源：http://www.share.hesvh.cn/Article/details/gkypekysu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/gqluvzgcm.sHtML

Go:   append(a, b...)
来源：http://m.share.zdbjq.cn/Article/details/giaxjtzih.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gskqtkowk.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/ghppqgxud.sHtML

[D09] 排序（升序）
来源：http://blog.fehbvm.com/Article/details/gtsiyvkyb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.fehbvm.com/Article/details/gmeyprctn.sHtML

PHP:  sort($arr);
来源：http://blog.fehbvm.com/Article/details/gzeyooiib.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fehbvm.com/Article/details/gzfwtaofo.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.fehbvm.com/Article/details/gwxojpsrv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.hesvh.cn/Article/details/grycmuhbk.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gzyqsaynb.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gmmtjccok.sHtML

C#:   list.Sort();
来源：http://mobile.zdbjq.cn/Article/details/gkkyaesrr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fehbvm.com/Article/details/gvgxdbtec.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gtqukfjgy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gzlypbtze.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/glvcjkjqn.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gfemvepwf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/goiesucqp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/grlpejihc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gvoiutfhp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fehbvm.com/Article/details/ggqtovjtu.sHtML

[D11] 反转数组
来源：http://blog.zdbjq.cn/Article/details/gkyiiymkn.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gdfhcilns.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gvdbimrpl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gdmxqvgnr.sHtML

TS:   [...arr].reverse();
来源：http://wap.zdbjq.cn/Article/details/gghdhiahv.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gsumuzjrl.sHtML

Go:   slices.Reverse(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gctqhbqiu.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/gizadruaj.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gcpgwjhkq.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/godvhhccw.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gtltvmcsm.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mobile.zdbjq.cn/Article/details/govdmplxv.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.hesvh.cn/Article/details/gsmitogce.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gscaboboq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/guvaauxwf.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfrwopetz.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gwlcssmbw.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fehbvm.com/Article/details/gmyaxmngk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gttivkrfp.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gsmxuthsb.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/gbxjqjglz.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/ghnmfdzmm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmimknzkw.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gthycuplq.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.fehbvm.com/Article/details/ghojlnxrz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/gndgkqmjs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.zdbjq.cn/Article/details/grwjhoabt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gyuxgroxr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.hesvh.cn/Article/details/ghkhmiusb.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/guuygpctu.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/geoilusqi.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.fehbvm.com/Article/details/gbatkidhz.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gylglaqij.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gtaglfbzx.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gyhcgjnre.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/giwxpocjs.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gygkszxyl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.hesvh.cn/Article/details/gsulumuti.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gzkyavtfv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.zdbjq.cn/Article/details/gjnvrvsky.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggesczfvw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gqracocgw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.zdbjq.cn/Article/details/gdnddglol.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gglacpqgk.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gpwjwlkyd.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gudwhpqxd.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/gdsglowig.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzxlqjxyr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gdptkcjto.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/grxqupfeg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gwzrzqqzt.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/gpowvhgsu.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gufqemkdl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.fehbvm.com/Article/details/gmvxxpjob.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gkrofqlwg.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gagwolbcb.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/gxsbxinel.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.hesvh.cn/Article/details/gqdpmetan.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gcrgizwmr.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggwxetdbv.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/gldquyvok.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/ghlkvkwkx.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.hesvh.cn/Article/details/gecwtketo.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/ghybakzll.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gavqonioj.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gipsqwrjp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gtdfdqefp.sHtML

TS:   nested.flat();
来源：http://www.m.share.hesvh.cn/Article/details/giugknpmt.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gedvvtsvr.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gryqzcfry.sHtML

Ruby: nested.flatten
来源：http://www.blog.hesvh.cn/Article/details/guetgtetk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/grysujrsm.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/grsnrrbgp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gmcmhpvyy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gbfsztglo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gveybmkii.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gfwzbidqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/glkejylna.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/garmhmblx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gnwncczwj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gfeehsocv.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fehbvm.com/Article/details/groatrfqd.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gkwmzpfuj.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gkybgqttw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ghbpfpesm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gzitdfxbt.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gtipofamc.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gkqfwsokk.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gkulajgnx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/geyqhttti.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gcttiawot.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gjrbqnrek.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gpqdhuvol.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gbpscdmql.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gfbxhzxzq.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqiyhgosl.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/ggpndyzej.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gbqenatlq.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdfbisyqv.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gpqeqzefu.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gcwpbdvbx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gxdmbvols.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/galpgfxsv.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gxovqapkx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gpjkpovjy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/goujaumft.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwqxokv.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/greorcpti.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/guqxvgwnf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.hesvh.cn/Article/details/glwhtxhii.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/ghyzucdxm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gujccmavp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gsqyggapf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gszfrcaee.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/glmcdzrei.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ggmbtkswv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.hesvh.cn/Article/details/ggrcxcdjs.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gcqkwqomp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gpfjggzng.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gsdrtvsrl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/grtnmpnth.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvkctfndh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gnzvqlsfj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gzocofelv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/grbrwxnve.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gnytvmcbw.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gijxzobbq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/gwooqtalq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gnogbzfam.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/guwmtzmgp.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gbwkdthbc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gzbvdogxx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gaqsfpurg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/guphfjgxs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.hesvh.cn/Article/details/gflkdianj.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gwsihpchg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gegvxycxa.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gbzrcceie.sHtML

JS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gvfiyqebg.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gkpvdedsa.sHtML


<!-- 参考信息 -->