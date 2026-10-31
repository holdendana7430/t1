代发 wailian999

TS:   同 JS
来源：http://yo.bookmarksfly.cn

Java: 方法内为块级作用域
来源：http://lk.wgjwhj.cn

Go:   花括号块级作用域
来源：http://cv.gzmigu.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://pi.jctech888.com.cn

C#:   块级作用域
来源：http://mi.nszjky.cn

[C11] 模块导入与导出
来源：http://yk.szxytkj.cn

Py:   from module import func
来源：http://ih.wgjwhj.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://bc.yuexingan06.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://pb.bjjhwx.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hp.jianghongdianzi.cn

Java: import java.util.List;
来源：http://vf.bjjhwx.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://oo.bookmarksfly.cn

Ruby: require "json"; require_relative "./util"
来源：http://gx.yuntaijiaju.cn

C#:   using System.Text;
来源：http://xl.panjiajie.cn

[C12] 立即执行函数 IIFE
来源：http://ex.bjjhwx.cn

Py:   (lambda: print("run"))()
来源：http://zy.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://kn.hahajie.cn

JS:   (() => { console.log("run"); })();
来源：http://ld.jctech888.com.cn

TS:   (() => { console.log("run"); })();
来源：http://rj.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://xt.muxihuayi.cn

Go:   func() { fmt.Println("run") }()
来源：http://ex.huixiangedu.cn

Ruby: -> { puts "run" }.call
来源：http://pr.nszjky.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://lj.521024.cn

[C13] 类型声明 / 类型注解
来源：http://hd.muxihuayi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ue.nicolike.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://jy.haigaiapp.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gg.9csxet.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://id.yuexingan06.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jz.chemitech.net.cn

Go:   func add(a, b int) int
来源：http://qr.newstarts.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://yp.shtwfgs.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ke.gzmigu.cn

[C14] 泛型函数
来源：http://bi.bookmarksfly.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://jq.hnjuh.cn

PHP:  // 无泛型
来源：http://jt.shxzskj.cn

JS:   // 无泛型
来源：http://ie.jctech888.com.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mj.szsharing.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://kl.panjiajie.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://gs.shxzskj.cn

Ruby: # 无泛型
来源：http://fu.shtwfgs.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lh.haigaiapp.cn

[C15] 解构 / 展开参数
来源：http://yg.huanxung.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ag.huixiangedu.cn

PHP:  [$a, $b] = $pair;
来源：http://im.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://dr.lnxyls.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://az.wgjwhj.cn

Java: // 无解构
来源：http://is.colortex.cn

Go:   // 无解构
来源：http://nu.newstarts.cn

Ruby: a, b = pair
来源：http://rb.newstarts.cn

C#:   var (a, b) = pair;
来源：http://sv.lnxyls.cn

[C16] 函数 / 方法重载
来源：http://nf.yuexingan06.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://xy.nicolike.cn

PHP:  // 无重载
来源：http://tf.chemitech.net.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ky.colortex.cn

TS:   // 用联合类型或重载签名声明
来源：http://fu.muxihuayi.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://zn.yuntaijiaju.cn

Go:   // 无重载：用不同函数名
来源：http://sf.huixiangedu.cn

Ruby: # 无重载：靠动态参数
来源：http://pf.haigaiapp.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://xu.nszjky.cn

================================================================================
来源：http://ib.jctech888.com.cn

D. 数组 / 列表 / 集合
来源：http://bx.muxihuayi.cn

================================================================================
来源：http://ac.nszjky.cn

[D01] 创建数组 / 列表
来源：http://qz.bookmarksfly.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://xc.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hahajie.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://tr.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://nf.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://de.huanxung.cn

Go:   arr := []int{1, 2, 3}
来源：http://ob.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://av.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yh.wgjwhj.cn

[D02] 追加元素到末尾
来源：http://ec.521024.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://da.bookmarksfly.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://et.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://pr.hahajie.cn

TS:   arr.push(4);
来源：http://bc.colortex.cn

Java: list.add(4);
来源：http://qo.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://xs.huanxung.cn

Ruby: arr << 4; arr.push(5)
来源：http://ud.newstarts.cn

C#:   list.Add(4);
来源：http://sh.9csxet.cn

[D03] 在指定位置插入元素
来源：http://yt.nszjky.cn

Py:   arr.insert(0, 0)
来源：http://bi.lnxyls.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://xd.szsharing.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://bs.newstarts.cn

