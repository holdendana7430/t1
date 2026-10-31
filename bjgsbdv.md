代发 wailian999

TS:   同 JS
来源：http://dn.newstarts.cn

Java: 方法内为块级作用域
来源：http://aa.bookmarksfly.cn

Go:   花括号块级作用域
来源：http://if.lnxyls.cn

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://df.jctech888.com.cn

C#:   块级作用域
来源：http://du.haigaiapp.cn

[C11] 模块导入与导出
来源：http://os.hnjuh.cn

Py:   from module import func
来源：http://gg.hahajie.cn

PHP:  require "file.php";  或 use App\Service;
来源：http://ay.huixiangedu.cn

JS:   export default function f() {};  import f from "./m.js";
来源：http://bt.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://yb.haigaiapp.cn

Java: import java.util.List;
来源：http://pr.chemitech.net.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://lu.9csxet.cn

Ruby: require "json"; require_relative "./util"
来源：http://tu.panjiajie.cn

C#:   using System.Text;
来源：http://zl.bookmarksfly.cn

[C12] 立即执行函数 IIFE
来源：http://xd.hnjuh.cn

Py:   (lambda: print("run"))()
来源：http://be.9csxet.cn

PHP:  (function () { echo "run"; })();
来源：http://wr.521024.cn

JS:   (() => { console.log("run"); })();
来源：http://wp.szsharing.cn

TS:   (() => { console.log("run"); })();
来源：http://wr.gzmigu.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://tl.newstarts.cn

Go:   func() { fmt.Println("run") }()
来源：http://qq.newstarts.cn

Ruby: -> { puts "run" }.call
来源：http://hj.gzmigu.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://bt.bjjhwx.cn

[C13] 类型声明 / 类型注解
来源：http://pv.nszjky.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://os.9csxet.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://uu.nicolike.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://cs.shxzskj.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://sc.bookmarksfly.cn

Java: int add(int a, int b) { return a + b; }
来源：http://xr.haigaiapp.cn

Go:   func add(a, b int) int
来源：http://ik.shtwfgs.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://tx.shxzskj.cn

C#:   int Add(int a, int b) => a + b;
来源：http://gj.gzmigu.cn

[C14] 泛型函数
来源：http://ex.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://au.lnxyls.cn

PHP:  // 无泛型
来源：http://zq.hnjuh.cn

JS:   // 无泛型
来源：http://hy.huixiangedu.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://fa.haigaiapp.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://oz.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ji.521024.cn

Ruby: # 无泛型
来源：http://ua.nszjky.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://qv.yuntaijiaju.cn

[C15] 解构 / 展开参数
来源：http://ob.shxzukj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://us.yuntaijiaju.cn

PHP:  [$a, $b] = $pair;
来源：http://xg.hahajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://fy.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://jb.shtwfgs.cn

Java: // 无解构
来源：http://cb.shtwfgs.cn

Go:   // 无解构
来源：http://av.shxzukj.cn

Ruby: a, b = pair
来源：http://ab.huixiangedu.cn

C#:   var (a, b) = pair;
来源：http://vk.gzmigu.cn

[C16] 函数 / 方法重载
来源：http://fw.yuntaijiaju.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qh.muxihuayi.cn

PHP:  // 无重载
来源：http://mz.jianghongdianzi.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://gm.jctech888.com.cn

TS:   // 用联合类型或重载签名声明
来源：http://be.yuexingan06.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://er.lnxyls.cn

Go:   // 无重载：用不同函数名
来源：http://yh.yuntaijiaju.cn

Ruby: # 无重载：靠动态参数
来源：http://xf.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://to.huixinmuqiang.cn

================================================================================
来源：http://it.521024.cn

D. 数组 / 列表 / 集合
来源：http://rx.gzmigu.cn

================================================================================
来源：http://aa.521024.cn

[D01] 创建数组 / 列表
来源：http://id.asd995.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://jj.szsharing.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://uz.asd995.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://gn.nszjky.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pi.9csxet.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://ou.bjjhwx.cn

Go:   arr := []int{1, 2, 3}
来源：http://ii.9csxet.cn

Ruby: arr = [1, 2, 3]
来源：http://dg.hahajie.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sw.szsharing.cn

[D02] 追加元素到末尾
来源：http://dv.chemitech.net.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://wj.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://la.lnxyls.cn

JS:   arr.push(4);
来源：http://hs.hnjuh.cn

TS:   arr.push(4);
来源：http://ut.huanxung.cn

Java: list.add(4);
来源：http://ic.szsharing.cn

Go:   arr = append(arr, 4)
来源：http://om.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://zu.szxytkj.cn

