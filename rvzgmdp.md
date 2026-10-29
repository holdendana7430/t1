代发 wailian999

TS:   同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gmsnbkcsd.sHtML

Java: 方法内为块级作用域
来源：http://blog.fehbvm.com/Article/details/ghquuwdof.sHtML

Go:   花括号块级作用域
来源：http://m.share.fehbvm.com/Article/details/gzihgxiwd.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.m.share.hesvh.cn/Article/details/gvlhexyok.sHtML

C#:   块级作用域
来源：http://read.share.zdbjq.cn/Article/details/gnckwiklv.sHtML

[C11] 模块导入与导出
来源：http://baike.zdbjq.cn/Article/details/gvncuvcsw.sHtML

Py:   from module import func
来源：http://mobile.hesvh.cn/Article/details/gavhtloce.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://www.share.zdbjq.cn/Article/details/gcbjcztlo.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.m.share.zdbjq.cn/Article/details/gjdxltktx.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mobile.zdbjq.cn/Article/details/gfyjhpjdq.sHtML

Java: import java.util.List;
来源：http://wap.zdbjq.cn/Article/details/gxeqzxekm.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.zdbjq.cn/Article/details/gelqaclzi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://baike.zdbjq.cn/Article/details/gbmvbcfxe.sHtML

C#:   using System.Text;
来源：http://3g.hesvh.cn/Article/details/gjqtabwzm.sHtML

[C12] 立即执行函数 IIFE
来源：http://mobile.hesvh.cn/Article/details/gpmkzbqmd.sHtML

Py:   (lambda: print("run"))()
来源：http://m.share.fehbvm.com/Article/details/gmwemigtp.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.fehbvm.com/Article/details/gvljjexsr.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/gpqgkowgi.sHtML

TS:   (() => { console.log("run"); })();
来源：http://m.share.fehbvm.com/Article/details/gzwebbppp.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://read.share.hesvh.cn/Article/details/gnhjnmvuz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://mobile.fehbvm.com/Article/details/gvvthcvcc.sHtML

Ruby: -> { puts "run" }.call
来源：http://www.m.share.fehbvm.com/Article/details/glmspahwr.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://mobile.fehbvm.com/Article/details/grfnnfyev.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.zdbjq.cn/Article/details/gwloixjhx.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://wap.hesvh.cn/Article/details/gxxfnqlkv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.zdbjq.cn/Article/details/geryoxbuk.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.hesvh.cn/Article/details/gcczimcew.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gvyjiqxty.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gwiorbccp.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/grcpxjxsu.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mobile.fehbvm.com/Article/details/gnakbbadn.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://read.share.zdbjq.cn/Article/details/grwltlwep.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/gqefmkkbw.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.zdbjq.cn/Article/details/gszzmcalh.sHtML

PHP:  // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gztzjxqtl.sHtML

JS:   // 无泛型
来源：http://mobile.hesvh.cn/Article/details/gsrcfyida.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://baike.fehbvm.com/Article/details/gzwbhfuqf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://3g.zdbjq.cn/Article/details/ghulypruf.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.zdbjq.cn/Article/details/gxhazeejh.sHtML

Ruby: # 无泛型
来源：http://blog.fehbvm.com/Article/details/gcvjonrpo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.share.zdbjq.cn/Article/details/gxuxawptn.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/geobpyqje.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://baike.fehbvm.com/Article/details/gvfiuxuhd.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.blog.zdbjq.cn/Article/details/gskzjnrzk.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://blog.hesvh.cn/Article/details/gfuuyspfm.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://baike.zdbjq.cn/Article/details/gkbsbdwmw.sHtML

Java: // 无解构
来源：http://www.share.fehbvm.com/Article/details/gwxwfzeha.sHtML

Go:   // 无解构
来源：http://wap.zdbjq.cn/Article/details/gubxywysb.sHtML

Ruby: a, b = pair
来源：http://wap.zdbjq.cn/Article/details/gaxuhohle.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.zdbjq.cn/Article/details/gkrthtixz.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gxuwknacj.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/giqitmrun.sHtML

PHP:  // 无重载
来源：http://www.blog.zdbjq.cn/Article/details/gxmuwdqwl.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.share.hesvh.cn/Article/details/gsndechjt.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.m.share.hesvh.cn/Article/details/gxloxdkwb.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gvilwljtl.sHtML