TS:   arr.splice(0, 0, 0);
来源：http://oo.huanxung.cn

Java: list.add(0, 0);
来源：http://qo.szxytkj.cn

Go:   arr = append([]int{0}, arr...)
来源：http://bm.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sf.huixiangedu.cn

C#:   list.Insert(0, 0);
来源：http://zl.jctech888.com.cn

[D04] 删除元素
来源：http://hy.9csxet.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://uj.huanxung.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://bq.asd995.cn

TS:   arr.splice(0, 1);
来源：http://au.nszjky.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://mn.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wh.hnjuh.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ob.nszjky.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ko.nszjky.cn

[D05] 访问与修改元素
来源：http://rs.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://vy.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://dy.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://xw.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://ki.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://dq.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://ic.bjjhwx.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://sn.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://uj.9csxet.cn

[D06] 数组长度
来源：http://qu.hnjuh.cn

Py:   len(arr)
来源：http://gw.9csxet.cn

PHP:  count($arr);
来源：http://fe.bookmarksfly.cn

JS:   arr.length
来源：http://pj.shtwfgs.cn

TS:   arr.length
来源：http://er.szsharing.cn

Java: list.size();
来源：http://sc.lnxyls.cn

Go:   len(arr)
来源：http://yp.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://um.shxzukj.cn

C#:   list.Count;
来源：http://cl.hahajie.cn

[D07] 切片 / 取子数组
来源：http://tr.jctech888.com.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ua.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://st.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://wk.nicolike.cn

TS:   arr.slice(1, 4);
来源：http://fa.shtwfgs.cn

Java: list.subList(1, 4);
来源：http://su.haigaiapp.cn

Go:   arr[1:4]
来源：http://iv.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://uh.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://jb.jianghongdianzi.cn

[D08] 合并两个数组
来源：http://wk.521024.cn

Py:   a + b;  a.extend(b)
来源：http://en.huixinmuqiang.cn

PHP:  array_merge($a, $b);
来源：http://yh.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://rq.colortex.cn

TS:   [...a, ...b];
来源：http://lg.nszjky.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ea.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://is.hahajie.cn

Ruby: a + b;  a.concat(b)
来源：http://oj.9csxet.cn

C#:   a.Concat(b).ToList()
来源：http://bm.lnxyls.cn

[D09] 排序（升序）
来源：http://wm.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://mt.panjiajie.cn

PHP:  sort($arr);
来源：http://ma.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://xh.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://mn.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://gs.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://um.521024.cn

Ruby: arr.sort
来源：http://xh.521024.cn

C#:   list.Sort();
来源：http://jl.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ny.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://sz.9csxet.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ev.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://ls.nicolike.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://lq.haigaiapp.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://gm.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://nt.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://cu.hahajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://oi.jctech888.com.cn

[D11] 反转数组
来源：http://ai.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lt.gzmigu.cn

PHP:  array_reverse($arr);
来源：http://yz.521024.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kx.9csxet.cn

TS:   [...arr].reverse();
来源：http://tr.szsharing.cn

Java: Collections.reverse(list);
来源：http://rg.gzmigu.cn

Go:   slices.Reverse(arr)
来源：http://ko.521024.cn

Ruby: arr.reverse
来源：http://jn.asd995.cn

C#:   list.Reverse();
来源：http://yq.521024.cn

[D12] 查找元素下标
来源：http://jn.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://hb.shtwfgs.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ee.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://qi.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://vp.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://mw.shtwfgs.cn

Go:   slices.Index(arr, x)
来源：http://jb.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://wg.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://vo.521024.cn

[D13] 过滤（保留满足条件的）
来源：http://kd.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://qn.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://od.bjjhwx.cn

JS:   arr.filter(x => x > 3)
来源：http://yu.521024.cn

TS:   arr.filter(x => x > 3)
来源：http://nt.hahajie.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://up.521024.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nb.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://jn.panjiajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gi.shxzskj.cn

[D14] 映射转换（每个元素变形）
来源：http://uv.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://sc.chemitech.net.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ms.yuntaijiaju.cn

JS:   arr.map(x => x * 2)
来源：http://wm.jianghongdianzi.cn

TS:   arr.map(x => x * 2)
来源：http://jp.yuntaijiaju.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tr.panjiajie.cn

Go:   // 手写循环
来源：http://tm.yuntaijiaju.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cp.colortex.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rc.chemitech.net.cn

