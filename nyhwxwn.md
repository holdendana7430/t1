代发 wailian999

C#:   块级作用域
来源：http://vk.yuntaijiaju.cn

[C11] 模块导入与导出
来源：http://il.shxzskj.cn

Py:   from module import func
来源：http://rn.shtwfgs.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://zo.gzmigu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://rz.wgjwhj.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://xq.jctech888.com.cn

Java: import java.util.List;
来源：http://vo.huixinmuqiang.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://ux.chemitech.net.cn

Ruby: require "json"; require_relative "./util"
来源：http://aq.nszjky.cn

C#:   using System.Text;
来源：http://hg.chemitech.net.cn

[C12] 立即执行函数 IIFE
来源：http://xm.asd995.cn

Py:   (lambda: print("run"))()
来源：http://qa.colortex.cn

PHP:  (function () { echo "run"; })();
来源：http://yx.hnjuh.cn

JS:   (() => { console.log("run"); })();
来源：http://wf.lnxyls.cn

TS:   (() => { console.log("run"); })();
来源：http://lm.9csxet.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://um.hnjuh.cn

Go:   func() { fmt.Println("run") }()
来源：http://ik.shtwfgs.cn

Ruby: -> { puts "run" }.call
来源：http://ft.panjiajie.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://ev.shxzukj.cn

[C13] 类型声明 / 类型注解
来源：http://mk.jianghongdianzi.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://ol.shtwfgs.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://dv.jctech888.com.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://rl.panjiajie.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://fz.hnjuh.cn

Java: int add(int a, int b) { return a + b; }
来源：http://bl.9csxet.cn

Go:   func add(a, b int) int
来源：http://wo.nszjky.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://vf.shxzukj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://kg.nszjky.cn

[C14] 泛型函数
来源：http://vd.nszjky.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://vp.chemitech.net.cn

PHP:  // 无泛型
来源：http://cy.szxytkj.cn

JS:   // 无泛型
来源：http://ng.bookmarksfly.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://eb.yuexingan06.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://fr.wgjwhj.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://bf.panjiajie.cn

Ruby: # 无泛型
来源：http://bl.huixinmuqiang.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://bo.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://ri.nicolike.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ou.huanxung.cn

PHP:  [$a, $b] = $pair;
来源：http://ux.lnxyls.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://tt.jianghongdianzi.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://go.muxihuayi.cn

Java: // 无解构
来源：http://pl.nszjky.cn

Go:   // 无解构
来源：http://sx.chemitech.net.cn

Ruby: a, b = pair
来源：http://xx.9csxet.cn

C#:   var (a, b) = pair;
来源：http://kg.szsharing.cn

[C16] 函数 / 方法重载
来源：http://oa.asd995.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://kw.yuntaijiaju.cn

PHP:  // 无重载
来源：http://by.bookmarksfly.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://rf.panjiajie.cn

TS:   // 用联合类型或重载签名声明
来源：http://hg.521024.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://wn.bjjhwx.cn

Go:   // 无重载：用不同函数名
来源：http://sj.wgjwhj.cn

Ruby: # 无重载：靠动态参数
来源：http://gz.bjjhwx.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://dp.panjiajie.cn

================================================================================
来源：http://xh.panjiajie.cn

D. 数组 / 列表 / 集合
来源：http://vq.szsharing.cn

================================================================================
来源：http://qn.jctech888.com.cn

[D01] 创建数组 / 列表
来源：http://af.shxzskj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ck.hnjuh.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://cf.muxihuayi.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ih.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://jh.bjjhwx.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://rc.jctech888.com.cn

Go:   arr := []int{1, 2, 3}
来源：http://me.haigaiapp.cn

Ruby: arr = [1, 2, 3]
来源：http://tw.jctech888.com.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://od.bjjhwx.cn

[D02] 追加元素到末尾
来源：http://pc.shxzukj.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://sf.huixiangedu.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://oc.jctech888.com.cn

JS:   arr.push(4);
来源：http://hw.9csxet.cn

TS:   arr.push(4);
来源：http://ms.colortex.cn

Java: list.add(4);
来源：http://xb.wgjwhj.cn

Go:   arr = append(arr, 4)
来源：http://zm.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://uw.shxzskj.cn

C#:   list.Add(4);
来源：http://ae.jctech888.com.cn