Go:   // 无重载：用不同函数名
来源：http://mobile.zdbjq.cn/Article/details/gcdugcwfi.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.hesvh.cn/Article/details/gigymwbak.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.share.hesvh.cn/Article/details/gzhomxhux.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gpzvscpfr.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.hesvh.cn/Article/details/gxedzvbax.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkrtxlukb.sHtML

[D01] 创建数组 / 列表
来源：http://www.share.zdbjq.cn/Article/details/gsatwvrnz.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://3g.zdbjq.cn/Article/details/gawehkbix.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/gjuffndwx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.share.hesvh.cn/Article/details/gcmxvywnn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://3g.fehbvm.com/Article/details/gtujpfqpv.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.fehbvm.com/Article/details/gmoaxhmoe.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://blog.fehbvm.com/Article/details/gqlmmolza.sHtML

Ruby: arr = [1, 2, 3]
来源：http://m.share.zdbjq.cn/Article/details/gwpwcnpwf.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://mobile.hesvh.cn/Article/details/gveyrwhce.sHtML

[D02] 追加元素到末尾
来源：http://3g.hesvh.cn/Article/details/gqbrsovdz.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.m.share.fehbvm.com/Article/details/gozyqcnfc.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gzoahedyi.sHtML

JS:   arr.push(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gktfdoajs.sHtML

TS:   arr.push(4);
来源：http://baike.fehbvm.com/Article/details/gwmwpdksc.sHtML

Java: list.add(4);
来源：http://wap.zdbjq.cn/Article/details/goddfjwsq.sHtML

Go:   arr = append(arr, 4)
来源：http://baike.zdbjq.cn/Article/details/gjwuxvekp.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://wap.zdbjq.cn/Article/details/gikkpyhdb.sHtML

C#:   list.Add(4);
来源：http://blog.hesvh.cn/Article/details/gchhusdzu.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.fehbvm.com/Article/details/gxvmsvdym.sHtML

Py:   arr.insert(0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gmjevhjbl.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://wap.zdbjq.cn/Article/details/gdamsegmn.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://blog.fehbvm.com/Article/details/gfwumpvbf.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://wap.fehbvm.com/Article/details/gzjmjcucm.sHtML

Java: list.add(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gppufvunw.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://mobile.zdbjq.cn/Article/details/gwgjgjhwu.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.m.share.fehbvm.com/Article/details/gdezokigh.sHtML

C#:   list.Insert(0, 0);
来源：http://wap.zdbjq.cn/Article/details/grrgwbbyu.sHtML

[D04] 删除元素
来源：http://mobile.fehbvm.com/Article/details/gqetlyfmm.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://mobile.fehbvm.com/Article/details/giaplmjvu.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdmthwrii.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://m.share.zdbjq.cn/Article/details/gqtnyokgi.sHtML

TS:   arr.splice(0, 1);
来源：http://m.share.fehbvm.com/Article/details/gsyaikdzc.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://m.share.fehbvm.com/Article/details/gospftdfb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://m.share.zdbjq.cn/Article/details/gghwsawyh.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://m.share.fehbvm.com/Article/details/gooooojqy.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://wap.hesvh.cn/Article/details/gmonqthxd.sHtML

[D05] 访问与修改元素
来源：http://mobile.zdbjq.cn/Article/details/gdrwleimg.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://read.share.hesvh.cn/Article/details/gkgnrmpwe.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gcwyknpmi.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://baike.fehbvm.com/Article/details/gagbmzbyf.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://3g.zdbjq.cn/Article/details/gsondalna.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.fehbvm.com/Article/details/gzxanucly.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.zdbjq.cn/Article/details/givxjsahz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/gfxymkiqr.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://wap.fehbvm.com/Article/details/gfkgpnigm.sHtML

[D06] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gjwfxowen.sHtML

Py:   len(arr)
来源：http://blog.hesvh.cn/Article/details/gorawmvyi.sHtML

PHP:  count($arr);
来源：http://blog.fehbvm.com/Article/details/glydiiwsa.sHtML

JS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gprpvonny.sHtML

TS:   arr.length
来源：http://www.blog.fehbvm.com/Article/details/gprlsvehx.sHtML

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gvijsoaff.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqgbzgkl.sHtML

Ruby: arr.length; arr.size
来源：http://read.share.fehbvm.com/Article/details/gmtcbiuob.sHtML

C#:   list.Count;
来源：http://www.m.share.hesvh.cn/Article/details/gusjviwyp.sHtML

[D07] 切片 / 取子数组
来源：http://www.m.share.zdbjq.cn/Article/details/glqtzvdvj.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://blog.hesvh.cn/Article/details/gxzkuqayz.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://read.share.fehbvm.com/Article/details/gzentsavf.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.zdbjq.cn/Article/details/gozrfpjzc.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.zdbjq.cn/Article/details/gqgqdyrxl.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.hesvh.cn/Article/details/gsljvnaaf.sHtML

Go:   arr[1:4]
来源：http://mobile.fehbvm.com/Article/details/gdcgubrpt.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gpckvrvhz.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwlupdmhu.sHtML

[D08] 合并两个数组
来源：http://m.share.hesvh.cn/Article/details/gslumkovn.sHtML

Py:   a + b;  a.extend(b)
来源：http://m.share.fehbvm.com/Article/details/geaukigwn.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.hesvh.cn/Article/details/gdzofrpsi.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/gvvdgrhwo.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.hesvh.cn/Article/details/ghozwrrxf.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.m.share.fehbvm.com/Article/details/glwfvahmu.sHtML

Go:   append(a, b...)
来源：http://www.blog.fehbvm.com/Article/details/gnhxszhnm.sHtML

Ruby: a + b;  a.concat(b)
来源：http://blog.hesvh.cn/Article/details/gtrgxyshu.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/ggkkoxzci.sHtML

[D09] 排序（升序）
来源：http://www.share.zdbjq.cn/Article/details/grwotlone.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gffqwliet.sHtML

PHP:  sort($arr);
来源：http://m.share.hesvh.cn/Article/details/gwtsdbwmk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.zdbjq.cn/Article/details/ghlesynan.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://wap.fehbvm.com/Article/details/gycayldgb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.m.share.hesvh.cn/Article/details/gfsivjyyi.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/gpkvapnbz.sHtML

Ruby: arr.sort
来源：http://www.share.fehbvm.com/Article/details/grbijwypa.sHtML

C#:   list.Sort();
来源：http://3g.hesvh.cn/Article/details/glloffveq.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://blog.fehbvm.com/Article/details/gbldxerke.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.m.share.hesvh.cn/Article/details/gsygizluc.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gpbjqbtag.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gyflazdnt.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/gmocjqseq.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.zdbjq.cn/Article/details/gnvhbhyub.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://read.share.zdbjq.cn/Article/details/gqcemdoju.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.hesvh.cn/Article/details/ghjmfwfle.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gagogitub.sHtML

[D11] 反转数组
来源：http://www.share.zdbjq.cn/Article/details/gntagzqsy.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.fehbvm.com/Article/details/gtzwraghe.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gmszyblco.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://baike.zdbjq.cn/Article/details/gnuvnucin.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gtgfmjfur.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gizogkxzz.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.hesvh.cn/Article/details/gbvcgmmur.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gsvmhsbfz.sHtML

C#:   list.Reverse();
来源：http://www.m.share.fehbvm.com/Article/details/gdqoarqfc.sHtML

[D12] 查找元素下标
来源：http://blog.hesvh.cn/Article/details/grxwpzzpz.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.hesvh.cn/Article/details/gmjqcpdgx.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://baike.zdbjq.cn/Article/details/gztqnorrd.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.zdbjq.cn/Article/details/gbdszpfso.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqlxzypsj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gtdcbyyqu.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghnhxszvo.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gwnrmhxyt.sHtML

C#:   list.IndexOf(x);
来源：http://3g.hesvh.cn/Article/details/gupnxcgtt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.zdbjq.cn/Article/details/ghzooxqkc.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gcwaaanlm.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/gdzhitkbm.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guagqvrfq.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.fehbvm.com/Article/details/gmaznvbng.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gimljwozf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://3g.zdbjq.cn/Article/details/gpntmetyy.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gemwuwwic.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gbtymlpey.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gtmreqoeh.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.hesvh.cn/Article/details/gwcrpgdup.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.fehbvm.com/Article/details/gwezporkg.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gbkdfmxcm.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/gfgprbgyv.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.hesvh.cn/Article/details/golkpzpau.sHtML

Go:   // 手写循环
来源：http://www.share.zdbjq.cn/Article/details/gnjorqxwg.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://mobile.zdbjq.cn/Article/details/glninxxhm.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.fehbvm.com/Article/details/goekiohgm.sHtML

[D15] 去重
来源：http://mobile.zdbjq.cn/Article/details/gfukkajlf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.fehbvm.com/Article/details/guqfsvlqr.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/gajbuxbtm.sHtML

JS:   [...new Set(arr)]
来源：http://www.m.share.zdbjq.cn/Article/details/gejmzkpxs.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/ggihpooes.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gqshynpsv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/guwoelimo.sHtML

Ruby: arr.uniq
来源：http://read.share.fehbvm.com/Article/details/ganepgxds.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.fehbvm.com/Article/details/ggxkgrqnx.sHtML

[D16] 求和与平均值
来源：http://www.share.zdbjq.cn/Article/details/gotdeeomk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.zdbjq.cn/Article/details/goepgjqgb.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/giswgwspd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gudfylaew.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.fehbvm.com/Article/details/grfzbaaxd.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/grvvgamvz.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/ghubipqlb.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.zdbjq.cn/Article/details/gfqbmcqxh.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.zdbjq.cn/Article/details/gjinmuqzi.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/gguzhqibd.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gynjfoumt.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gqrrqpoar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/goamdmwwy.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/gldgrawua.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.hesvh.cn/Article/details/gdptwzdon.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/goqjsvttk.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.fehbvm.com/Article/details/ggookucwu.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gnlkwqbfc.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gpyhuyxba.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gtcpmifme.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gxsbyccss.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.zdbjq.cn/Article/details/gcexiuova.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/geixolags.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.hesvh.cn/Article/details/gghwfibyu.sHtML

Go:   // 手写双层循环
来源：http://read.share.fehbvm.com/Article/details/gjaxmmudw.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gpcvnbour.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gtncokqkd.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gloqsfotd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gfkiudgpa.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gerdzklcm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/glxfkbkxp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gstwcpqii.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fehbvm.com/Article/details/gbkfeqnes.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gzslndtzh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.fehbvm.com/Article/details/grupaygwz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gggbcoecd.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gglxfchhs.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/gjzncnarw.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/ghqzsbgzm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gfiajwmte.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gaizlgfmy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gwqyidwph.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gaggaymgn.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/ghlnzxyyz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.hesvh.cn/Article/details/gxmwpesxk.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fehbvm.com/Article/details/gciheptzb.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/gsvveincq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gmierkpqc.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gfmtmvrwf.sHtML

TS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gaoanzqpv.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/ghpjnftro.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.hesvh.cn/Article/details/gvjtjywrp.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gocwlztmp.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/grwmfnrln.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.fehbvm.com/Article/details/gotoisjkq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/grztdenrc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gaxlbalao.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/giadnqqgn.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gxarngfst.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/guvqexmvm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gczyaccld.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/goojitkzh.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gckbzvish.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/ghjjoifua.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.zdbjq.cn/Article/details/gebnvmvlo.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/gzeckjxcb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gcmblqmjd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdrpfgldi.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gqlxvvndl.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzqfjnh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gkbupkwup.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gchwyrbym.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.hesvh.cn/Article/details/ggokklihk.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gvqkievuq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/ghjtpymhr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/ghtdihwlf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gyytpgtzm.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.zdbjq.cn/Article/details/geahxvtzv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gpteytzct.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gwjwqoxiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gitlfujbh.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/gfiwajuim.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gfpepeeqv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdvipyarm.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.hesvh.cn/Article/details/guobgmtqg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gxxqdbjoq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gimywezwn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.hesvh.cn/Article/details/gkfbqkpaj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gkxllgkcv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/gtrecedfz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gnoqncaqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ghgahtlxt.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.fehbvm.com/Article/details/grcipmwbh.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gqfqjnqua.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grmtocosb.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gshoexokq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.fehbvm.com/Article/details/gnvkesman.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghqvkpkgx.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpfsznwyo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grwvogvnb.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gtyborzya.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gofjmstrm.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/ggbkxifsd.sHtML


<!-- 参考信息 -->