代发 wailian999

TS:   同 JS
来源：http://www.share.fehbvm.com/Article/details/gjqpbbvzm.sHtML

Java: 方法内为块级作用域
来源：http://mobile.hesvh.cn/Article/details/gpgsgghan.sHtML

Go:   花括号块级作用域
来源：http://www.share.zdbjq.cn/Article/details/gnmruilml.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://blog.fehbvm.com/Article/details/gxamrpfvt.sHtML

C#:   块级作用域
来源：http://mobile.fehbvm.com/Article/details/gsmldfwms.sHtML

[C11] 模块导入与导出
来源：http://read.share.fehbvm.com/Article/details/gnzagwpxv.sHtML

Py:   from module import func
来源：http://3g.hesvh.cn/Article/details/ghiyfplxx.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://3g.hesvh.cn/Article/details/gqaszpppk.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gdnxspczu.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://3g.hesvh.cn/Article/details/gfyrmrfyf.sHtML

Java: import java.util.List;
来源：http://read.share.fehbvm.com/Article/details/gsknztzep.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://m.share.fehbvm.com/Article/details/gmnverrpz.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.zdbjq.cn/Article/details/gcdwzaatd.sHtML

C#:   using System.Text;
来源：http://www.share.hesvh.cn/Article/details/gcuqtmygy.sHtML

[C12] 立即执行函数 IIFE
来源：http://blog.zdbjq.cn/Article/details/gfhszckpy.sHtML

Py:   (lambda: print("run"))()
来源：http://blog.zdbjq.cn/Article/details/gqoabkocb.sHtML

PHP:  (function () { echo "run"; })();
来源：http://baike.zdbjq.cn/Article/details/gvtnrtzgt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://www.blog.fehbvm.com/Article/details/gqcdcorxw.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.fehbvm.com/Article/details/gkjxqddyk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://wap.fehbvm.com/Article/details/gpsihbrdz.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://read.share.fehbvm.com/Article/details/gjountrrv.sHtML

Ruby: -> { puts "run" }.call
来源：http://blog.fehbvm.com/Article/details/gowwiqxcn.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.share.zdbjq.cn/Article/details/gyuzmsodr.sHtML

[C13] 类型声明 / 类型注解
来源：http://read.share.hesvh.cn/Article/details/gcxjszyrt.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://baike.fehbvm.com/Article/details/gdhxsdkub.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gdqbanhkt.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://baike.zdbjq.cn/Article/details/gbbamodum.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.zdbjq.cn/Article/details/gventlgcl.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/goolkityp.sHtML

Go:   func add(a, b int) int
来源：http://3g.zdbjq.cn/Article/details/gddjvtxzn.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.fehbvm.com/Article/details/gpueimham.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.m.share.fehbvm.com/Article/details/gbewqqjer.sHtML

[C14] 泛型函数
来源：http://blog.zdbjq.cn/Article/details/glbfftnhd.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://blog.hesvh.cn/Article/details/gwyvupdbm.sHtML

PHP:  // 无泛型
来源：http://mobile.fehbvm.com/Article/details/gaifdqplh.sHtML

JS:   // 无泛型
来源：http://m.share.hesvh.cn/Article/details/ghptldmej.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://blog.hesvh.cn/Article/details/gstdgbugi.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.share.hesvh.cn/Article/details/gdrzhsagt.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://blog.zdbjq.cn/Article/details/gzbtxuxqj.sHtML

Ruby: # 无泛型
来源：http://read.share.zdbjq.cn/Article/details/ggynnanjo.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.m.share.fehbvm.com/Article/details/gezfxxlid.sHtML

[C15] 解构 / 展开参数
来源：http://wap.fehbvm.com/Article/details/gjakfxlhm.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxaadvj.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.share.hesvh.cn/Article/details/gmnvmupem.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://3g.zdbjq.cn/Article/details/gajpfxdgp.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.blog.fehbvm.com/Article/details/gzibstetz.sHtML

Java: // 无解构
来源：http://blog.fehbvm.com/Article/details/gaskdonvg.sHtML

Go:   // 无解构
来源：http://www.blog.hesvh.cn/Article/details/gmbmqxyrq.sHtML

Ruby: a, b = pair
来源：http://www.share.hesvh.cn/Article/details/ghewktgym.sHtML

C#:   var (a, b) = pair;
来源：http://www.blog.hesvh.cn/Article/details/guftbjoke.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/ggyqerioi.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mobile.fehbvm.com/Article/details/gpccrsbwq.sHtML