[D03] 在指定位置插入元素
来源：http://or.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://aw.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vp.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://sz.bookmarksfly.cn

TS:   arr.splice(0, 0, 0);
来源：http://gg.wgjwhj.cn

Java: list.add(0, 0);
来源：http://km.9csxet.cn

Go:   arr = append([]int{0}, arr...)
来源：http://od.szsharing.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ai.yuexingan06.cn

C#:   list.Insert(0, 0);
来源：http://sw.shxzukj.cn

[D04] 删除元素
来源：http://km.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://wr.bookmarksfly.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ww.panjiajie.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://dl.szxytkj.cn

TS:   arr.splice(0, 1);
来源：http://ps.huixiangedu.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fn.chemitech.net.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hw.huixiangedu.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://os.lnxyls.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ml.shxzukj.cn

[D05] 访问与修改元素
来源：http://nu.huanxung.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://so.bjjhwx.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://up.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://mh.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://qs.asd995.cn

Java: list.get(0); list.set(0, 9);
来源：http://ke.colortex.cn

Go:   arr[0]; arr[0] = 9
来源：http://fo.hahajie.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yr.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ar.9csxet.cn

[D06] 数组长度
来源：http://ds.lnxyls.cn

Py:   len(arr)
来源：http://ts.hahajie.cn

PHP:  count($arr);
来源：http://fx.bjjhwx.cn

JS:   arr.length
来源：http://rx.huanxung.cn

TS:   arr.length
来源：http://jg.nicolike.cn

Java: list.size();
来源：http://dc.bjjhwx.cn

Go:   len(arr)
来源：http://fn.jctech888.com.cn

Ruby: arr.length; arr.size
来源：http://mh.jianghongdianzi.cn

C#:   list.Count;
来源：http://vv.lnxyls.cn

[D07] 切片 / 取子数组
来源：http://of.newstarts.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://pt.bjjhwx.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fo.szxytkj.cn

JS:   arr.slice(1, 4);
来源：http://vv.jianghongdianzi.cn

TS:   arr.slice(1, 4);
来源：http://eu.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://bm.jianghongdianzi.cn

Go:   arr[1:4]
来源：http://jk.wgjwhj.cn

Ruby: arr[1, 3]
来源：http://dm.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://nt.chemitech.net.cn

[D08] 合并两个数组
来源：http://my.muxihuayi.cn

Py:   a + b;  a.extend(b)
来源：http://gp.nszjky.cn

PHP:  array_merge($a, $b);
来源：http://as.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://yo.521024.cn

TS:   [...a, ...b];
来源：http://nv.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ca.newstarts.cn

Go:   append(a, b...)
来源：http://ty.nicolike.cn

Ruby: a + b;  a.concat(b)
来源：http://bz.yuexingan06.cn

C#:   a.Concat(b).ToList()
来源：http://ma.shxzskj.cn

[D09] 排序（升序）
来源：http://fw.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://uy.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://va.nicolike.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://co.bjjhwx.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://qi.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://jt.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sc.bookmarksfly.cn

Ruby: arr.sort
来源：http://re.muxihuayi.cn

C#:   list.Sort();
来源：http://yf.newstarts.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tm.shtwfgs.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://yl.huixiangedu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hd.lnxyls.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cj.jianghongdianzi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bj.wgjwhj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mi.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://zv.haigaiapp.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://si.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://iz.shxzukj.cn

[D11] 反转数组
来源：http://fx.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pc.hnjuh.cn

PHP:  array_reverse($arr);
来源：http://kn.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://td.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://gh.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://rj.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://rl.nszjky.cn

Ruby: arr.reverse
来源：http://wa.huanxung.cn

C#:   list.Reverse();
来源：http://bb.chemitech.net.cn

[D12] 查找元素下标
来源：http://io.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://cc.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://wi.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://lk.wgjwhj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://pw.9csxet.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ld.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://gt.9csxet.cn

Ruby: arr.index(x)
来源：http://vs.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://lq.bjjhwx.cn

[D13] 过滤（保留满足条件的）
来源：http://at.yuexingan06.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ec.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://tz.asd995.cn

JS:   arr.filter(x => x > 3)
来源：http://xs.huanxung.cn

TS:   arr.filter(x => x > 3)
来源：http://yd.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fx.nicolike.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ca.hnjuh.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qf.yuntaijiaju.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wp.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://vb.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gx.shxzskj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://id.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://lr.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://ow.bookmarksfly.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kf.gzmigu.cn

