代发 wailian999

TS:   同 JS
来源：http://baike.fanxiaobao.xyz/Article/details/gfhagiftp.sHtML

Java: 方法内为块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnzrayys.sHtML

Go:   花括号块级作用域
来源：http://3g.fanxiaobao.xyz/Article/details/gecxqgwfa.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://wap.fanxiaobao.xyz/Article/details/ghdvqazut.sHtML

C#:   块级作用域
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfhiizmo.sHtML

[C11] 模块导入与导出
来源：http://blog.fanxiaobao.xyz/Article/details/gdpeksngv.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnuhrgkh.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.fanxiaobao.xyz/Article/details/grfxfietl.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://read.share.fanxiaobao.xyz/Article/details/guqbhtdta.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://baike.fanxiaobao.xyz/Article/details/gwxgecvha.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gersokdru.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.fanxiaobao.xyz/Article/details/gctyljaok.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjhupoec.sHtML

C#:   using System.Text;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzvetlxi.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/gakqekzkh.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.fanxiaobao.xyz/Article/details/ggjtavqxb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfgpnvhm.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/gwuwhobhh.sHtML

TS:   (() => { console.log("run"); })();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyomqhwg.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjnkxtfr.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgbdirvh.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfebjusa.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gybmntcjv.sHtML

[C13] 类型声明 / 类型注解
来源：http://wap.fanxiaobao.xyz/Article/details/grvdfhnzt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.blog.fanxiaobao.xyz/Article/details/guofmsuma.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gebltgcbf.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgzyofxv.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghhsxrary.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/godfkyloz.sHtML

Go:   func add(a, b int) int
来源：http://3g.fanxiaobao.xyz/Article/details/grluvhmdr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gfezukhaf.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://blog.fanxiaobao.xyz/Article/details/gkqngaemu.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gaihybdhw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.share.fanxiaobao.xyz/Article/details/guatmjjmz.sHtML

PHP:  // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/gctojetun.sHtML

JS:   // 无泛型
来源：http://read.share.fanxiaobao.xyz/Article/details/guexhvyww.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdqtzuhz.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://baike.fanxiaobao.xyz/Article/details/gjoeznlse.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjthzlvbj.sHtML

Ruby: # 无泛型
来源：http://www.share.fanxiaobao.xyz/Article/details/gqllskudb.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://baike.fanxiaobao.xyz/Article/details/gzpsacwwh.sHtML

[C15] 解构 / 展开参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghltqwpyi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://blog.fanxiaobao.xyz/Article/details/gvkhjhxis.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpmappvi.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzsvxpnm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gstcxrkup.sHtML

Java: // 无解构
来源：http://read.share.fanxiaobao.xyz/Article/details/giwaihlpi.sHtML

Go:   // 无解构
来源：http://m.share.fanxiaobao.xyz/Article/details/gxywdtvwb.sHtML

Ruby: a, b = pair
来源：http://www.share.fanxiaobao.xyz/Article/details/gqejcpbpz.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxkkfvvr.sHtML

[C16] 函数 / 方法重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gucadeqhe.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://read.share.fanxiaobao.xyz/Article/details/gdfmibqcx.sHtML

PHP:  // 无重载
来源：http://www.share.fanxiaobao.xyz/Article/details/gnpuavkol.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://baike.fanxiaobao.xyz/Article/details/gkeizmmcu.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://3g.fanxiaobao.xyz/Article/details/gevnzmtce.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqgdpcwbx.sHtML

Go:   // 无重载：用不同函数名
来源：http://m.share.fanxiaobao.xyz/Article/details/grxdtjfrj.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gylbqwgfh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gdypbrqed.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrdvlyig.sHtML

D. 数组 / 列表 / 集合
来源：http://3g.fanxiaobao.xyz/Article/details/gqurvkcup.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gobmcmvfc.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnztqdmo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.share.fanxiaobao.xyz/Article/details/gwizswbdw.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://baike.fanxiaobao.xyz/Article/details/gkwtdxbqy.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcptweuve.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://blog.fanxiaobao.xyz/Article/details/galakvmrf.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhjgnbc.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://wap.fanxiaobao.xyz/Article/details/gujavhxhz.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/grlyssqwb.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://3g.fanxiaobao.xyz/Article/details/giyffnhea.sHtML

[D02] 追加元素到末尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueecrlvz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkgljoeqs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fanxiaobao.xyz/Article/details/gfyalqzez.sHtML

JS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gijxjufwq.sHtML

