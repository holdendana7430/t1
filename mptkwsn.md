代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://m.share.hesvh.cn/Article/details/gwigqfbbr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://m.share.zdbjq.cn/Article/details/grdtwskwi.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gecajemcb.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.blog.fehbvm.com/Article/details/geqrienyi.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://www.blog.fehbvm.com/Article/details/gubytqpcz.sHtML

C#:   using System.Text;
来源：http://baike.fehbvm.com/Article/details/gsqgxzwzq.sHtML

[C12] 立即执行函数 IIFE
来源：http://m.share.fehbvm.com/Article/details/gbfysltme.sHtML

Py:   (lambda: print("run"))()
来源：http://baike.hesvh.cn/Article/details/gdjxlswra.sHtML

PHP:  (function () { echo "run"; })();
来源：http://www.blog.zdbjq.cn/Article/details/gnpwwlrhu.sHtML

JS:   (() => { console.log("run"); })();
来源：http://mobile.fehbvm.com/Article/details/goatrsfvf.sHtML

TS:   (() => { console.log("run"); })();
来源：http://wap.zdbjq.cn/Article/details/gsppblzsh.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.m.share.hesvh.cn/Article/details/giglvvkvj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://baike.fehbvm.com/Article/details/gdublmxxl.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/givhedzfo.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://baike.fehbvm.com/Article/details/gterkojqi.sHtML

[C13] 类型声明 / 类型注解
来源：http://m.share.zdbjq.cn/Article/details/ghebzpjov.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://3g.hesvh.cn/Article/details/gkwaaxmif.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/ggrwknkbw.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://read.share.hesvh.cn/Article/details/gbujlxxsk.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkeeqqmlx.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gchatxbvi.sHtML

Go:   func add(a, b int) int
来源：http://baike.fehbvm.com/Article/details/gzovraitr.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.m.share.hesvh.cn/Article/details/giwldhiee.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.hesvh.cn/Article/details/gaepwlljn.sHtML

[C14] 泛型函数
来源：http://read.share.fehbvm.com/Article/details/goaoioqzu.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://m.share.fehbvm.com/Article/details/gnoayyvpl.sHtML

PHP:  // 无泛型
来源：http://m.share.zdbjq.cn/Article/details/guzvfkogp.sHtML

JS:   // 无泛型
来源：http://www.blog.zdbjq.cn/Article/details/gupjgxmes.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://wap.fehbvm.com/Article/details/gmaqvjejf.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbsbmik.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gormtmkwv.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/guetietnn.sHtML

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.blog.zdbjq.cn/Article/details/gulaexqbd.sHtML

[C15] 解构 / 展开参数
来源：http://blog.fehbvm.com/Article/details/gflmgalft.sHtML

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wap.zdbjq.cn/Article/details/gtnxsyysl.sHtML

PHP:  [$a, $b] = $pair;
来源：http://www.m.share.fehbvm.com/Article/details/goairqfon.sHtML

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://baike.fehbvm.com/Article/details/gkgmwogsk.sHtML

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://blog.hesvh.cn/Article/details/gnycdeemt.sHtML

Java: // 无解构
来源：http://mobile.fehbvm.com/Article/details/guadpxeqe.sHtML

Go:   // 无解构
来源：http://www.m.share.fehbvm.com/Article/details/gwdgtmdtc.sHtML

Ruby: a, b = pair
来源：http://www.blog.zdbjq.cn/Article/details/gatxzluiu.sHtML

C#:   var (a, b) = pair;
来源：http://mobile.hesvh.cn/Article/details/gekqapbkr.sHtML

[C16] 函数 / 方法重载
来源：http://www.blog.hesvh.cn/Article/details/gslpoeeml.sHtML

Py:   # 无重载：用默认参数或 *args 变通
来源：http://blog.hesvh.cn/Article/details/ghivfindf.sHtML

PHP:  // 无重载
来源：http://read.share.fehbvm.com/Article/details/gqaqbtcmj.sHtML

JS:   // 无重载：靠 arguments.length 分支
来源：http://wap.zdbjq.cn/Article/details/gpvlgapvw.sHtML

TS:   // 用联合类型或重载签名声明
来源：http://www.share.fehbvm.com/Article/details/gepxowxjf.sHtML

Java: void f(int a) {}  void f(String a) {}
来源：http://3g.zdbjq.cn/Article/details/gtyflblvv.sHtML

Go:   // 无重载：用不同函数名
来源：http://blog.zdbjq.cn/Article/details/gakasdmaz.sHtML

Ruby: # 无重载：靠动态参数
来源：http://mobile.fehbvm.com/Article/details/gdogxjpdl.sHtML

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.m.share.fehbvm.com/Article/details/gcbwuhebq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwgxllyfv.sHtML

