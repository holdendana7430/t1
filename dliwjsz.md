代发 wailian999

C#:   块级作用域
来源：http://www.share.zdbjq.cn/Article/details/ggwqmxoex.sHtML

[C11] 模块导入与导出
来源：http://www.m.share.zdbjq.cn/Article/details/ginybeouq.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/guubfbowr.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://blog.fehbvm.com/Article/details/gjwuamcut.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://baike.hesvh.cn/Article/details/gzyofgszn.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/gfebqoqna.sHtML

Java: import java.util.List;
来源：http://blog.zdbjq.cn/Article/details/gdixuhpmw.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://3g.zdbjq.cn/Article/details/gujpmbwhz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.hesvh.cn/Article/details/grxozycnk.sHtML

C#:   using System.Text;
来源：http://wap.hesvh.cn/Article/details/godqtmhpc.sHtML

[C12] 立即执行函数 IIFE
来源：http://wap.zdbjq.cn/Article/details/gyrrebbot.sHtML

Py:   (lambda: print("run"))()
来源：http://wap.hesvh.cn/Article/details/gvexytxem.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.share.zdbjq.cn/Article/details/gkycjvdgo.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.m.share.hesvh.cn/Article/details/gcgoepoan.sHtML

TS:   (() => { console.log("run"); })();
来源：http://read.share.zdbjq.cn/Article/details/gwcwnpcgb.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.blog.zdbjq.cn/Article/details/giclemrbq.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gcrbzuzvy.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.blog.hesvh.cn/Article/details/gxftchutf.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gafqrgkzj.sHtML

[C13] 类型声明 / 类型注解
来源：http://mobile.fehbvm.com/Article/details/gpqrdudxe.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://read.share.fehbvm.com/Article/details/ghgviwkmr.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/goqnelhvm.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wap.fehbvm.com/Article/details/gayudsodk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/gejniyouq.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/ggoffursz.sHtML

Go:   func add(a, b int) int
来源：http://3g.hesvh.cn/Article/details/ghjyzkkdh.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://m.share.fehbvm.com/Article/details/gqykwrqyj.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://mobile.fehbvm.com/Article/details/gtwoionag.sHtML

[C14] 泛型函数
来源：http://m.share.fehbvm.com/Article/details/getfxuwuj.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gaguepxbj.sHtML

PHP:  // 无泛型
来源：http://www.share.fehbvm.com/Article/details/gqcecjzfw.sHtML

JS:   // 无泛型
来源：http://3g.hesvh.cn/Article/details/gpfmnyagk.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gbusldhqc.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://read.share.zdbjq.cn/Article/details/gwjgzgovc.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://m.share.hesvh.cn/Article/details/gkpshwpof.sHtML

Ruby: # 无泛型
来源：http://3g.zdbjq.cn/Article/details/gxltxcwoy.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://blog.hesvh.cn/Article/details/gphyvzqtf.sHtML

[C15] 解构 / 展开参数
来源：http://mobile.fehbvm.com/Article/details/gsyuwebgi.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://read.share.zdbjq.cn/Article/details/grymvwxky.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.hesvh.cn/Article/details/gpubcqouy.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.share.fehbvm.com/Article/details/gooacfmhi.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://3g.zdbjq.cn/Article/details/gcmuikumr.sHtML

Java: // 无解构
来源：http://read.share.fehbvm.com/Article/details/goaxeyxqa.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gcflgopbb.sHtML

Ruby: a, b = pair
来源：http://baike.hesvh.cn/Article/details/gtjsvaqig.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.fehbvm.com/Article/details/gwbcecaml.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gfmlnfbkl.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.fehbvm.com/Article/details/gvxjinacg.sHtML

PHP:  // 无重载
来源：http://www.blog.hesvh.cn/Article/details/gnsibkyor.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://read.share.zdbjq.cn/Article/details/glsqdbjfv.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://blog.zdbjq.cn/Article/details/gfnfdsqkc.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gisnoqmax.sHtML

Go:   // 无重载：用不同函数名
来源：http://3g.zdbjq.cn/Article/details/guddwtinv.sHtML

Ruby: # 无重载：靠动态参数
来源：http://www.blog.hesvh.cn/Article/details/gypfjbqwq.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://wap.hesvh.cn/Article/details/gvnffgrad.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtnifphwg.sHtML

D. 数组 / 列表 / 集合
来源：http://blog.hesvh.cn/Article/details/gmojsebne.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gprhxvfih.sHtML

[D01] 创建数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gswdqcwro.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.hesvh.cn/Article/details/gnkvrzahf.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxtjjpbvj.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.blog.hesvh.cn/Article/details/gxxskfdma.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gzvlgopnp.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://3g.hesvh.cn/Article/details/gjwjvevlb.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.hesvh.cn/Article/details/gjpfwiqek.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.hesvh.cn/Article/details/guqyvzeoo.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.zdbjq.cn/Article/details/ghgbvujsw.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gkuwlrhlh.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.blog.fehbvm.com/Article/details/gthlwlspe.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://read.share.zdbjq.cn/Article/details/gillifnqx.sHtML