TS:   arr.push(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gylnlguch.sHtML

Java: list.add(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzixypwa.sHtML

Go:   arr = append(arr, 4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyffpiaz.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjwbcdx.sHtML

C#:   list.Add(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gcwgaxdqi.sHtML

[D03] 在指定位置插入元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgpklncf.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gemmlugrx.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://3g.fanxiaobao.xyz/Article/details/gckbexyzd.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnbrepdg.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsvuxgnxv.sHtML

Java: list.add(0, 0);
来源：http://wap.fanxiaobao.xyz/Article/details/ghvltbwfq.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvuckvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwteglzyu.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzgifmab.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gzharyreo.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gagqaxymj.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gninnfrwo.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgpgzru.sHtML

TS:   arr.splice(0, 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gosifvogv.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gqimuzqxf.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbnoeebe.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiyuyvzh.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.fanxiaobao.xyz/Article/details/gsuijszej.sHtML

[D05] 访问与修改元素
来源：http://baike.fanxiaobao.xyz/Article/details/gbzlqddhw.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/gatqpbarl.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gthwgudkc.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmphssor.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzooyajdy.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gurnophyr.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtbyxxpn.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fanxiaobao.xyz/Article/details/gbbgcpoco.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://3g.fanxiaobao.xyz/Article/details/grjnucgic.sHtML

[D06] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gyorlumvi.sHtML

Py:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gccwztnqs.sHtML

PHP:  count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggskdcwfq.sHtML

JS:   arr.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glthqyprl.sHtML

TS:   arr.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grmafmrcc.sHtML

Java: list.size();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaqgiggq.sHtML

Go:   len(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gefoveirv.sHtML

Ruby: arr.length; arr.size
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwkujlff.sHtML

C#:   list.Count;
来源：http://wap.fanxiaobao.xyz/Article/details/gusyweifq.sHtML

[D07] 切片 / 取子数组
来源：http://blog.fanxiaobao.xyz/Article/details/gsngarsds.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrmebvuf.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gupolfalt.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.fanxiaobao.xyz/Article/details/gvgozwchb.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gxdetrqhi.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrxchmet.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwrtnenb.sHtML

Ruby: arr[1, 3]
来源：http://3g.fanxiaobao.xyz/Article/details/gxrvntpvq.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdlmnjbnl.sHtML

[D08] 合并两个数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuacujun.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfidaiqv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gviosxlka.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdljhdwbn.sHtML

TS:   [...a, ...b];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvwuwoi.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fanxiaobao.xyz/Article/details/gyxregjql.sHtML

Go:   append(a, b...)
来源：http://baike.fanxiaobao.xyz/Article/details/ggnnwmbbx.sHtML

Ruby: a + b;  a.concat(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gnbjrmhfg.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gyatygvae.sHtML

[D09] 排序（升序）
来源：http://wap.fanxiaobao.xyz/Article/details/ggogyqfuw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fanxiaobao.xyz/Article/details/grclxabyn.sHtML

PHP:  sort($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gforgcrif.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fanxiaobao.xyz/Article/details/gskqlfrto.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcetejgca.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.fanxiaobao.xyz/Article/details/guefzxpwt.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/ghfyowdbl.sHtML

Ruby: arr.sort
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrpkbgww.sHtML

C#:   list.Sort();
来源：http://baike.fanxiaobao.xyz/Article/details/gwjcgujks.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://mobile.fanxiaobao.xyz/Article/details/grmgwtcro.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.fanxiaobao.xyz/Article/details/gksxfhsfi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gziitnijz.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fanxiaobao.xyz/Article/details/gebgjjizt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkvusomh.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fanxiaobao.xyz/Article/details/gqpvubhbo.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gcpnwcqhz.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnhtpysix.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtzdpwgn.sHtML

[D11] 反转数组
来源：http://3g.fanxiaobao.xyz/Article/details/gvpovmjta.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fanxiaobao.xyz/Article/details/gjskodjop.sHtML

PHP:  array_reverse($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwiegvnjx.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/grujccbgo.sHtML

TS:   [...arr].reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gakpftnpz.sHtML

Java: Collections.reverse(list);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdxkvopg.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzpoixbh.sHtML

Ruby: arr.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/glgowmifq.sHtML

C#:   list.Reverse();
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuffnazn.sHtML

[D12] 查找元素下标
来源：http://baike.fanxiaobao.xyz/Article/details/ggkzmhmoo.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/geoqpxzcv.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfoblfvd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gigviouyj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjdrpoqsv.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fanxiaobao.xyz/Article/details/gbqrdnkov.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/giipjlpxo.sHtML

Ruby: arr.index(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gsubcvzjn.sHtML

C#:   list.IndexOf(x);
来源：http://baike.fanxiaobao.xyz/Article/details/gqcbhzzpc.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fanxiaobao.xyz/Article/details/gyocjevpx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuhrzxle.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbigemrj.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfnlxwxy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdriadjy.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fanxiaobao.xyz/Article/details/guwdobaxs.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://read.share.fanxiaobao.xyz/Article/details/ginqmwkvu.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpbufrvl.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmlbanjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fanxiaobao.xyz/Article/details/gbzvuolsm.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gxnqpxizy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.fanxiaobao.xyz/Article/details/gobwkpsfu.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjpskjsny.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwfbecqk.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtrpfdgfy.sHtML

Go:   // 手写循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakwoxqkf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqztkis.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gejdfmwcg.sHtML

[D15] 去重
来源：http://mobile.fanxiaobao.xyz/Article/details/gaowslqaq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fanxiaobao.xyz/Article/details/gjbihejzd.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiezfupt.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.fanxiaobao.xyz/Article/details/grvfajuzm.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudrbbjbz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxriobcym.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacalsqcc.sHtML

Ruby: arr.uniq
来源：http://read.share.fanxiaobao.xyz/Article/details/gygniwoyf.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/glgbqarox.sHtML

[D16] 求和与平均值
来源：http://blog.fanxiaobao.xyz/Article/details/gzmkrdvqw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gretcughr.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgyddprp.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gvqargikk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/glhhvjzlv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.fanxiaobao.xyz/Article/details/gaubhfari.sHtML

Go:   // 手写循环累加
来源：http://wap.fanxiaobao.xyz/Article/details/gtqtshxsr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfalcboss.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspvcuynx.sHtML

[D17] 最大值与最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gkesedouq.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gscrmkssw.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.fanxiaobao.xyz/Article/details/gktfycuhw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gupboydjl.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gwrromdav.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjdivxfn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfktbddm.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fanxiaobao.xyz/Article/details/gnvootgpe.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjtsplsu.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.fanxiaobao.xyz/Article/details/gikoxxszp.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fanxiaobao.xyz/Article/details/gflbyyeze.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gioyojbwc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gkkqljfsj.sHtML

TS:   nested.flat();
来源：http://mobile.fanxiaobao.xyz/Article/details/ghoetmgbr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gavetihnd.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gehypttyt.sHtML

Ruby: nested.flatten
来源：http://mobile.fanxiaobao.xyz/Article/details/gvukbviet.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbslswxd.sHtML

[D19] 按字段分组
来源：http://www.share.fanxiaobao.xyz/Article/details/glitrauxq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghexeujij.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/gjyfrfrzb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnufrrkk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fanxiaobao.xyz/Article/details/gaktzndgc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.fanxiaobao.xyz/Article/details/gnvqyoxwh.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fanxiaobao.xyz/Article/details/gylqbwjzf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fanxiaobao.xyz/Article/details/grrfopmqc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/glxauxipg.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmgpumje.sHtML

Py:   Counter(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/gqehaunjo.sHtML

PHP:  array_count_values($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gdufluhdh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlamiqyr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmyhoqsnh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmnyxbzj.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbvtqedt.sHtML

Ruby: arr.tally
来源：http://blog.fanxiaobao.xyz/Article/details/gynawblco.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fanxiaobao.xyz/Article/details/giaqgcxlm.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzgttqkxc.sHtML

Py:   x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/gsrclcymu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gihogbsdi.sHtML

JS:   arr.includes(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gyvpzsdod.sHtML

TS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gllapjtpz.sHtML

Java: list.contains(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gapujqbsa.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrkulwar.sHtML

Ruby: arr.include?(x)
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwbsuqk.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhqmocno.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.fanxiaobao.xyz/Article/details/gxadcyezl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhihnhpj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/gzofaxrea.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gjwzfvwse.sHtML

TS:   [...arr];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqoasmlt.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gwwfervlg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fanxiaobao.xyz/Article/details/gnjhbagul.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fanxiaobao.xyz/Article/details/gkanleuww.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/goadtlllh.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gytwnzdvr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqdsuoia.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/gnegebqtj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/glcliimjz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gasauesmd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fanxiaobao.xyz/Article/details/gergeimdu.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsylsiqx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsifuerqh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxxvvjeg.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/ghizrfiil.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/galnzoovg.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gesotsrkl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqbfplbu.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlyhuztw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmhdiwqn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvchsddip.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcsnbovp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fanxiaobao.xyz/Article/details/gdebzkcwt.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fanxiaobao.xyz/Article/details/gadjskjaj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fanxiaobao.xyz/Article/details/gkimmklmp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwauykrf.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/giebjxvcc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/glfbbrhgt.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gohktnbxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fanxiaobao.xyz/Article/details/gnivdkwiy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fanxiaobao.xyz/Article/details/glsobhtzz.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzshwdyum.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gizzxpzmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxrhamjb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhvysxqj.sHtML

JS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gxuyrbgzf.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutipzucq.sHtML

Java: String.join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gllkzecll.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gowehxphi.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godrkbsix.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fanxiaobao.xyz/Article/details/gxsfdkucf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gcofpnczh.sHtML

E. 字符串处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gmywvsdrs.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gcjxzzyng.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcuphxzt.sHtML


<!-- 参考信息 -->