C#:   list.Add(4);
来源：http://nr.lnxyls.cn

[D03] 在指定位置插入元素
来源：http://ys.chemitech.net.cn

Py:   arr.insert(0, 0)
来源：http://vh.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vt.jctech888.com.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://ky.wgjwhj.cn

TS:   arr.splice(0, 0, 0);
来源：http://jm.newstarts.cn

Java: list.add(0, 0);
来源：http://yu.yuexingan06.cn

Go:   arr = append([]int{0}, arr...)
来源：http://wi.yuntaijiaju.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vj.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://au.hnjuh.cn

[D04] 删除元素
来源：http://xv.shxzskj.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ub.huixinmuqiang.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wg.gzmigu.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://zb.nszjky.cn

TS:   arr.splice(0, 1);
来源：http://qh.wgjwhj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://kd.521024.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://nz.jctech888.com.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://lo.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ru.lnxyls.cn

[D05] 访问与修改元素
来源：http://ld.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://zj.jianghongdianzi.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://cy.chemitech.net.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://vm.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://qn.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://yf.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://wq.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nw.jianghongdianzi.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://px.huixiangedu.cn

[D06] 数组长度
来源：http://ph.jianghongdianzi.cn

Py:   len(arr)
来源：http://tq.bookmarksfly.cn

PHP:  count($arr);
来源：http://ax.wgjwhj.cn

JS:   arr.length
来源：http://io.bjjhwx.cn

TS:   arr.length
来源：http://kt.muxihuayi.cn

Java: list.size();
来源：http://ns.panjiajie.cn

Go:   len(arr)
来源：http://sz.szxytkj.cn

Ruby: arr.length; arr.size
来源：http://wo.hnjuh.cn

C#:   list.Count;
来源：http://pb.panjiajie.cn

[D07] 切片 / 取子数组
来源：http://yd.asd995.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://wx.9csxet.cn

PHP:  array_slice($arr, 1, 3);
来源：http://bw.bjjhwx.cn

JS:   arr.slice(1, 4);
来源：http://lp.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://rx.nicolike.cn

Java: list.subList(1, 4);
来源：http://wt.shtwfgs.cn

Go:   arr[1:4]
来源：http://gk.shxzskj.cn

Ruby: arr[1, 3]
来源：http://zt.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://vz.huixiangedu.cn

[D08] 合并两个数组
来源：http://kc.chemitech.net.cn

Py:   a + b;  a.extend(b)
来源：http://eo.shxzukj.cn

PHP:  array_merge($a, $b);
来源：http://sz.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sn.nicolike.cn

TS:   [...a, ...b];
来源：http://wg.muxihuayi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://qf.newstarts.cn

Go:   append(a, b...)
来源：http://sh.nszjky.cn

Ruby: a + b;  a.concat(b)
来源：http://cc.nicolike.cn

C#:   a.Concat(b).ToList()
来源：http://ai.szsharing.cn

[D09] 排序（升序）
来源：http://us.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://fw.521024.cn

PHP:  sort($arr);
来源：http://ni.newstarts.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wg.lnxyls.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cy.panjiajie.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://kl.asd995.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ao.huixiangedu.cn

Ruby: arr.sort
来源：http://st.lnxyls.cn

C#:   list.Sort();
来源：http://oc.szsharing.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://lj.gzmigu.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://aj.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rj.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://xk.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://bn.521024.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://qh.jctech888.com.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yy.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rf.wgjwhj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ne.nicolike.cn

[D11] 反转数组
来源：http://ek.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://rc.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://kn.hahajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://dp.huanxung.cn

TS:   [...arr].reverse();
来源：http://ag.521024.cn

Java: Collections.reverse(list);
来源：http://iy.muxihuayi.cn

Go:   slices.Reverse(arr)
来源：http://xv.newstarts.cn

Ruby: arr.reverse
来源：http://ja.bookmarksfly.cn

C#:   list.Reverse();
来源：http://ly.bjjhwx.cn

[D12] 查找元素下标
来源：http://wm.shxzskj.cn

Py:   arr.index(x);  x in arr
来源：http://do.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://qb.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://go.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://er.huixiangedu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://dl.colortex.cn

Go:   slices.Index(arr, x)
来源：http://cv.521024.cn

Ruby: arr.index(x)
来源：http://tk.hahajie.cn

C#:   list.IndexOf(x);
来源：http://mo.bookmarksfly.cn

[D13] 过滤（保留满足条件的）
来源：http://rs.nszjky.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://cq.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://jg.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://fo.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://nw.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ia.jianghongdianzi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lo.jianghongdianzi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://px.muxihuayi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gy.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://mk.lnxyls.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qw.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jx.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://zr.yuntaijiaju.cn