Go:   // 手写循环
来源：http://vn.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://si.newstarts.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oj.shxzskj.cn

[D15] 去重
来源：http://ex.521024.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mg.colortex.cn

PHP:  array_unique($arr);
来源：http://ga.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://tu.9csxet.cn

TS:   [...new Set(arr)]
来源：http://st.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pr.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://re.huanxung.cn

Ruby: arr.uniq
来源：http://db.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://iu.panjiajie.cn

[D16] 求和与平均值
来源：http://qd.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://dy.newstarts.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uv.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fk.colortex.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://sd.szxytkj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ga.muxihuayi.cn

Go:   // 手写循环累加
来源：http://ex.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://we.asd995.cn

C#:   list.Sum();  list.Average()
来源：http://cm.9csxet.cn

[D17] 最大值与最小值
来源：http://eb.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://uy.yuntaijiaju.cn

PHP:  max($arr);  min($arr);
来源：http://cv.hnjuh.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://nm.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://ya.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://fo.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://eg.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://ua.bookmarksfly.cn

C#:   list.Max();  list.Min()
来源：http://je.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://cn.hahajie.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://cq.asd995.cn

PHP:  array_merge(...$nested);
来源：http://lh.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ul.huixinmuqiang.cn

TS:   nested.flat();
来源：http://aj.jianghongdianzi.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mt.jianghongdianzi.cn

Go:   // 手写双层循环
来源：http://ar.panjiajie.cn

Ruby: nested.flatten
来源：http://xp.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zz.huixinmuqiang.cn

[D19] 按字段分组
来源：http://kr.hnjuh.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nd.huixiangedu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cy.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xh.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://zz.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hs.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://un.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://cc.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://af.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://re.jianghongdianzi.cn

Py:   Counter(arr)
来源：http://qp.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://qf.muxihuayi.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bk.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bj.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dq.asd995.cn

Go:   // 手写 map[T]int
来源：http://zl.yuexingan06.cn

Ruby: arr.tally
来源：http://ev.newstarts.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jy.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://fd.colortex.cn

Py:   x in arr
来源：http://nn.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://qr.jctech888.com.cn

JS:   arr.includes(x)
来源：http://lr.lnxyls.cn

TS:   arr.includes(x)
来源：http://ri.panjiajie.cn

Java: list.contains(x)
来源：http://sf.muxihuayi.cn

Go:   slices.Contains(arr, x)
来源：http://dg.hahajie.cn

Ruby: arr.include?(x)
来源：http://ee.nicolike.cn

C#:   list.Contains(x)
来源：http://px.panjiajie.cn

[D22] 复制数组（避免共享引用）
来源：http://cq.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oz.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xh.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://xe.huixiangedu.cn

TS:   [...arr];
来源：http://wr.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://hw.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xj.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ha.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://tp.lnxyls.cn

[D23] reduce 累积计算
来源：http://to.newstarts.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://yk.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://om.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wx.huanxung.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://op.colortex.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://wr.jianghongdianzi.cn

Go:   // 手写循环
来源：http://te.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://gx.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://se.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://yr.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://eg.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://in.521024.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xq.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jw.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://gf.chemitech.net.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bu.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://dm.huanxung.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://fe.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://pf.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://uf.bookmarksfly.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://jj.gzmigu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ny.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qs.szsharing.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hh.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://iq.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mf.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hh.shxzskj.cn

[D26] 数组转字符串
来源：http://kp.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://ks.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://xa.szsharing.cn

JS:   arr.join(", ")
来源：http://be.colortex.cn

TS:   arr.join(", ")
来源：http://cr.hahajie.cn

Java: String.join(", ", list)
来源：http://lw.lnxyls.cn

Go:   strings.Join(strs, ", ")
来源：http://xc.chemitech.net.cn

Ruby: arr.join(", ")
来源：http://dm.colortex.cn

C#:   string.Join(", ", list)
来源：http://jw.9csxet.cn

================================================================================
来源：http://wg.muxihuayi.cn

E. 字符串处理
来源：http://ij.shtwfgs.cn

================================================================================
来源：http://bp.jctech888.com.cn

[E01] 拼接字符串
来源：http://qq.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xa.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ne.nszjky.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://na.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bs.521024.cn


<!-- 参考信息 -->