代发 wailian999

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gfohowapf.sHtML

[C11] 模块导入与导出
来源：http://3g.zdbjq.cn/Article/details/gdtvcnzhx.sHtML

Py:   from module import func
来源：http://wap.hesvh.cn/Article/details/gxkbioqyw.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gucucxcrp.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.share.fehbvm.com/Article/details/gzrmiwnmh.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.hesvh.cn/Article/details/grspjigdw.sHtML

Java: import java.util.List;
来源：http://3g.fehbvm.com/Article/details/gvskatdwe.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.hesvh.cn/Article/details/gvathoxfs.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.share.hesvh.cn/Article/details/gdvgmcwht.sHtML

C#:   using System.Text;
来源：http://read.share.hesvh.cn/Article/details/gcrorsdfv.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.fehbvm.com/Article/details/gpdcxtude.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gsxbphlll.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.m.share.fehbvm.com/Article/details/gxuahrpjm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/ghquswate.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gbsfjdgyl.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.fehbvm.com/Article/details/gjilrgtlq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.hesvh.cn/Article/details/gdtdumucg.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.share.hesvh.cn/Article/details/gkzzvtttm.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://wap.zdbjq.cn/Article/details/gwndfkjdd.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gqtbailkt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.hesvh.cn/Article/details/ggsumvdjs.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.zdbjq.cn/Article/details/goestsukj.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://blog.hesvh.cn/Article/details/gyhzsctpg.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gqyknjiqs.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gviwulutf.sHtML

Go:   func add(a, b int) int
来源：http://baike.zdbjq.cn/Article/details/gjzdwfnja.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.zdbjq.cn/Article/details/gphdgsini.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.hesvh.cn/Article/details/gqzszwyau.sHtML

[C14] 泛型函数
来源：http://wap.fehbvm.com/Article/details/gekbbiroy.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://3g.hesvh.cn/Article/details/gmoenxdjx.sHtML

PHP:  // 无泛型
来源：http://www.m.share.zdbjq.cn/Article/details/grybbvglm.sHtML

JS:   // 无泛型
来源：http://blog.fehbvm.com/Article/details/gzoulclwj.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://3g.zdbjq.cn/Article/details/gttwurtuy.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.blog.fehbvm.com/Article/details/ggxubokww.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gyvbbbkjy.sHtML

Ruby: # 无泛型
来源：http://wap.hesvh.cn/Article/details/gheizhavm.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.hesvh.cn/Article/details/gkqnnztzf.sHtML

[C15] 解构 / 展开参数
来源：http://blog.hesvh.cn/Article/details/gwvwjtqof.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.hesvh.cn/Article/details/ggxrruorb.sHtML

PHP:  [$a, $b] = $pair;
来源：http://mobile.hesvh.cn/Article/details/gqgrojwqd.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.zdbjq.cn/Article/details/gzmcnisze.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.share.zdbjq.cn/Article/details/gwqezzief.sHtML

Java: // 无解构
来源：http://baike.zdbjq.cn/Article/details/gphmvjqom.sHtML

Go:   // 无解构
来源：http://www.m.share.hesvh.cn/Article/details/gpjglbiag.sHtML

Ruby: a, b = pair
来源：http://m.share.hesvh.cn/Article/details/gurdwrmci.sHtML

C#:   var (a, b) = pair;
来源：http://baike.zdbjq.cn/Article/details/gzfbagfgn.sHtML

[C16] 函数 / 方法重载
来源：http://3g.hesvh.cn/Article/details/gausnyxnx.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.blog.fehbvm.com/Article/details/gycexolql.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gbqmyxmuq.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://blog.fehbvm.com/Article/details/gkaaomcsx.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/gdrheuwiw.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://wap.zdbjq.cn/Article/details/gjfxsfzfj.sHtML

Go:   // 无重载：用不同函数名
来源：http://baike.hesvh.cn/Article/details/gjbcmutps.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.fehbvm.com/Article/details/gourisgbx.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.hesvh.cn/Article/details/gwgigrxta.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcarxmzfw.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gmttulegt.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/greizspgw.sHtML