TS:   arr.map(x => x * 2)
来源：http://cd.muxihuayi.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://va.bjjhwx.cn

Go:   // 手写循环
来源：http://ni.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hy.huixinmuqiang.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ha.yuntaijiaju.cn

[D15] 去重
来源：http://gq.shxzskj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fv.nicolike.cn

PHP:  array_unique($arr);
来源：http://hh.yuntaijiaju.cn

JS:   [...new Set(arr)]
来源：http://sp.asd995.cn

TS:   [...new Set(arr)]
来源：http://iv.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wz.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wm.asd995.cn

Ruby: arr.uniq
来源：http://dm.asd995.cn

C#:   list.Distinct().ToList()
来源：http://yv.wgjwhj.cn

[D16] 求和与平均值
来源：http://vc.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://fw.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ac.nicolike.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bb.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jr.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://bf.yuexingan06.cn

Go:   // 手写循环累加
来源：http://ei.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hb.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://ho.asd995.cn

[D17] 最大值与最小值
来源：http://em.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://bz.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://kd.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://rd.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://bx.huixinmuqiang.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mh.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://jr.shxzskj.cn

Ruby: arr.max;  arr.min
来源：http://lp.huixinmuqiang.cn

C#:   list.Max();  list.Min()
来源：http://yz.gzmigu.cn

[D18] 扁平化嵌套数组
来源：http://qb.chemitech.net.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ph.yuexingan06.cn

PHP:  array_merge(...$nested);
来源：http://cp.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wz.shxzskj.cn

TS:   nested.flat();
来源：http://di.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hx.szxytkj.cn

Go:   // 手写双层循环
来源：http://bn.wgjwhj.cn

Ruby: nested.flatten
来源：http://jz.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://za.bjjhwx.cn

[D19] 按字段分组
来源：http://ca.colortex.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://nq.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zv.bjjhwx.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://lk.shxzskj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ni.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ds.newstarts.cn

Go:   // 手写 map[string][]T
来源：http://dc.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://px.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wd.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://rc.szsharing.cn

Py:   Counter(arr)
来源：http://lv.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://rm.szxytkj.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xq.szsharing.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bh.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://se.nszjky.cn

Go:   // 手写 map[T]int
来源：http://db.szxytkj.cn

Ruby: arr.tally
来源：http://ck.hnjuh.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://rt.szsharing.cn

[D21] 判断是否包含某元素
来源：http://kt.muxihuayi.cn

Py:   x in arr
来源：http://tp.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://ul.yuexingan06.cn

JS:   arr.includes(x)
来源：http://sl.shxzskj.cn

TS:   arr.includes(x)
来源：http://vj.lnxyls.cn

Java: list.contains(x)
来源：http://ab.9csxet.cn

Go:   slices.Contains(arr, x)
来源：http://bz.muxihuayi.cn

Ruby: arr.include?(x)
来源：http://vb.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://zt.shxzukj.cn

[D22] 复制数组（避免共享引用）
来源：http://wv.nszjky.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cg.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hh.szsharing.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://va.wgjwhj.cn

TS:   [...arr];
来源：http://ud.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://jd.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://nd.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://rp.hnjuh.cn

C#:   new List<int>(list);
来源：http://kj.shxzskj.cn

[D23] reduce 累积计算
来源：http://la.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://zn.huixiangedu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ea.bjjhwx.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vd.panjiajie.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ce.521024.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yo.gzmigu.cn

Go:   // 手写循环
来源：http://cm.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mt.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://oz.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://ak.szsharing.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mt.huanxung.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gv.szxytkj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gy.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wh.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://fg.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qq.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ep.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pn.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://ng.hnjuh.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://be.panjiajie.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://py.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ye.colortex.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yh.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ap.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://da.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://bz.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dz.chemitech.net.cn

[D26] 数组转字符串
来源：http://jw.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://aj.bjjhwx.cn

PHP:  implode(", ", $arr);
来源：http://lx.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://xm.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://mu.jctech888.com.cn

Java: String.join(", ", list)
来源：http://td.wgjwhj.cn

Go:   strings.Join(strs, ", ")
来源：http://nl.gzmigu.cn

Ruby: arr.join(", ")
来源：http://kf.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ne.wgjwhj.cn

================================================================================
来源：http://nf.chemitech.net.cn

E. 字符串处理
来源：http://az.szsharing.cn

================================================================================
来源：http://mi.colortex.cn

[E01] 拼接字符串
来源：http://ic.huixinmuqiang.cn


<!-- 参考信息 -->