D. 数组 / 列表 / 集合
来源：http://baike.zdbjq.cn/Article/details/gzvesznfr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggvgkrksy.sHtML

[D01] 创建数组 / 列表
来源：http://mobile.zdbjq.cn/Article/details/guycpmrjo.sHtML

Py:   arr = [1, 2, 3];  empty = []
来源：http://wap.zdbjq.cn/Article/details/gcnpfnpqn.sHtML

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://mobile.fehbvm.com/Article/details/gpnmoksbx.sHtML

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://mobile.zdbjq.cn/Article/details/goghwroqq.sHtML

TS:   const arr: number[] = [1, 2, 3];
来源：http://baike.zdbjq.cn/Article/details/gchgzislu.sHtML

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://baike.hesvh.cn/Article/details/gkctrmbwm.sHtML

Go:   arr := []int{1, 2, 3}
来源：http://mobile.zdbjq.cn/Article/details/gvxcmrlsu.sHtML

Ruby: arr = [1, 2, 3]
来源：http://www.m.share.fehbvm.com/Article/details/gyhisxvcu.sHtML

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://m.share.fehbvm.com/Article/details/gfydqhzko.sHtML

[D02] 追加元素到末尾
来源：http://www.share.hesvh.cn/Article/details/gtmmttlni.sHtML

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wap.zdbjq.cn/Article/details/gmtyoohck.sHtML

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://blog.fehbvm.com/Article/details/gdsbudocj.sHtML

JS:   arr.push(4);
来源：http://www.blog.hesvh.cn/Article/details/gcgmgsybv.sHtML

TS:   arr.push(4);
来源：http://3g.zdbjq.cn/Article/details/gkjnqlyex.sHtML

Java: list.add(4);
来源：http://wap.fehbvm.com/Article/details/gqsziuwbl.sHtML