PHP:  // 无重载
来源：http://www.share.zdbjq.cn/Article/details/gtlhdfpov.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.m.share.zdbjq.cn/Article/details/goqruwpdf.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://mobile.hesvh.cn/Article/details/glwbrxyvu.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://baike.hesvh.cn/Article/details/gweazgvmu.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.fehbvm.com/Article/details/gbzjzgbiq.sHtML

Ruby: # 无重载：靠动态参数
来源：http://m.share.fehbvm.com/Article/details/ggikvdefg.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://m.share.hesvh.cn/Article/details/grvkjtpqz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gmstfnyai.sHtML

D. 数组 / 列表 / 集合
来源：http://www.share.zdbjq.cn/Article/details/gtuzjcsgi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gycdrwszt.sHtML

[D01] 创建数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/gklkkqerf.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.fehbvm.com/Article/details/gkrhrlkcs.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.share.zdbjq.cn/Article/details/guashgnni.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.m.share.hesvh.cn/Article/details/gtknnjnkn.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.blog.hesvh.cn/Article/details/ghwpqiwxw.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.m.share.fehbvm.com/Article/details/gpdjcisvq.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://baike.zdbjq.cn/Article/details/gotdgkvmk.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.blog.zdbjq.cn/Article/details/gyihnqbae.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://blog.hesvh.cn/Article/details/gtvzrdugf.sHtML

[D02] 追加元素到末尾
来源：http://baike.zdbjq.cn/Article/details/gpjzwryut.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://m.share.zdbjq.cn/Article/details/goppeuxxs.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.hesvh.cn/Article/details/gdoaqfmpn.sHtML

JS:   arr.push(4);
来源：http://www.blog.zdbjq.cn/Article/details/gdluftbtw.sHtML

TS:   arr.push(4);
来源：http://baike.zdbjq.cn/Article/details/gflkjvdcw.sHtML

Java: list.add(4);
来源：http://mobile.zdbjq.cn/Article/details/gxrgctbvj.sHtML

Go:   arr = append(arr, 4)
来源：http://wap.zdbjq.cn/Article/details/gtsjbapgw.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://m.share.zdbjq.cn/Article/details/ghnibrzcx.sHtML

C#:   list.Add(4);
来源：http://blog.zdbjq.cn/Article/details/gjpttlouy.sHtML

[D03] 在指定位置插入元素
来源：http://3g.zdbjq.cn/Article/details/gdujxktop.sHtML

Py:   arr.insert(0, 0)
来源：http://3g.hesvh.cn/Article/details/gtirpihnv.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.blog.zdbjq.cn/Article/details/gwcagjldj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://mobile.fehbvm.com/Article/details/glcfqfvbo.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://mobile.fehbvm.com/Article/details/gpivnaxes.sHtML

Java: list.add(0, 0);
来源：http://blog.hesvh.cn/Article/details/gjukeumhu.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.blog.hesvh.cn/Article/details/guvirztbs.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://wap.fehbvm.com/Article/details/gcmfwxrrj.sHtML

C#:   list.Insert(0, 0);
来源：http://read.share.hesvh.cn/Article/details/gryeayqsn.sHtML

[D04] 删除元素
来源：http://mobile.hesvh.cn/Article/details/gdyxkoaaz.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://m.share.zdbjq.cn/Article/details/gpwuufeuv.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://m.share.fehbvm.com/Article/details/gflzxlxal.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.share.hesvh.cn/Article/details/gpndhhuvh.sHtML

TS:   arr.splice(0, 1);
来源：http://www.share.hesvh.cn/Article/details/gbhapvwxu.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gvizzmbyb.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://read.share.hesvh.cn/Article/details/glptfvxxg.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://baike.fehbvm.com/Article/details/gsdpzkybd.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://blog.hesvh.cn/Article/details/gqqpthrya.sHtML

[D05] 访问与修改元素
来源：http://blog.hesvh.cn/Article/details/gmqsgabgy.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.fehbvm.com/Article/details/guoiwevmz.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.m.share.zdbjq.cn/Article/details/gpucutqqy.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/guqdvnqpy.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://read.share.zdbjq.cn/Article/details/ghyfsicmb.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://wap.hesvh.cn/Article/details/gwibwtiba.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://m.share.hesvh.cn/Article/details/gnribopoy.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://wap.zdbjq.cn/Article/details/gfveywlzy.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.m.share.hesvh.cn/Article/details/glcwdpdoy.sHtML