[D15] 去重
来源：http://ix.panjiajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ql.nszjky.cn

PHP:  array_unique($arr);
来源：http://tg.521024.cn

JS:   [...new Set(arr)]
来源：http://py.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://rr.szxytkj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ht.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iw.huanxung.cn

Ruby: arr.uniq
来源：http://ma.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://yi.jctech888.com.cn

[D16] 求和与平均值
来源：http://hp.shxzukj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://iz.muxihuayi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gs.shxzukj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qp.haigaiapp.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fj.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bl.szxytkj.cn

Go:   // 手写循环累加
来源：http://kj.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mi.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://vd.asd995.cn

[D17] 最大值与最小值
来源：http://bz.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://vk.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://mz.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ks.lnxyls.cn

TS:   Math.max(...arr);
来源：http://mg.szsharing.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://uo.nszjky.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://go.hnjuh.cn

Ruby: arr.max;  arr.min
来源：http://tx.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://jw.panjiajie.cn

[D18] 扁平化嵌套数组
来源：http://cv.hnjuh.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ol.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://tr.bookmarksfly.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://qk.nszjky.cn

TS:   nested.flat();
来源：http://np.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://my.newstarts.cn

Go:   // 手写双层循环
来源：http://qp.shtwfgs.cn

Ruby: nested.flatten
来源：http://bv.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xf.gzmigu.cn

[D19] 按字段分组
来源：http://fy.hahajie.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qa.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://yy.panjiajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://pj.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rj.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://el.shxzukj.cn

Go:   // 手写 map[string][]T
来源：http://wl.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://li.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://iz.colortex.cn

[D20] 统计每个元素出现次数
来源：http://lo.nszjky.cn

Py:   Counter(arr)
来源：http://ki.huanxung.cn

PHP:  array_count_values($arr);
来源：http://og.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jl.newstarts.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://km.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gw.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://ar.shxzukj.cn

Ruby: arr.tally
来源：http://yk.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://aq.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://ce.yuntaijiaju.cn

Py:   x in arr
来源：http://wa.colortex.cn

PHP:  in_array($x, $arr, true);
来源：http://cj.panjiajie.cn

JS:   arr.includes(x)
来源：http://zz.shxzskj.cn

TS:   arr.includes(x)
来源：http://ya.huixinmuqiang.cn

Java: list.contains(x)
来源：http://pf.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://zh.nicolike.cn

Ruby: arr.include?(x)
来源：http://az.521024.cn

C#:   list.Contains(x)
来源：http://zw.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://be.muxihuayi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://xk.newstarts.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://un.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xl.shtwfgs.cn

TS:   [...arr];
来源：http://ss.szxytkj.cn

Java: new ArrayList<>(list);
来源：http://je.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://rr.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://tr.newstarts.cn

C#:   new List<int>(list);
来源：http://hk.yuntaijiaju.cn

[D23] reduce 累积计算
来源：http://fg.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ra.chemitech.net.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jc.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kw.hahajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ge.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mo.huixiangedu.cn

Go:   // 手写循环
来源：http://rs.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ux.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bv.jianghongdianzi.cn

[D24] 字典 / Map 基本操作
来源：http://kt.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://li.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cf.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://rg.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://bx.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://pj.panjiajie.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://jr.9csxet.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sr.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://bo.jianghongdianzi.cn

[D25] Set 集合去重与交并差
来源：http://cu.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jv.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qw.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wn.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pw.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ul.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://jl.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fi.huanxung.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://iw.9csxet.cn

[D26] 数组转字符串
来源：http://fk.shxzukj.cn

Py:   ", ".join(map(str, arr))
来源：http://qd.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://yl.hahajie.cn

JS:   arr.join(", ")
来源：http://zc.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ex.szsharing.cn

Java: String.join(", ", list)
来源：http://jc.muxihuayi.cn

Go:   strings.Join(strs, ", ")
来源：http://lm.huanxung.cn

Ruby: arr.join(", ")
来源：http://cz.shxzskj.cn

C#:   string.Join(", ", list)
来源：http://aw.bookmarksfly.cn

================================================================================
来源：http://ov.szxytkj.cn

E. 字符串处理
来源：http://wa.szsharing.cn

================================================================================
来源：http://jn.haigaiapp.cn

[E01] 拼接字符串
来源：http://gz.muxihuayi.cn


<!-- 参考信息 -->