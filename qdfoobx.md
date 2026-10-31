代发 wailian999

[C10] 变量作用域
来源：http://eq.newstarts.cn

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://qh.huixinmuqiang.cn

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://oe.yuexingan06.cn

JS:   let/const 块级作用域，var 函数级作用域
来源：http://rd.nszjky.cn

TS:   同 JS
来源：http://cc.wgjwhj.cn

Java: 方法内为块级作用域
来源：http://tq.hahajie.cn

Go:   花括号块级作用域
来源：http://zw.521024.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://is.asd995.cn

C#:   块级作用域
来源：http://px.jctech888.com.cn

[C11] 模块导入与导出
来源：http://to.yuexingan06.cn

Py:   from module import func
来源：http://ou.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://sk.nszjky.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://qp.chemitech.net.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://th.szxytkj.cn

Java: import java.util.List;
来源：http://bu.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://tu.huixinmuqiang.cn

Ruby: require "json"; require_relative "./util"
来源：http://yz.521024.cn

C#:   using System.Text;
来源：http://jm.nszjky.cn

[C12] 立即执行函数 IIFE
来源：http://zl.asd995.cn

Py:   (lambda: print("run"))()
来源：http://ve.jianghongdianzi.cn

PHP:  (function () { echo "run"; })();
来源：http://ks.haigaiapp.cn

JS:   (() => { console.log("run"); })();
来源：http://ql.nicolike.cn

TS:   (() => { console.log("run"); })();
来源：http://da.bookmarksfly.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://ro.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://eu.hahajie.cn

Ruby: -> { puts "run" }.call
来源：http://mo.muxihuayi.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://fk.jianghongdianzi.cn

[C13] 类型声明 / 类型注解
来源：http://ky.shxzukj.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qb.colortex.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://ef.gzmigu.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://gi.521024.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://il.colortex.cn

Java: int add(int a, int b) { return a + b; }
来源：http://lv.yuntaijiaju.cn

Go:   func add(a, b int) int
来源：http://rk.muxihuayi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://mq.bjjhwx.cn

C#:   int Add(int a, int b) => a + b;
来源：http://ht.nicolike.cn

[C14] 泛型函数
来源：http://el.yuexingan06.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ew.huixiangedu.cn

PHP:  // 无泛型
来源：http://ct.nszjky.cn

JS:   // 无泛型
来源：http://jz.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fz.huixinmuqiang.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hb.huixiangedu.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xd.bookmarksfly.cn

Ruby: # 无泛型
来源：http://bp.521024.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://ho.jctech888.com.cn

[C15] 解构 / 展开参数
来源：http://qd.huixinmuqiang.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ud.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://bc.yuexingan06.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ne.shxzskj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://cl.nszjky.cn

Java: // 无解构
来源：http://np.shxzskj.cn

Go:   // 无解构
来源：http://tp.colortex.cn

Ruby: a, b = pair
来源：http://ol.gzmigu.cn

C#:   var (a, b) = pair;
来源：http://jz.asd995.cn

[C16] 函数 / 方法重载
来源：http://zx.szxytkj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://in.shxzskj.cn

PHP:  // 无重载
来源：http://ef.hnjuh.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://xp.huixinmuqiang.cn

TS:   // 用联合类型或重载签名声明
来源：http://lm.shtwfgs.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://kj.chemitech.net.cn

Go:   // 无重载：用不同函数名
来源：http://uv.shxzukj.cn

Ruby: # 无重载：靠动态参数
来源：http://wb.9csxet.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://fh.hahajie.cn

================================================================================
来源：http://sg.hahajie.cn

D. 数组 / 列表 / 集合
来源：http://og.shtwfgs.cn

================================================================================
来源：http://lk.bjjhwx.cn

[D01] 创建数组 / 列表
来源：http://mr.yuexingan06.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://mu.shxzukj.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://kq.huixinmuqiang.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ew.huanxung.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ix.wgjwhj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://sy.yuntaijiaju.cn

Go:   arr := []int{1, 2, 3}
来源：http://ms.jctech888.com.cn

Ruby: arr = [1, 2, 3]
来源：http://py.haigaiapp.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://pf.muxihuayi.cn

[D02] 追加元素到末尾
来源：http://yn.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tw.huanxung.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://zg.huixinmuqiang.cn

JS:   arr.push(4);
来源：http://nk.bookmarksfly.cn

TS:   arr.push(4);
来源：http://bf.panjiajie.cn

Java: list.add(4);
来源：http://em.shxzskj.cn