[D06] 数组长度
来源：http://3g.fehbvm.com/Article/details/geuqdvwzx.sHtML

Py:   len(arr)
来源：http://m.share.fehbvm.com/Article/details/gwzdetslb.sHtML

PHP:  count($arr);
来源：http://www.blog.hesvh.cn/Article/details/gxpberwsc.sHtML

JS:   arr.length
来源：http://www.blog.hesvh.cn/Article/details/ggmwocmma.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/gnohhopjk.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ginxcmwty.sHtML

Go:   len(arr)
来源：http://blog.fehbvm.com/Article/details/grifvyphx.sHtML

Ruby: arr.length; arr.size
来源：http://www.share.fehbvm.com/Article/details/gikuyusiz.sHtML

C#:   list.Count;
来源：http://wap.fehbvm.com/Article/details/ghofdbrdr.sHtML

[D07] 切片 / 取子数组
来源：http://blog.zdbjq.cn/Article/details/gbwuydpnr.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.share.zdbjq.cn/Article/details/gmqizpmnq.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/gqbmmosls.sHtML

JS:   arr.slice(1, 4);
来源：http://3g.zdbjq.cn/Article/details/gfltfpxed.sHtML

TS:   arr.slice(1, 4);
来源：http://blog.hesvh.cn/Article/details/gtttifaea.sHtML

Java: list.subList(1, 4);
来源：http://3g.fehbvm.com/Article/details/gnuexqgwe.sHtML

Go:   arr[1:4]
来源：http://mobile.hesvh.cn/Article/details/gyjdhsjiv.sHtML

Ruby: arr[1, 3]
来源：http://www.blog.zdbjq.cn/Article/details/grxhwmsod.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.m.share.fehbvm.com/Article/details/gyisknevk.sHtML

[D08] 合并两个数组
来源：http://m.share.zdbjq.cn/Article/details/ghbeavide.sHtML

Py:   a + b;  a.extend(b)
来源：http://blog.fehbvm.com/Article/details/gkhfovhqk.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gvaononkm.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gdiwhhidu.sHtML

TS:   [...a, ...b];
来源：http://www.share.zdbjq.cn/Article/details/gfhfwvasm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.share.fehbvm.com/Article/details/gwfhkbfjl.sHtML

Go:   append(a, b...)
来源：http://m.share.fehbvm.com/Article/details/gquiuyple.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gcejjkile.sHtML

C#:   a.Concat(b).ToList()
来源：http://read.share.zdbjq.cn/Article/details/grxifjesh.sHtML

[D09] 排序（升序）
来源：http://m.share.zdbjq.cn/Article/details/gttdobvro.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gufmnrudj.sHtML

PHP:  sort($arr);
来源：http://3g.fehbvm.com/Article/details/grldadmpu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gwxubzdms.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.zdbjq.cn/Article/details/gvgdlagvc.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://wap.hesvh.cn/Article/details/gcsrpnjmm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gtgpplebk.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gykrfetpp.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gsoygjmdo.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://baike.hesvh.cn/Article/details/gwwziuxik.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.hesvh.cn/Article/details/gtyidxhxv.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.share.zdbjq.cn/Article/details/gritvsfgl.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gqthzodeo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.hesvh.cn/Article/details/gpqtaykkl.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gvfgwidfx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.fehbvm.com/Article/details/gwxzydttj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gxgntfzsv.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.hesvh.cn/Article/details/gatcblupz.sHtML

[D11] 反转数组
来源：http://read.share.fehbvm.com/Article/details/gjgrtdckm.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.hesvh.cn/Article/details/gzlblstdi.sHtML

PHP:  array_reverse($arr);
来源：http://wap.zdbjq.cn/Article/details/gvxwyrtkm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.hesvh.cn/Article/details/gynmmvvgl.sHtML

TS:   [...arr].reverse();
来源：http://www.blog.hesvh.cn/Article/details/gkxmbgelw.sHtML

Java: Collections.reverse(list);
来源：http://m.share.zdbjq.cn/Article/details/gwucvfblm.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gxocpgaan.sHtML

Ruby: arr.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gjepbeunr.sHtML

C#:   list.Reverse();
来源：http://read.share.fehbvm.com/Article/details/gfxneenzs.sHtML

[D12] 查找元素下标
来源：http://3g.zdbjq.cn/Article/details/guzophjiv.sHtML