JS:   arr.push(4);
来源：http://blog.zdbjq.cn/Article/details/galrekkkf.sHtML

TS:   arr.push(4);
来源：http://mobile.hesvh.cn/Article/details/ghxatlcxq.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/glmnplxtt.sHtML

Go:   arr = append(arr, 4)
来源：http://mobile.hesvh.cn/Article/details/gaozhokyc.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwlizawpb.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gmdiodkjp.sHtML

[D03] 在指定位置插入元素
来源：http://3g.hesvh.cn/Article/details/glmqkcvxl.sHtML

Py:   arr.insert(0, 0)
来源：http://mobile.hesvh.cn/Article/details/guowmpjwj.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://blog.zdbjq.cn/Article/details/gsygvmbzv.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://3g.hesvh.cn/Article/details/gjtzbzmvs.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://read.share.fehbvm.com/Article/details/govvpfbah.sHtML

Java: list.add(0, 0);
来源：http://mobile.hesvh.cn/Article/details/gzbthiujj.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://m.share.hesvh.cn/Article/details/gakfrzdns.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://m.share.zdbjq.cn/Article/details/gdzxtwcby.sHtML

C#:   list.Insert(0, 0);
来源：http://www.blog.zdbjq.cn/Article/details/gjrtopjuq.sHtML

[D04] 删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gmjzeiabe.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://read.share.hesvh.cn/Article/details/gleswkyqv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://baike.zdbjq.cn/Article/details/giqfsvwae.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.fehbvm.com/Article/details/geeiagoja.sHtML

TS:   arr.splice(0, 1);
来源：http://www.m.share.hesvh.cn/Article/details/gnxttmgtl.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://blog.zdbjq.cn/Article/details/gocitemmh.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://baike.hesvh.cn/Article/details/gvukzekmu.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://wap.hesvh.cn/Article/details/ggudqqeia.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.share.zdbjq.cn/Article/details/gbbnkapwf.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gabyyjowe.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.share.fehbvm.com/Article/details/gkscwkxmx.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://read.share.zdbjq.cn/Article/details/gqbabjacl.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gmjgpkwua.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://baike.fehbvm.com/Article/details/glzblijvo.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://www.m.share.hesvh.cn/Article/details/gmgllieos.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/gfdyhxxfo.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/gtgvubsqs.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gzjairvzk.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/gbqoapmeq.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gykdokzva.sHtML

PHP:  count($arr);
来源：http://3g.hesvh.cn/Article/details/gwtwkuqnp.sHtML

JS:   arr.length
来源：http://m.share.hesvh.cn/Article/details/gaasntaea.sHtML

TS:   arr.length
来源：http://3g.hesvh.cn/Article/details/glbfsduks.sHtML

Java: list.size();
来源：http://baike.fehbvm.com/Article/details/gvmmngzrs.sHtML

Go:   len(arr)
来源：http://read.share.fehbvm.com/Article/details/gijwmzqca.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gqemldoim.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/ggwisbnzy.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gsjhmxheg.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.m.share.fehbvm.com/Article/details/gksfwudkm.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gqwwmvavb.sHtML

JS:   arr.slice(1, 4);
来源：http://wap.zdbjq.cn/Article/details/gtrslojwn.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.hesvh.cn/Article/details/gqxbzmrvm.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gyimkqbwz.sHtML

Go:   arr[1:4]
来源：http://www.blog.hesvh.cn/Article/details/gvzxstlks.sHtML

Ruby: arr[1, 3]
来源：http://wap.zdbjq.cn/Article/details/gchmkttnx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gkksmligl.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gifymgahh.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.zdbjq.cn/Article/details/gdsdmzmcf.sHtML

PHP:  array_merge($a, $b);
来源：http://wap.zdbjq.cn/Article/details/gemmnsmor.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://www.m.share.fehbvm.com/Article/details/gaqnucxba.sHtML

TS:   [...a, ...b];
来源：http://blog.zdbjq.cn/Article/details/glvweqtyk.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/gljtaoceg.sHtML

Go:   append(a, b...)
来源：http://baike.zdbjq.cn/Article/details/gkqvaqfdt.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/gageqjglj.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gmeepzaul.sHtML

[D09] 排序（升序）
来源：http://www.blog.zdbjq.cn/Article/details/gfrvnjqhi.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gducgmmoz.sHtML

PHP:  sort($arr);
来源：http://baike.zdbjq.cn/Article/details/gynqetqpb.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://blog.fehbvm.com/Article/details/gihjfkqqr.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.zdbjq.cn/Article/details/gfifbuidk.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://read.share.fehbvm.com/Article/details/gkkwxutdp.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkopqryhu.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/ggcxradbt.sHtML

C#:   list.Sort();
来源：http://www.m.share.hesvh.cn/Article/details/glcootrkr.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gvdvojhal.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gblmjccsq.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/ggoqnspdi.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gthqwrbxf.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gmkgeqvfe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.fehbvm.com/Article/details/gxolznvwf.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gdbhrznzj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/gtuhcjite.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.fehbvm.com/Article/details/gkixzwwzq.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gfzvjqoqp.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.fehbvm.com/Article/details/gqulegqjv.sHtML