[D01] 创建数组 / 列表
来源：http://blog.hesvh.cn/Article/details/gctntytua.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.hesvh.cn/Article/details/guwrelqld.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fehbvm.com/Article/details/gdggstpbo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://blog.hesvh.cn/Article/details/gvkzzcmga.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://m.share.hesvh.cn/Article/details/gpmikjvzp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mobile.hesvh.cn/Article/details/gctatxtor.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://www.m.share.fehbvm.com/Article/details/gvksismzk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.zdbjq.cn/Article/details/gpsvmwhfg.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.zdbjq.cn/Article/details/gvcsvdxvo.sHtML

[D02] 追加元素到末尾
来源：http://www.m.share.fehbvm.com/Article/details/gsuoopkzi.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.fehbvm.com/Article/details/gbujagfwm.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/ghqzuutzb.sHtML

JS:   arr.push(4);
来源：http://www.share.zdbjq.cn/Article/details/gxrfalusv.sHtML

TS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gzxpdndsb.sHtML

Java: list.add(4);
来源：http://m.share.fehbvm.com/Article/details/gigtgtnwx.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gkubgdtdk.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.blog.zdbjq.cn/Article/details/ghxpeqsfs.sHtML

C#:   list.Add(4);
来源：http://www.blog.hesvh.cn/Article/details/glfdcyolq.sHtML

[D03] 在指定位置插入元素
来源：http://wap.hesvh.cn/Article/details/gafbtmmtd.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgweouig.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.fehbvm.com/Article/details/gundosckc.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://wap.zdbjq.cn/Article/details/gwzdcvnvn.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.hesvh.cn/Article/details/gxaakvfmk.sHtML