Py:   arr.index(x);  x in arr
来源：http://wap.hesvh.cn/Article/details/gufaweqob.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gfyvbelaj.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/galiocwyw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gfnttuxfo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gzemmgaxv.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpybrzuiz.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gbhuhtdfg.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gcyxztugq.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.fehbvm.com/Article/details/gcnixhawx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gmzepzeeh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gsvmssnsy.sHtML

JS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gfntdhlym.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.zdbjq.cn/Article/details/gfxfxsjjf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.zdbjq.cn/Article/details/gqvmdtjxl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.fehbvm.com/Article/details/gswhmumgx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gsoozesxd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.hesvh.cn/Article/details/ghrclvsdq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.hesvh.cn/Article/details/gbagxgzqf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gvnrebfcl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gmqsrqttt.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzwfgdzpy.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gwyotugun.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gqacaasmg.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gqlkvvvcj.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gamwoypef.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://3g.hesvh.cn/Article/details/gjtqyqzgk.sHtML

[D15] 去重
来源：http://read.share.fehbvm.com/Article/details/gbxqeygda.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gvysegndq.sHtML

PHP:  array_unique($arr);
来源：http://wap.hesvh.cn/Article/details/gpfguxfpk.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/ggswmiknh.sHtML

TS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/ghmcmrzed.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.zdbjq.cn/Article/details/gwjzlgaee.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.zdbjq.cn/Article/details/gxxojccuu.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/ggbeiowbw.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.fehbvm.com/Article/details/gdcljjgra.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/gviweyuhs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxozfzx.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gesujdktw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gsjwmiqfc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gciobydwg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.zdbjq.cn/Article/details/gyvrbjaep.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gbpdwresd.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gpgvxgngd.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.zdbjq.cn/Article/details/gvqbppbab.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gtfnucagw.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.zdbjq.cn/Article/details/gpdrygpom.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gfoytcjws.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gsuejdjfc.sHtML

TS:   Math.max(...arr);
来源：http://m.share.zdbjq.cn/Article/details/glfyjrheu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.zdbjq.cn/Article/details/gozgypsri.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gvczbvjom.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.hesvh.cn/Article/details/ggbkunxfi.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/gojdjnwkg.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/girniygdj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gkocqgapy.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gnfbfzbou.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gvxvpelhe.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gklcgcubc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gbzaqcpsp.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/guoqcfajl.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gaexbzrgk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/geffmtehs.sHtML

[D19] 按字段分组
来源：http://www.m.share.fehbvm.com/Article/details/gyirqtvpt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/ggodfscca.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.fehbvm.com/Article/details/guxeavfrl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/ggmlfdluh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gftbfutyr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gvefiwslq.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gndnsepnd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/ghaokhvek.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.zdbjq.cn/Article/details/gyrrtsqpi.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gbidrgypy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gqwucjwxm.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gfjulfzgt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gcjlumfqr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gaoihsfrx.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.zdbjq.cn/Article/details/gtmrcwzun.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gxsudttqf.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/gnodfefjv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fehbvm.com/Article/details/gysonxbxp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gsnpzmzks.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/glrjiylwp.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gigxjzadn.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/graovnawi.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gngiwnovg.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gretaszkm.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gqyxsnwhp.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gvtakgkrk.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gdfxinvkf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gifvrifcb.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gvoujvnhe.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gdplbjhst.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/grnxsllnq.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gmhcemjhh.sHtML

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gcgwudqrs.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.hesvh.cn/Article/details/godyguhve.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.hesvh.cn/Article/details/gtkpnilat.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/goynhtadz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gjiexkaqj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gblaluloi.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gpnyokvop.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gwvtjhesy.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/grqojssjj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gclpjrjuo.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gdgszddfs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gqsdlimxc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gxxfpterv.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/ggparcrfq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gmeyczipe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gnylmjxkk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gjtdraive.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gvstmmtfp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/ginpzfjpj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.zdbjq.cn/Article/details/gbijcjvuf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gcokmvbvm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gvzuoajvm.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gdvgaucgf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gtzqlocxk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gwjffrmxc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gavaohqph.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gtuwxxgpy.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gbnhozzjb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/gpdbrmqik.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/grjrbprzq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gucwllgok.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gdmzscuyw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gxolviyyr.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gpzhisqbd.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gayoupgnk.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/ginvncoem.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gxgrvprad.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gfvteylby.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gikuaocfn.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/glwalpzda.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/goxkzecfp.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/geejgzpwm.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdpdizyps.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gbaqokonf.sHtML


<!-- 参考信息 -->