Go:   arr = append(arr, 4)
来源：http://gv.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://yv.bjjhwx.cn

C#:   list.Add(4);
来源：http://kq.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://uu.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://ks.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fl.shtwfgs.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xv.lnxyls.cn

TS:   arr.splice(0, 0, 0);
来源：http://ku.wgjwhj.cn

Java: list.add(0, 0);
来源：http://ff.asd995.cn

Go:   arr = append([]int{0}, arr...)
来源：http://lk.shxzukj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ca.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://lf.bookmarksfly.cn

[D04] 删除元素
来源：http://vi.huixinmuqiang.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://kj.szxytkj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nn.newstarts.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://cw.panjiajie.cn

TS:   arr.splice(0, 1);
来源：http://qv.hahajie.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oa.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://sv.521024.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://gq.shxzskj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://tk.szsharing.cn

[D05] 访问与修改元素
来源：http://zg.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gl.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://xw.yuexingan06.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://tx.lnxyls.cn

TS:   arr[0]; arr.at(-1);
来源：http://bc.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://od.szsharing.cn

Go:   arr[0]; arr[0] = 9
来源：http://na.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://kn.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cd.wgjwhj.cn

[D06] 数组长度
来源：http://ur.colortex.cn

Py:   len(arr)
来源：http://qt.shxzskj.cn

PHP:  count($arr);
来源：http://qj.hnjuh.cn

JS:   arr.length
来源：http://ql.chemitech.net.cn

TS:   arr.length
来源：http://ir.asd995.cn

Java: list.size();
来源：http://ca.colortex.cn

Go:   len(arr)
来源：http://ce.szsharing.cn

Ruby: arr.length; arr.size
来源：http://wq.asd995.cn

C#:   list.Count;
来源：http://na.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://id.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://de.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://xe.haigaiapp.cn

JS:   arr.slice(1, 4);
来源：http://wl.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://wc.9csxet.cn

Java: list.subList(1, 4);
来源：http://wa.huanxung.cn

Go:   arr[1:4]
来源：http://ap.huanxung.cn

Ruby: arr[1, 3]
来源：http://vi.9csxet.cn

C#:   list.GetRange(1, 3);
来源：http://wv.chemitech.net.cn

[D08] 合并两个数组
来源：http://ee.bookmarksfly.cn

Py:   a + b;  a.extend(b)
来源：http://hp.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://ho.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wb.huixiangedu.cn

TS:   [...a, ...b];
来源：http://uu.haigaiapp.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jo.shtwfgs.cn

Go:   append(a, b...)
来源：http://jl.jianghongdianzi.cn

Ruby: a + b;  a.concat(b)
来源：http://it.yuntaijiaju.cn

C#:   a.Concat(b).ToList()
来源：http://xd.bjjhwx.cn

[D09] 排序（升序）
来源：http://sm.huixinmuqiang.cn

Py:   sorted(arr);  arr.sort()
来源：http://xg.panjiajie.cn

PHP:  sort($arr);
来源：http://qw.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://lx.hnjuh.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://fq.jctech888.com.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://lr.lnxyls.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mr.shtwfgs.cn

Ruby: arr.sort
来源：http://ss.jianghongdianzi.cn

C#:   list.Sort();
来源：http://fo.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fy.bookmarksfly.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ej.bjjhwx.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zh.nicolike.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yf.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://jl.colortex.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ym.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hn.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://gq.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wo.yuntaijiaju.cn

[D11] 反转数组
来源：http://rg.521024.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rh.9csxet.cn

PHP:  array_reverse($arr);
来源：http://be.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mf.9csxet.cn

TS:   [...arr].reverse();
来源：http://bb.hnjuh.cn

Java: Collections.reverse(list);
来源：http://yx.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://or.yuexingan06.cn

Ruby: arr.reverse
来源：http://vk.szsharing.cn

C#:   list.Reverse();
来源：http://so.newstarts.cn

[D12] 查找元素下标
来源：http://yx.haigaiapp.cn

Py:   arr.index(x);  x in arr
来源：http://vt.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qz.lnxyls.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://do.jianghongdianzi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://dw.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vn.panjiajie.cn

Go:   slices.Index(arr, x)
来源：http://di.lnxyls.cn

Ruby: arr.index(x)
来源：http://to.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ts.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://li.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kd.shxzskj.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://im.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://po.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://wn.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://dp.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://du.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://eb.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dg.yuntaijiaju.cn

[D14] 映射转换（每个元素变形）
来源：http://yf.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://am.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vq.hnjuh.cn