Java: list.add(0, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gyavkitkk.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://wap.fehbvm.com/Article/details/gvgrgxxlj.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gasdkadva.sHtML

C#:   list.Insert(0, 0);
来源：http://baike.fehbvm.com/Article/details/gwxtjolph.sHtML

[D04] 删除元素
来源：http://blog.zdbjq.cn/Article/details/glezqhpfr.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.hesvh.cn/Article/details/gnugshvwu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.hesvh.cn/Article/details/gnhmarjcp.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://3g.zdbjq.cn/Article/details/gehbbztyt.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.zdbjq.cn/Article/details/gheyrpbef.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://read.share.zdbjq.cn/Article/details/gtvhjhiwg.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.zdbjq.cn/Article/details/gbtfrsocj.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://blog.hesvh.cn/Article/details/gmgchjuha.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://mobile.fehbvm.com/Article/details/gckmxdxhz.sHtML

[D05] 访问与修改元素
来源：http://www.share.zdbjq.cn/Article/details/gcovtwsrx.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://3g.zdbjq.cn/Article/details/gsjyqhyrh.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://baike.zdbjq.cn/Article/details/gygciuhpr.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gtdvwjhmr.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://mobile.hesvh.cn/Article/details/ghhqxuqak.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.blog.fehbvm.com/Article/details/gwbeeuwtn.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gqrrofkwq.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.fehbvm.com/Article/details/gwfayurrz.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.share.fehbvm.com/Article/details/goduwrwlx.sHtML

[D06] 数组长度
来源：http://3g.hesvh.cn/Article/details/gskcbgchf.sHtML

Py:   len(arr)
来源：http://www.blog.hesvh.cn/Article/details/giiqoqkaf.sHtML

PHP:  count($arr);
来源：http://read.share.hesvh.cn/Article/details/gafwdnbul.sHtML

JS:   arr.length
来源：http://3g.hesvh.cn/Article/details/gomobinuu.sHtML

TS:   arr.length
来源：http://mobile.zdbjq.cn/Article/details/gsbvrtsjg.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gvmxjkiff.sHtML

Go:   len(arr)
来源：http://www.share.fehbvm.com/Article/details/gyffspmoy.sHtML

Ruby: arr.length; arr.size
来源：http://baike.hesvh.cn/Article/details/gxliaijhz.sHtML

C#:   list.Count;
来源：http://www.share.fehbvm.com/Article/details/gaguraota.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fehbvm.com/Article/details/gtpubmwxr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://3g.hesvh.cn/Article/details/gnwfgrtmq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://blog.zdbjq.cn/Article/details/gnefexmgb.sHtML

JS:   arr.slice(1, 4);
来源：http://www.blog.zdbjq.cn/Article/details/gaskjslgf.sHtML

TS:   arr.slice(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gninbuhag.sHtML

Java: list.subList(1, 4);
来源：http://m.share.hesvh.cn/Article/details/gnrykhtfd.sHtML

Go:   arr[1:4]
来源：http://baike.fehbvm.com/Article/details/gwihyvxbb.sHtML

Ruby: arr[1, 3]
来源：http://blog.fehbvm.com/Article/details/gqzwcarwc.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.zdbjq.cn/Article/details/gaotjhjfo.sHtML

[D08] 合并两个数组
来源：http://blog.fehbvm.com/Article/details/ggxtrtpxd.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.fehbvm.com/Article/details/guytpjfgl.sHtML

PHP:  array_merge($a, $b);
来源：http://m.share.hesvh.cn/Article/details/gbqjgjgwn.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.zdbjq.cn/Article/details/gdawztuut.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/ggmhgugst.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://read.share.hesvh.cn/Article/details/goflixiom.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gytiurpvc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.zdbjq.cn/Article/details/gggtdvhtk.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.zdbjq.cn/Article/details/guutbvmhp.sHtML

[D09] 排序（升序）
来源：http://m.share.fehbvm.com/Article/details/gxrkpcafu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gosunkbtc.sHtML

PHP:  sort($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gcupqldyb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://3g.zdbjq.cn/Article/details/gdugerfvk.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.zdbjq.cn/Article/details/gdqlmxwgu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.zdbjq.cn/Article/details/gmaagnyff.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/goispvoxc.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gmxuaqkrh.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/gajgrankh.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.fehbvm.com/Article/details/gtcfjaodf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gtqhvsymy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gtcxfiglx.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.zdbjq.cn/Article/details/gqslqhtyd.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/ghpvhmkvq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.hesvh.cn/Article/details/gyqlgenak.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.blog.hesvh.cn/Article/details/gycbgnimu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.fehbvm.com/Article/details/gfdusiamr.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.hesvh.cn/Article/details/geusmpojw.sHtML

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gusdndmna.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.zdbjq.cn/Article/details/gecspuvkc.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.hesvh.cn/Article/details/gmzyyftzm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.hesvh.cn/Article/details/grcovkgwb.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gjktfojwa.sHtML

Java: Collections.reverse(list);
来源：http://www.share.hesvh.cn/Article/details/givhmkhvo.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.fehbvm.com/Article/details/giuidmvia.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/ghyllmbwv.sHtML

C#:   list.Reverse();
来源：http://baike.fehbvm.com/Article/details/ghezlcedt.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/gsdzgtqkv.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gqhgrrvig.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gaizmitjc.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gvsphrsqa.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gbznlwwyq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gwzrjvclr.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gkwhhtpom.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnsganmsv.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gkercvnuw.sHtML

[D13] 过滤（保留满足条件的）
来源：http://baike.fehbvm.com/Article/details/gvteuwedt.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/gldangnvm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.fehbvm.com/Article/details/girivuayq.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gieubxgzk.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gdgvoxvtc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.zdbjq.cn/Article/details/gvmeqhysk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gaygiyzpc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.hesvh.cn/Article/details/gvlnqtqjt.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gokkjgowu.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/ghoxmjkqd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gwgzhwtgh.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/ggpnsutmt.sHtML

JS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/ggfpfarxc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/ghiascrbb.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fehbvm.com/Article/details/gcbnjduzw.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gknwbxwnk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.zdbjq.cn/Article/details/gwgoaajkl.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gvmatrfif.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gjtkmtbgd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/gdoetpoaz.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gzwgravye.sHtML

JS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/ghyqehfzu.sHtML

TS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gvsopwrmk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.fehbvm.com/Article/details/gkvjidfmz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gxbthccgn.sHtML

Ruby: arr.uniq
来源：http://baike.hesvh.cn/Article/details/ggkcxpqop.sHtML

C#:   list.Distinct().ToList()
来源：http://read.share.zdbjq.cn/Article/details/gjbjvbarf.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gefiaiohc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.fehbvm.com/Article/details/ghsdfcmfo.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gixypizvf.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/grmckqfwn.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/goinsgvgw.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gryrneeyb.sHtML

Go:   // 手写循环累加
来源：http://wap.zdbjq.cn/Article/details/gbtwptezy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gcgftbqnr.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gkgsqajlv.sHtML

[D17] 最大值与最小值
来源：http://read.share.fehbvm.com/Article/details/glspwnadz.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/gjneixnhi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gpyvanvza.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gpohvsscg.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gohwdweur.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.hesvh.cn/Article/details/giejvnhsn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/glwqqxmbq.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.zdbjq.cn/Article/details/gcvdtjwzp.sHtML

C#:   list.Max();  list.Min()
来源：http://m.share.zdbjq.cn/Article/details/gcfayzdpr.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gmdjcxqqo.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/ghkrkrzgy.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gytqenncz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gkkndnpqf.sHtML

TS:   nested.flat();
来源：http://www.share.zdbjq.cn/Article/details/glzedcpwx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gsurjkurh.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gypjipdvb.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/goxkxqxsk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gfvzebyqr.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/gmwgufkby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gdfwybmif.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gyslesutl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.zdbjq.cn/Article/details/ghmxendnn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.fehbvm.com/Article/details/gzfagprmy.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gkzfrcder.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gjltrovnq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gunjxwkny.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gwjxdrfxn.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gloxitguq.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gxamgnppg.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fehbvm.com/Article/details/ghguoyuuj.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/grjegjzle.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gakvbvfkq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gsjuwgczk.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gfsnfawfv.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gxehnaapx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gfmbqkklu.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gozisdfts.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gkcfxqwpa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.fehbvm.com/Article/details/gddgmlilw.sHtML

JS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gpzzfelai.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gabfwdhmz.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gjkgcvntw.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.hesvh.cn/Article/details/ghtzwymnc.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gkqeldxnc.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/gapwfdxdi.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/gbuklcqzq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gvkplatzz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.hesvh.cn/Article/details/gkpxittiu.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gyqmmfewz.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/gbqdmgbpu.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gkdllyuzb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.hesvh.cn/Article/details/gbkseacpa.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gmohkmpbd.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gfkmiibcw.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gfoviymrf.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gjzzvtvvg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gzsuqdxlq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gtbqjamwq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fehbvm.com/Article/details/graomvrkf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gcmfmvpuq.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gencybgew.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gocoawnlh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/geetwxfui.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gufbipzcj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmudnihor.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/ggjeiszuc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gojtohigt.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gjdjozwfc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gvbtpkegf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gjpfvovgc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gyapviopf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/grpptgkhh.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gkqvnsibb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/gdpcbhnqg.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gagqiydon.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/gojwcaejl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/guyfldamb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gentahvtq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpyqgocud.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/goxkqyxwq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/grlpzytgm.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gzpqxlppv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gbdzapueg.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gyqvexsny.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzicjrdup.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gdnaapjky.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gleecdrut.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gzgxhwqua.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gkbdrakpp.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gsqwxnxjy.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkntrsizy.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gbhplfnsh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grwmpwxxv.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gwskvkxoj.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gsuvpzxzt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gnbrupyxd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gbyqgjcik.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gqzqukrzg.sHtML


<!-- 参考信息 -->