PHP:  array_reverse($arr);
来源：http://wap.fehbvm.com/Article/details/gvapurjcd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.fehbvm.com/Article/details/gckpmrqbq.sHtML

TS:   [...arr].reverse();
来源：http://baike.fehbvm.com/Article/details/gmvolqacs.sHtML

Java: Collections.reverse(list);
来源：http://3g.zdbjq.cn/Article/details/gqssoecyl.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gticyqgcz.sHtML

Ruby: arr.reverse
来源：http://mobile.fehbvm.com/Article/details/gssxdbrud.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/gyxdtkbnl.sHtML

[D12] 查找元素下标
来源：http://read.share.zdbjq.cn/Article/details/giqtkslpp.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gscqcggry.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gvhzhyxvi.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.hesvh.cn/Article/details/gedfmstdl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gbnnikglb.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gcuhejpnn.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gwjxduyoy.sHtML

Ruby: arr.index(x)
来源：http://baike.fehbvm.com/Article/details/gzotofuwd.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.hesvh.cn/Article/details/gljtwsbhe.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.zdbjq.cn/Article/details/genziawfo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gpekhspjk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gbyifjmje.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.hesvh.cn/Article/details/ghhwqsikm.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gmgglrmmx.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gpydfeskv.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.hesvh.cn/Article/details/glrtcknjt.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.zdbjq.cn/Article/details/gpmbkuewz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gekhwtprc.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gedmwszlf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.hesvh.cn/Article/details/geyrigssy.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gjlthahxi.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gpvjhctst.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gmutsvfsi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.fehbvm.com/Article/details/ghjwcusyt.sHtML

Go:   // 手写循环
来源：http://read.share.zdbjq.cn/Article/details/gzwzhrvnk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gzsacugwd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gkehsnnpq.sHtML

[D15] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gnhpteudj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gitwoidrc.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/glhqgbrcn.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gwvtaegqj.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/giymmsvmq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gvyltbfjd.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gryimbsmu.sHtML

Ruby: arr.uniq
来源：http://3g.zdbjq.cn/Article/details/gfmupccdy.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.hesvh.cn/Article/details/gkrgdiypf.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gembwvuba.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.zdbjq.cn/Article/details/grttjkjre.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gijgenozo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.hesvh.cn/Article/details/gdvuyjiag.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/gchdiznwz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gocrjsmvb.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gdkhupngn.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggjwtnczm.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gxszmqpto.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gvdvgilwe.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/glqjsvkvy.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gcajgzpfw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.hesvh.cn/Article/details/glvqfmipc.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.fehbvm.com/Article/details/gmqsaoxzj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/grjyjybyj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gmyabyqta.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gbxtdyavy.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/guyvhmhza.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/glbukdspk.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/ggbsvlpxv.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gxtycybmi.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gijqziclj.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gzhgcjvdq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/ginohdgtu.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gerlsgujn.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gfugefozr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gvpcrlvcq.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gqyvzismi.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gpnbfcgmc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gwqxmpxzw.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fehbvm.com/Article/details/gyfpitaiq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/ginsvcjdp.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/govnpjldc.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.zdbjq.cn/Article/details/gikzoomde.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gzgorhlcs.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gkyyqfziu.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gplxdzuqj.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/ggvinmarg.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gfbhsdvsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gczdigxcn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gmqowohwi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/givogbsge.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/glijhkzdf.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/groqgviuj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gviahyjyw.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gsydtgcfn.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gbqvbaydv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gynhdbjtd.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gbzbbrgow.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/gbqiwdkvk.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/glhwbvkzl.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gncngwbht.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gytbtewcy.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gckerehcx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gsvdoatrd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/gxykeqoxw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gfiefsesi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fehbvm.com/Article/details/gxxepohmj.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gbrbanlaj.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gkpsfxswb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gdasuzawo.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/gnwcdblai.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/giyqfryuj.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gvrvywtjl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gtuqgyyhe.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gsmjgzmir.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gldjnldzn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gzdnaokcv.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gceviolon.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gasjvjfua.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gfbpetinj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/guujkzedo.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gnywbkjfs.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gnlyqllhh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.hesvh.cn/Article/details/ggcsxryeh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.zdbjq.cn/Article/details/godhosquk.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gvpiwevyv.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gmymdztiv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/glosdhlkv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gbsicgtux.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gdhjscxah.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gihecserk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.hesvh.cn/Article/details/gxophjboo.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gnwdwfcbh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtwfwhxie.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/ghomycwml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.fehbvm.com/Article/details/gzjcinyyo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gvgqthzxp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gquiiidej.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gdaebpnrs.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gzkubvzza.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gkefxgjqq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gsiulnrkz.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghktmbqoe.sHtML

TS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gbggnvara.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvqbsubma.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gzzptlwzt.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gfohuirqq.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gvgiambtz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdvvzcphc.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gsvhlpsxg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsmxpoesv.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gqgmvilhs.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gvkoszgdp.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/galmkhtkh.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.hesvh.cn/Article/details/gqawfoded.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/goqyrwfbe.sHtML


<!-- 参考信息 -->