Go:   arr = append(arr, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gwhhrclnh.sHtML

Ruby: arr << 4; arr.push(5)
来源：http://3g.hesvh.cn/Article/details/gkpzlbkzp.sHtML

C#:   list.Add(4);
来源：http://3g.hesvh.cn/Article/details/gpyktipcr.sHtML

[D03] 在指定位置插入元素
来源：http://www.m.share.hesvh.cn/Article/details/gerxuihov.sHtML

Py:   arr.insert(0, 0)
来源：http://baike.hesvh.cn/Article/details/grapgylvb.sHtML

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.m.share.zdbjq.cn/Article/details/gzeeccuoj.sHtML

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.blog.fehbvm.com/Article/details/gunbwkntq.sHtML

TS:   arr.splice(0, 0, 0);
来源：http://www.blog.fehbvm.com/Article/details/gqlqgjklv.sHtML

Java: list.add(0, 0);
来源：http://3g.hesvh.cn/Article/details/gmvwpuoni.sHtML

Go:   arr = append([]int{0}, arr...)
来源：http://www.share.hesvh.cn/Article/details/gowzjdgvx.sHtML

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://baike.zdbjq.cn/Article/details/grjveakqp.sHtML

C#:   list.Insert(0, 0);
来源：http://mobile.zdbjq.cn/Article/details/gkxpqgpqq.sHtML

[D04] 删除元素
来源：http://wap.zdbjq.cn/Article/details/gwkofivuc.sHtML

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wap.fehbvm.com/Article/details/gkzfxcztm.sHtML

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjbozjaxb.sHtML

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://mobile.zdbjq.cn/Article/details/gmjxrriic.sHtML

TS:   arr.splice(0, 1);
来源：http://baike.hesvh.cn/Article/details/gxcefdmqm.sHtML

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.blog.hesvh.cn/Article/details/gwrcdgaei.sHtML

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://3g.fehbvm.com/Article/details/gdidsgxlz.sHtML

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.blog.hesvh.cn/Article/details/gtobntsro.sHtML

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.m.share.zdbjq.cn/Article/details/ggpkockae.sHtML

[D05] 访问与修改元素
来源：http://m.share.hesvh.cn/Article/details/gprafgyda.sHtML

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://m.share.zdbjq.cn/Article/details/guchhdfuy.sHtML

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wap.hesvh.cn/Article/details/geqxgwbwk.sHtML

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wap.zdbjq.cn/Article/details/gpsknjnos.sHtML

TS:   arr[0]; arr.at(-1);
来源：http://www.blog.hesvh.cn/Article/details/glcqywqkm.sHtML

Java: list.get(0); list.set(0, 9);
来源：http://baike.zdbjq.cn/Article/details/gbvgllfwo.sHtML

Go:   arr[0]; arr[0] = 9
来源：http://www.m.share.hesvh.cn/Article/details/goiailvjz.sHtML

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://blog.hesvh.cn/Article/details/gpizqfvmq.sHtML

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.blog.fehbvm.com/Article/details/grsmjykka.sHtML

[D06] 数组长度
来源：http://baike.fehbvm.com/Article/details/glzhpnkco.sHtML

Py:   len(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggptjlwfu.sHtML

PHP:  count($arr);
来源：http://wap.hesvh.cn/Article/details/gkkaztnqn.sHtML

JS:   arr.length
来源：http://blog.fehbvm.com/Article/details/gupvfhubv.sHtML

TS:   arr.length
来源：http://baike.zdbjq.cn/Article/details/getmfamrh.sHtML

Java: list.size();
来源：http://www.blog.hesvh.cn/Article/details/ggouhoyxz.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/grkalfdqs.sHtML

Ruby: arr.length; arr.size
来源：http://blog.fehbvm.com/Article/details/giamijfly.sHtML

C#:   list.Count;
来源：http://mobile.fehbvm.com/Article/details/ggbenwswn.sHtML

[D07] 切片 / 取子数组
来源：http://baike.zdbjq.cn/Article/details/gqjxqigzk.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://mobile.fehbvm.com/Article/details/gcgpdsqoy.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://wap.zdbjq.cn/Article/details/giejxccxv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/goasjnhqk.sHtML

TS:   arr.slice(1, 4);
来源：http://www.share.fehbvm.com/Article/details/gimsmvucb.sHtML

Java: list.subList(1, 4);
来源：http://blog.hesvh.cn/Article/details/gbmmpcymn.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gqfefxrub.sHtML

Ruby: arr[1, 3]
来源：http://baike.fehbvm.com/Article/details/godkojpbz.sHtML

C#:   list.GetRange(1, 3);
来源：http://blog.fehbvm.com/Article/details/gaehmryqe.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gpkbhkdsb.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.zdbjq.cn/Article/details/gdeapachm.sHtML

PHP:  array_merge($a, $b);
来源：http://mobile.zdbjq.cn/Article/details/gkixdjpxu.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.fehbvm.com/Article/details/ggysubwpr.sHtML

TS:   [...a, ...b];
来源：http://m.share.zdbjq.cn/Article/details/gmukoedru.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://blog.hesvh.cn/Article/details/genvvmwsy.sHtML

Go:   append(a, b...)
来源：http://wap.zdbjq.cn/Article/details/gxgokioet.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/glfcptshn.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.fehbvm.com/Article/details/gojwzqgpa.sHtML

[D09] 排序（升序）
来源：http://blog.hesvh.cn/Article/details/gylrigbrw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gelmwatbu.sHtML

PHP:  sort($arr);
来源：http://m.share.zdbjq.cn/Article/details/guauhtfvn.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gcblntsrp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.share.fehbvm.com/Article/details/gaphivkaf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://blog.fehbvm.com/Article/details/gpnuzhgnb.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggzrzjckz.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gdrgsqmza.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/geyxyppts.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.zdbjq.cn/Article/details/gmirlofgz.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gyqszfzvi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.m.share.fehbvm.com/Article/details/ggeuorxlf.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.hesvh.cn/Article/details/gulncphqy.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gmozdhjjb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/gpywvvlgg.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.hesvh.cn/Article/details/gculsjvjr.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://3g.hesvh.cn/Article/details/guafuuzdy.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://3g.hesvh.cn/Article/details/gizxmsbpe.sHtML

[D11] 反转数组
来源：http://read.share.zdbjq.cn/Article/details/gubvapfto.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gmpljvxwp.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.fehbvm.com/Article/details/gjemqnbxi.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.zdbjq.cn/Article/details/gkrcqubqx.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gqwlmozia.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gqaideycn.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.zdbjq.cn/Article/details/gazdsnxuu.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gorfrtujm.sHtML

C#:   list.Reverse();
来源：http://3g.zdbjq.cn/Article/details/gcdtbhxgx.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/ghejfoitl.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/ghxgywckc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.hesvh.cn/Article/details/grysgnrst.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.zdbjq.cn/Article/details/gqrzaqrzb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.hesvh.cn/Article/details/gaixdfllf.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.zdbjq.cn/Article/details/gvfcbzyqm.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gibrlcrfs.sHtML

Ruby: arr.index(x)
来源：http://read.share.hesvh.cn/Article/details/grlvmmcfe.sHtML

C#:   list.IndexOf(x);
来源：http://wap.fehbvm.com/Article/details/gizimqmop.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/gyxiipkzy.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.hesvh.cn/Article/details/ggbabckxe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gvvvlyhbd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gwqiblgiy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gkvtvhutm.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/ghnieairj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/glpqsmott.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/ghevapwcx.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gthdgbnap.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.zdbjq.cn/Article/details/gqvnyzewi.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.zdbjq.cn/Article/details/gpxgwoyzl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.share.hesvh.cn/Article/details/gxiaylhae.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gmtmwdcal.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.fehbvm.com/Article/details/gyqdftuca.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gocpjevxh.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gbjqdueat.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gfuqnbfui.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/gqseymajx.sHtML

[D15] 去重
来源：http://m.share.fehbvm.com/Article/details/gzipehnty.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gtzcbsbxj.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giiqosess.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gfuoudmjw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.hesvh.cn/Article/details/gprixmkqy.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gcdwwsoia.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://read.share.hesvh.cn/Article/details/gthklnjkb.sHtML

Ruby: arr.uniq
来源：http://m.share.fehbvm.com/Article/details/gyrbkdrxn.sHtML

C#:   list.Distinct().ToList()
来源：http://mobile.zdbjq.cn/Article/details/gvepgoqoo.sHtML

[D16] 求和与平均值
来源：http://3g.zdbjq.cn/Article/details/gapgprqfx.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gtbplmicv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.hesvh.cn/Article/details/gvbfweeit.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gabtmtjmb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmikxqhyy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.fehbvm.com/Article/details/gjzrdxnsn.sHtML

Go:   // 手写循环累加
来源：http://baike.hesvh.cn/Article/details/gzqbzkkhg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.hesvh.cn/Article/details/gutmypvhd.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/ggkbwsoxh.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/guwnvrsrr.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gindxfrkm.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gkzqcjbzu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gueettpvr.sHtML

TS:   Math.max(...arr);
来源：http://mobile.hesvh.cn/Article/details/gsarhkobg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gdwguyqgl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/giqbfajpg.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gpynutsjg.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.zdbjq.cn/Article/details/gmevhevnv.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gplixufkh.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gvditmkuw.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gygxnzqec.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gjrlzpcjr.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/glwmdgmul.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gzrdelpdw.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gzvxtsfov.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gwswfwukf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gjuyscnsq.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gtchsceax.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gfzeeycoc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gquvzfzzt.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gtepbmypm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gagjgcuul.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gmfppeswp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gbgdutmyh.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gkpykpulk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gypqzlfcp.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/goicducxc.sHtML

Py:   Counter(arr)
来源：http://wap.zdbjq.cn/Article/details/gvvjwopjh.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gzvyrudhk.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gwtdmbfxb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gtomteree.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.fehbvm.com/Article/details/guhzfylig.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.zdbjq.cn/Article/details/gwffclaem.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gtajdmzwm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.zdbjq.cn/Article/details/gkkwkgcut.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gkciwhise.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gicoskjct.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gusxznkkd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqewsmsbr.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gvzjfwzvs.sHtML

Java: list.contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gtyyaqpiq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/ghwbqugll.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjmnnfoxz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gnlaiofev.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gvibohmwo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gnmanngvr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gualprfkw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gwatvqaig.sHtML

TS:   [...arr];
来源：http://wap.zdbjq.cn/Article/details/gtmsijdgs.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gaxtixgqi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gcouwkdrs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.hesvh.cn/Article/details/gswjbxmus.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gtbixueja.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/grljdkvvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcrrzffbq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/ghtrcfopi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gpfeebyjo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gufvvnrjc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/guvmccpez.sHtML

Go:   // 手写循环
来源：http://m.share.fehbvm.com/Article/details/gpagwuleq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/grjbtmoaw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gxuxhudgb.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gelpgrxft.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gczfjcocy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.hesvh.cn/Article/details/geafhulgv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fehbvm.com/Article/details/gbakwcvks.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/gjiacsnvt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gvvycesfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gwkesents.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gtqjusoqo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gwgszycds.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gevpbiapg.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gtwlqcomy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gxwpsarge.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gunalvrko.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/gjrpwdzan.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gprfkahxu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gxraogulw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gecwtopvj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gibaebhid.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gqqzhlosn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gvtgondux.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gstufmgxv.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gzaanxafe.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gjqbzfrdb.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/ggdbbewlh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gzxmjsfhy.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gglevtixa.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gygwcdpeq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gxwupzveo.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gwibtrgau.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjklwrrri.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gqsmezwba.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/guxqspsql.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/ghrouflwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gfzpdillw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gqqwbxbqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gpvkgsmon.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/guznicncm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/guurrnpfd.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gmexclttn.sHtML


<!-- 参考信息 -->