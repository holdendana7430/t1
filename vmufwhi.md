代发 wailian999

C#:   块级作用域
来源：http://www.share.fanxiaobao.xyz/Article/details/gopsnffuf.sHtML

[C11] 模块导入与导出
来源：http://mobile.fanxiaobao.xyz/Article/details/glpwngaud.sHtML

Py:   from module import func
来源：http://read.share.fanxiaobao.xyz/Article/details/grykyyuyb.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.fanxiaobao.xyz/Article/details/gifyefzoe.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.fanxiaobao.xyz/Article/details/gvruijmtl.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://wap.fanxiaobao.xyz/Article/details/gmnscccff.sHtML

Java: import java.util.List;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlzcqpxf.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://wap.fanxiaobao.xyz/Article/details/gaqxekxfa.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjhpxtyu.sHtML

C#:   using System.Text;
来源：http://blog.fanxiaobao.xyz/Article/details/gysdldoqv.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.fanxiaobao.xyz/Article/details/giyugqkjf.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmpavxzg.sHtML

PHP:  (function () { echo "run"; })();
来源：http://blog.fanxiaobao.xyz/Article/details/gsqctydhh.sHtML

JS:   (() => { console.log("run"); })();
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsnuwhvb.sHtML

TS:   (() => { console.log("run"); })();
来源：http://baike.fanxiaobao.xyz/Article/details/giexuhtor.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://3g.fanxiaobao.xyz/Article/details/goywlcras.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylfoqirt.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyquyrzh.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvzlkwsuq.sHtML

[C13] 类型声明 / 类型注解
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbhtqwgp.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.fanxiaobao.xyz/Article/details/gnshzfwku.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvhfgicdi.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.share.fanxiaobao.xyz/Article/details/geuuyhuoa.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gjgpnfcpq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganuxjvde.sHtML

Go:   func add(a, b int) int
来源：http://blog.fanxiaobao.xyz/Article/details/gpcoczyzx.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://blog.fanxiaobao.xyz/Article/details/gdellcfrw.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdykimiak.sHtML

[C14] 泛型函数
来源：http://3g.fanxiaobao.xyz/Article/details/gahtjovpu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://wap.fanxiaobao.xyz/Article/details/gplxjhxve.sHtML

PHP:  // 无泛型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfhuwoqo.sHtML

JS:   // 无泛型
来源：http://3g.fanxiaobao.xyz/Article/details/gbxagnfuw.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbtfzaji.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgnyjpix.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.fanxiaobao.xyz/Article/details/gjkdxcdxd.sHtML

Ruby: # 无泛型
来源：http://wap.fanxiaobao.xyz/Article/details/ghcnsjlpk.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhjtflwh.sHtML

[C15] 解构 / 展开参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtfqgomp.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fanxiaobao.xyz/Article/details/guasjpwgy.sHtML

PHP:  [$a, $b] = $pair;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmobwwao.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://wap.fanxiaobao.xyz/Article/details/glwvpmsfq.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gjuvectdt.sHtML

Java: // 无解构
来源：http://www.share.fanxiaobao.xyz/Article/details/gvszublzx.sHtML

Go:   // 无解构
来源：http://blog.fanxiaobao.xyz/Article/details/gbcfrzmxe.sHtML

Ruby: a, b = pair
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhjwxzyt.sHtML

C#:   var (a, b) = pair;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpkvfoky.sHtML

[C16] 函数 / 方法重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfwwhjed.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gefpcciqs.sHtML

PHP:  // 无重载
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsheetpp.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvayixcry.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://baike.fanxiaobao.xyz/Article/details/gjwmxmxee.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzmptmctu.sHtML

Go:   // 无重载：用不同函数名
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyuuhlqs.sHtML

Ruby: # 无重载：靠动态参数
来源：http://3g.fanxiaobao.xyz/Article/details/gyiebinoh.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfibojfuw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfbkjpwap.sHtML

D. 数组 / 列表 / 集合
来源：http://wap.fanxiaobao.xyz/Article/details/gjazmrwsw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtotfontk.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.fanxiaobao.xyz/Article/details/gwflbffbd.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnsqdjg.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://blog.fanxiaobao.xyz/Article/details/gxkvsnbbo.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayppadie.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fanxiaobao.xyz/Article/details/guocaasoi.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.fanxiaobao.xyz/Article/details/gegxmtwgs.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://read.share.fanxiaobao.xyz/Article/details/glnguwntj.sHtML