JS:   arr.map(x => x * 2)
来源：http://xs.lnxyls.cn

TS:   arr.map(x => x * 2)
来源：http://wy.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://yh.chemitech.net.cn

Go:   // 手写循环
来源：http://ho.szxytkj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://fa.bookmarksfly.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ru.hnjuh.cn

[D15] 去重
来源：http://fl.muxihuayi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ry.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://gm.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://ql.colortex.cn

TS:   [...new Set(arr)]
来源：http://qa.521024.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cm.lnxyls.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ll.bjjhwx.cn

Ruby: arr.uniq
来源：http://ko.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://px.szsharing.cn

[D16] 求和与平均值
来源：http://ke.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ra.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rf.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://cu.bookmarksfly.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ck.yuntaijiaju.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://if.szxytkj.cn

Go:   // 手写循环累加
来源：http://sw.jctech888.com.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gj.szxytkj.cn

C#:   list.Sum();  list.Average()
来源：http://qj.yuntaijiaju.cn

[D17] 最大值与最小值
来源：http://uh.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://gi.jctech888.com.cn

PHP:  max($arr);  min($arr);
来源：http://qw.nicolike.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://th.shxzskj.cn

TS:   Math.max(...arr);
来源：http://fc.colortex.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://xf.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://kf.huanxung.cn

Ruby: arr.max;  arr.min
来源：http://zy.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://eo.9csxet.cn

[D18] 扁平化嵌套数组
来源：http://bp.asd995.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sl.huixinmuqiang.cn

PHP:  array_merge(...$nested);
来源：http://ui.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fy.huanxung.cn

TS:   nested.flat();
来源：http://ws.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qa.chemitech.net.cn

Go:   // 手写双层循环
来源：http://tq.panjiajie.cn

Ruby: nested.flatten
来源：http://ff.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://wr.shtwfgs.cn

[D19] 按字段分组
来源：http://wh.nszjky.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://zj.haigaiapp.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jm.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xt.yuexingan06.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://at.gzmigu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://eh.nicolike.cn

Go:   // 手写 map[string][]T
来源：http://he.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ww.szxytkj.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://rn.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://lz.szsharing.cn

Py:   Counter(arr)
来源：http://gd.newstarts.cn

PHP:  array_count_values($arr);
来源：http://pd.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ya.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wg.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://jx.shxzskj.cn

Go:   // 手写 map[T]int
来源：http://py.gzmigu.cn

Ruby: arr.tally
来源：http://wo.bookmarksfly.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ty.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://mr.yuexingan06.cn

Py:   x in arr
来源：http://zh.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://de.haigaiapp.cn

JS:   arr.includes(x)
来源：http://df.jctech888.com.cn

TS:   arr.includes(x)
来源：http://vs.chemitech.net.cn

Java: list.contains(x)
来源：http://ou.huixinmuqiang.cn

Go:   slices.Contains(arr, x)
来源：http://pt.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://aq.asd995.cn

C#:   list.Contains(x)
来源：http://zd.bjjhwx.cn

[D22] 复制数组（避免共享引用）
来源：http://vc.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://av.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://px.jianghongdianzi.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://td.newstarts.cn

TS:   [...arr];
来源：http://mg.nicolike.cn

Java: new ArrayList<>(list);
来源：http://he.wgjwhj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://df.hnjuh.cn

Ruby: arr.dup;  arr.clone
来源：http://vd.shtwfgs.cn

C#:   new List<int>(list);
来源：http://oq.nszjky.cn

[D23] reduce 累积计算
来源：http://kw.nicolike.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yd.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pw.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ra.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ih.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ri.nicolike.cn

Go:   // 手写循环
来源：http://xs.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mf.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mt.huixiangedu.cn

[D24] 字典 / Map 基本操作
来源：http://fe.muxihuayi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://er.huixinmuqiang.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://qc.shxzukj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ng.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://sp.huixinmuqiang.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mb.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://yj.hahajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://sh.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pc.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://xc.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ue.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hu.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bc.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://at.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dw.9csxet.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lm.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://lb.huixinmuqiang.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://za.shtwfgs.cn

[D26] 数组转字符串
来源：http://lf.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://vg.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://kk.wgjwhj.cn

JS:   arr.join(", ")
来源：http://yv.yuexingan06.cn

TS:   arr.join(", ")
来源：http://dt.nicolike.cn

Java: String.join(", ", list)
来源：http://su.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://yt.yuntaijiaju.cn

Ruby: arr.join(", ")
来源：http://sj.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://mj.shtwfgs.cn


<!-- 参考信息 -->