Ruby: arr = [1, 2, 3]
来源：http://mobile.fanxiaobao.xyz/Article/details/giokanrgq.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://wap.fanxiaobao.xyz/Article/details/gzmdzlysv.sHtML

[D02] 追加元素到末尾
来源：http://wap.fanxiaobao.xyz/Article/details/ghlsltvsg.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fanxiaobao.xyz/Article/details/guifmmade.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://3g.fanxiaobao.xyz/Article/details/glwwxcesr.sHtML

JS:   arr.push(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywkqhkwc.sHtML

TS:   arr.push(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/githvaenp.sHtML

Java: list.add(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhfdijeb.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyfwmdvf.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gybtpsyfa.sHtML

C#:   list.Add(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpniqjpuq.sHtML

[D03] 在指定位置插入元素
来源：http://3g.fanxiaobao.xyz/Article/details/glhofovne.sHtML

Py:   arr.insert(0, 0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzclvoltq.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://mobile.fanxiaobao.xyz/Article/details/glnbowcpk.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghhvdhkt.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://3g.fanxiaobao.xyz/Article/details/glpbmzclu.sHtML

Java: list.add(0, 0);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmochplu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gzjveziry.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkasmeos.sHtML

C#:   list.Insert(0, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiielutk.sHtML

[D04] 删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gcciqmqro.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://blog.fanxiaobao.xyz/Article/details/gvggdflfi.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gbfszkbgc.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswyltlqg.sHtML

TS:   arr.splice(0, 1);
来源：http://wap.fanxiaobao.xyz/Article/details/glirwhbka.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxdxjayx.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.fanxiaobao.xyz/Article/details/gqnfcyodz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.fanxiaobao.xyz/Article/details/gkswcpako.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://baike.fanxiaobao.xyz/Article/details/gkjqwliny.sHtML

[D05] 访问与修改元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghisorbjo.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fanxiaobao.xyz/Article/details/goeunzmox.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbudjkyry.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://blog.fanxiaobao.xyz/Article/details/gzhstrped.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.share.fanxiaobao.xyz/Article/details/gliexjjyc.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fanxiaobao.xyz/Article/details/ggvyjspvo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://mobile.fanxiaobao.xyz/Article/details/gcuebcnmx.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://baike.fanxiaobao.xyz/Article/details/ghitrlnkh.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsitdfje.sHtML

[D06] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/geqybwfrn.sHtML

Py:   len(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gwsrctwpn.sHtML

PHP:  count($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gugsshysc.sHtML

JS:   arr.length
来源：http://mobile.fanxiaobao.xyz/Article/details/grfzcxlzt.sHtML

TS:   arr.length
来源：http://read.share.fanxiaobao.xyz/Article/details/grwvbvtvd.sHtML

Java: list.size();
来源：http://baike.fanxiaobao.xyz/Article/details/gvpuxozpb.sHtML

Go:   len(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfplxfau.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fanxiaobao.xyz/Article/details/gtltsqups.sHtML

C#:   list.Count;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvedetmyx.sHtML

[D07] 切片 / 取子数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gobslfhoe.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wap.fanxiaobao.xyz/Article/details/gpcjkdpko.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcmqjiks.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fanxiaobao.xyz/Article/details/gmgeaxunm.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gpnjixems.sHtML

Java: list.subList(1, 4);
来源：http://3g.fanxiaobao.xyz/Article/details/gyeimsglz.sHtML

Go:   arr[1:4]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabgubftv.sHtML

Ruby: arr[1, 3]
来源：http://wap.fanxiaobao.xyz/Article/details/gagwsvidy.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gtdovkxce.sHtML

[D08] 合并两个数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctgjasag.sHtML

Py:   a + b;  a.extend(b)
来源：http://wap.fanxiaobao.xyz/Article/details/gjxtofldq.sHtML

PHP:  array_merge($a, $b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkyxcssef.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwjwhmsl.sHtML

TS:   [...a, ...b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmndqaepz.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdusfbusj.sHtML

Go:   append(a, b...)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjskvtqc.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.fanxiaobao.xyz/Article/details/gsemlkyoc.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktzspsxo.sHtML

[D09] 排序（升序）
来源：http://blog.fanxiaobao.xyz/Article/details/gacuufbfh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fanxiaobao.xyz/Article/details/gtmyslukx.sHtML

PHP:  sort($arr);
来源：http://blog.fanxiaobao.xyz/Article/details/gwlbfbyyt.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.fanxiaobao.xyz/Article/details/gcaibgjhz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxsqicpy.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fanxiaobao.xyz/Article/details/gprxgyjwu.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/grhbzzbqu.sHtML

Ruby: arr.sort
来源：http://baike.fanxiaobao.xyz/Article/details/gvjngbjyu.sHtML

C#:   list.Sort();
来源：http://blog.fanxiaobao.xyz/Article/details/gpmlumpcy.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://m.share.fanxiaobao.xyz/Article/details/grindsomx.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gmftqrngq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwqujmuu.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://blog.fanxiaobao.xyz/Article/details/gtystqicr.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fanxiaobao.xyz/Article/details/gtumjpkxv.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqrqeeec.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.fanxiaobao.xyz/Article/details/gdgrrdoei.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykqplhnh.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fanxiaobao.xyz/Article/details/gttvpxevh.sHtML

[D11] 反转数组
来源：http://blog.fanxiaobao.xyz/Article/details/gutvosvfu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdfuvndlp.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljvuqvzo.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbbmfpjw.sHtML

TS:   [...arr].reverse();
来源：http://3g.fanxiaobao.xyz/Article/details/gytjrxzau.sHtML

Java: Collections.reverse(list);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwskccovn.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fanxiaobao.xyz/Article/details/gikgjhrmn.sHtML

Ruby: arr.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gnfpnwzsf.sHtML

C#:   list.Reverse();
来源：http://blog.fanxiaobao.xyz/Article/details/gnaaetnpj.sHtML

[D12] 查找元素下标
来源：http://read.share.fanxiaobao.xyz/Article/details/gtutfygtt.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.fanxiaobao.xyz/Article/details/goifzmqnr.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxmrwrid.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgqqnkma.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/geopzpxxe.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginybzmka.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/gjfhlshqi.sHtML

Ruby: arr.index(x)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgxzeqdg.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gewhkrlll.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fanxiaobao.xyz/Article/details/gxqzcblwx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gratrqpni.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqaliwcta.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoscvpip.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fanxiaobao.xyz/Article/details/gpgrcvumt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gjipdtigt.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvdisaux.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoebxupu.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fanxiaobao.xyz/Article/details/gtmsgenwh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.fanxiaobao.xyz/Article/details/gvrkfjnrg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giauwzqpp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gugiyvvuj.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmogqlid.sHtML

TS:   arr.map(x => x * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhntzyua.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gvrhvfoan.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwvgsola.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsdwuueik.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/giexptkrt.sHtML

[D15] 去重
来源：http://baike.fanxiaobao.xyz/Article/details/ghtnomtjj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.fanxiaobao.xyz/Article/details/gycarajhc.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkpbypgv.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtkbgyoi.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fanxiaobao.xyz/Article/details/gzaspcgqh.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.share.fanxiaobao.xyz/Article/details/gipnppfqd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fanxiaobao.xyz/Article/details/guijsozcd.sHtML

Ruby: arr.uniq
来源：http://mobile.fanxiaobao.xyz/Article/details/gggsrdnry.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fanxiaobao.xyz/Article/details/gbqajinaz.sHtML

[D16] 求和与平均值
来源：http://wap.fanxiaobao.xyz/Article/details/gddrvtenp.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwxiigx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fanxiaobao.xyz/Article/details/gyllegvde.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/gnrjahwta.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fanxiaobao.xyz/Article/details/ghozqjhhf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fanxiaobao.xyz/Article/details/giplagnzf.sHtML

Go:   // 手写循环累加
来源：http://www.share.fanxiaobao.xyz/Article/details/ghuombept.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gudsaakvc.sHtML

C#:   list.Sum();  list.Average()
来源：http://wap.fanxiaobao.xyz/Article/details/gutacyiuz.sHtML

[D17] 最大值与最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddintpzr.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/ggchrgqjn.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdccyiwfc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnkrrykgn.sHtML

TS:   Math.max(...arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gbjysbypu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fanxiaobao.xyz/Article/details/gchstaeto.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdctlnrek.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.fanxiaobao.xyz/Article/details/grmeskzze.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfwbhqaj.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fanxiaobao.xyz/Article/details/ggswnnqgh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.fanxiaobao.xyz/Article/details/gwgoaazvw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fanxiaobao.xyz/Article/details/gggepidoq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fanxiaobao.xyz/Article/details/gmrqaqlkq.sHtML

TS:   nested.flat();
来源：http://read.share.fanxiaobao.xyz/Article/details/gvgofapve.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkqubgmk.sHtML

Go:   // 手写双层循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjtsbscx.sHtML

Ruby: nested.flatten
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdivebmoo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnyiutdy.sHtML

[D19] 按字段分组
来源：http://3g.fanxiaobao.xyz/Article/details/gvgwzitig.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvmphelg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fanxiaobao.xyz/Article/details/goqejcpzr.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fanxiaobao.xyz/Article/details/gdbfsiwtn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gkewmzzrc.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsijqabxa.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwdmsnmt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.fanxiaobao.xyz/Article/details/gtkjxtpww.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gztdskflw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxdvlcia.sHtML

Py:   Counter(arr)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnchzfbo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzxvdrwt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.fanxiaobao.xyz/Article/details/gmbthenrm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsdrsxni.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fanxiaobao.xyz/Article/details/grkmnmlzl.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fanxiaobao.xyz/Article/details/gepefxygx.sHtML

Ruby: arr.tally
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydmhmrik.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwwftyxm.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fanxiaobao.xyz/Article/details/geaawjveq.sHtML

Py:   x in arr
来源：http://www.share.fanxiaobao.xyz/Article/details/gbecaihyb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gihpobzly.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/goencpczn.sHtML

TS:   arr.includes(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gbleimrmy.sHtML

Java: list.contains(x)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvkuvoct.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibkfucsc.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfwtvmbz.sHtML

C#:   list.Contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdcvsbrft.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/galjvybuc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fanxiaobao.xyz/Article/details/gimcrlegd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fanxiaobao.xyz/Article/details/ghewkturs.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfbibegz.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/gzebpglec.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fanxiaobao.xyz/Article/details/grfrurtty.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.fanxiaobao.xyz/Article/details/gfjpxqbqx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhcojudl.sHtML

C#:   new List<int>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/graibeiiy.sHtML

[D23] reduce 累积计算
来源：http://baike.fanxiaobao.xyz/Article/details/gsmjwqnhr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gumdfztim.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqpwcmpl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdqwwlju.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gmbgflvdu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fanxiaobao.xyz/Article/details/gsdbmeeid.sHtML

Go:   // 手写循环
来源：http://baike.fanxiaobao.xyz/Article/details/gtdbhvqqr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/gjldipbhh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrhnwutv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gicgmouby.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkofohxis.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fanxiaobao.xyz/Article/details/gilngzzgo.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gudxmbazc.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjlpwrg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpctpmbd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fanxiaobao.xyz/Article/details/gqysxcsqn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmlvrjkw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fanxiaobao.xyz/Article/details/gleylbhyh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fanxiaobao.xyz/Article/details/gxorrhimv.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fanxiaobao.xyz/Article/details/gmfmgrvgf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmqenssk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gdelqdlqb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcpibupy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiypmxrb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fanxiaobao.xyz/Article/details/gtdplmgwi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gomlhsein.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjuzlmfbk.sHtML

[D26] 数组转字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgfnxkuk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fanxiaobao.xyz/Article/details/grcfoofll.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwpxexyz.sHtML

JS:   arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvohmssd.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gltegpncu.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbysdsocb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxsotxqy.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtpiksuol.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfklbqdnv.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glrudetyd.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gklkvnbnt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glneadvsy.sHtML

[E01] 拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdonsiewq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fanxiaobao.xyz/Article/details/gtnqnhbrj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvgozczq.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fanxiaobao.xyz/Article/details/ghnaknruk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtamtsda.sHtML


<!-- 参考信息 -->