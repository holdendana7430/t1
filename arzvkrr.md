代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://yo.jctech888.com.cn

TS:   export function f(): void {};  import { f } from "./m";
来源：http://mt.bjjhwx.cn

Java: import java.util.List;
来源：http://dg.huanxung.cn

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://xk.jctech888.com.cn

Ruby: require "json"; require_relative "./util"
来源：http://ji.9csxet.cn

C#:   using System.Text;
来源：http://nl.wgjwhj.cn

[C12] 立即执行函数 IIFE
来源：http://re.asd995.cn

Py:   (lambda: print("run"))()
来源：http://zq.gzmigu.cn

PHP:  (function () { echo "run"; })();
来源：http://td.bjjhwx.cn

JS:   (() => { console.log("run"); })();
来源：http://bi.bjjhwx.cn

TS:   (() => { console.log("run"); })();
来源：http://ip.huanxung.cn

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://bq.521024.cn

Go:   func() { fmt.Println("run") }()
来源：http://nh.nicolike.cn

Ruby: -> { puts "run" }.call
来源：http://lv.szsharing.cn

C#:   // 无 IIFE：用静态构造函数
来源：http://qs.hahajie.cn

[C13] 类型声明 / 类型注解
来源：http://hg.hnjuh.cn

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://qi.newstarts.cn

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://np.bjjhwx.cn

JS:   // 无类型（可用 JSDoc 注释）
来源：http://wd.huixiangedu.cn

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://ik.muxihuayi.cn

Java: int add(int a, int b) { return a + b; }
来源：http://jh.shxzskj.cn

Go:   func add(a, b int) int
来源：http://js.asd995.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://en.521024.cn

C#:   int Add(int a, int b) => a + b;
来源：http://rq.hahajie.cn

[C14] 泛型函数
来源：http://jd.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://zx.szxytkj.cn

PHP:  // 无泛型
来源：http://hw.jianghongdianzi.cn

JS:   // 无泛型
来源：http://bh.szsharing.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://uu.yuntaijiaju.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://zo.newstarts.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://ke.gzmigu.cn

Ruby: # 无泛型
来源：http://rn.hahajie.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://xc.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://zn.asd995.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://wh.bjjhwx.cn

PHP:  [$a, $b] = $pair;
来源：http://yi.jianghongdianzi.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://md.nicolike.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://pv.hahajie.cn

Java: // 无解构
来源：http://ye.szsharing.cn

Go:   // 无解构
来源：http://bv.colortex.cn

Ruby: a, b = pair
来源：http://yb.asd995.cn

C#:   var (a, b) = pair;
来源：http://rp.haigaiapp.cn

[C16] 函数 / 方法重载
来源：http://gw.wgjwhj.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qe.gzmigu.cn

PHP:  // 无重载
来源：http://yj.jctech888.com.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://jy.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://dw.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://bv.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://ay.shtwfgs.cn

Ruby: # 无重载：靠动态参数
来源：http://tc.gzmigu.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rg.lnxyls.cn

================================================================================
来源：http://uk.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://zr.shxzskj.cn

================================================================================
来源：http://ck.newstarts.cn

[D01] 创建数组 / 列表
来源：http://qz.shxzukj.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ja.huanxung.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://pk.bjjhwx.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://vm.panjiajie.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://tn.huixinmuqiang.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://mw.shtwfgs.cn

Go:   arr := []int{1, 2, 3}
来源：http://gb.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://xd.hnjuh.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://de.gzmigu.cn

[D02] 追加元素到末尾
来源：http://th.asd995.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ox.chemitech.net.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://vu.jctech888.com.cn

JS:   arr.push(4);
来源：http://gs.nszjky.cn

TS:   arr.push(4);
来源：http://xf.shxzukj.cn

Java: list.add(4);
来源：http://ed.chemitech.net.cn

Go:   arr = append(arr, 4)
来源：http://wb.yuexingan06.cn

Ruby: arr << 4; arr.push(5)
来源：http://zn.huanxung.cn

C#:   list.Add(4);
来源：http://lu.huixinmuqiang.cn

[D03] 在指定位置插入元素
来源：http://rq.lnxyls.cn

Py:   arr.insert(0, 0)
来源：http://ri.wgjwhj.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://zf.panjiajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cs.haigaiapp.cn

TS:   arr.splice(0, 0, 0);
来源：http://tx.panjiajie.cn

Java: list.add(0, 0);
来源：http://ci.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://yt.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://ve.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://ig.huixinmuqiang.cn

[D04] 删除元素
来源：http://vz.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://lv.yuntaijiaju.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ul.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://am.haigaiapp.cn

TS:   arr.splice(0, 1);
来源：http://ep.9csxet.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://dc.yuexingan06.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://pc.szxytkj.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://qe.bjjhwx.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ey.lnxyls.cn

[D05] 访问与修改元素
来源：http://ts.wgjwhj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ji.yuntaijiaju.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ze.panjiajie.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://kj.9csxet.cn

TS:   arr[0]; arr.at(-1);
来源：http://lz.gzmigu.cn

Java: list.get(0); list.set(0, 9);
来源：http://pp.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://fo.hnjuh.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://oh.szsharing.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://sm.lnxyls.cn

[D06] 数组长度
来源：http://ls.yuntaijiaju.cn

Py:   len(arr)
来源：http://ib.jctech888.com.cn

PHP:  count($arr);
来源：http://ii.newstarts.cn

JS:   arr.length
来源：http://pt.newstarts.cn

TS:   arr.length
来源：http://ft.colortex.cn

Java: list.size();
来源：http://hy.haigaiapp.cn

Go:   len(arr)
来源：http://oa.bookmarksfly.cn

Ruby: arr.length; arr.size
来源：http://ku.jianghongdianzi.cn

C#:   list.Count;
来源：http://pp.9csxet.cn

[D07] 切片 / 取子数组
来源：http://ot.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://zi.huixiangedu.cn

PHP:  array_slice($arr, 1, 3);
来源：http://md.asd995.cn

JS:   arr.slice(1, 4);
来源：http://xa.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://pw.wgjwhj.cn

Java: list.subList(1, 4);
来源：http://sf.nicolike.cn

Go:   arr[1:4]
来源：http://ew.jianghongdianzi.cn

Ruby: arr[1, 3]
来源：http://ot.shxzskj.cn

C#:   list.GetRange(1, 3);
来源：http://xs.asd995.cn

[D08] 合并两个数组
来源：http://fd.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://gp.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://sa.yuexingan06.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://op.jctech888.com.cn

TS:   [...a, ...b];
来源：http://ys.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://xh.huixinmuqiang.cn

Go:   append(a, b...)
来源：http://at.huixiangedu.cn

Ruby: a + b;  a.concat(b)
来源：http://io.jctech888.com.cn

C#:   a.Concat(b).ToList()
来源：http://ek.szsharing.cn

[D09] 排序（升序）
来源：http://ia.haigaiapp.cn

Py:   sorted(arr);  arr.sort()
来源：http://oy.jianghongdianzi.cn

PHP:  sort($arr);
来源：http://fs.jianghongdianzi.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://po.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sm.yuexingan06.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://qh.huanxung.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qe.panjiajie.cn

Ruby: arr.sort
来源：http://yk.haigaiapp.cn

C#:   list.Sort();
来源：http://gb.shxzskj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://bd.bjjhwx.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zw.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rx.bjjhwx.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dd.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://ta.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://uv.wgjwhj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://px.chemitech.net.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://pz.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yb.hahajie.cn

[D11] 反转数组
来源：http://wx.jctech888.com.cn

Py:   arr[::-1];  arr.reverse()
来源：http://iu.yuntaijiaju.cn

PHP:  array_reverse($arr);
来源：http://fs.haigaiapp.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mk.huanxung.cn

TS:   [...arr].reverse();
来源：http://ka.colortex.cn

Java: Collections.reverse(list);
来源：http://cs.9csxet.cn

Go:   slices.Reverse(arr)
来源：http://mz.colortex.cn

Ruby: arr.reverse
来源：http://fc.huanxung.cn

C#:   list.Reverse();
来源：http://wh.yuexingan06.cn

[D12] 查找元素下标
来源：http://ga.panjiajie.cn

Py:   arr.index(x);  x in arr
来源：http://ok.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://cm.shxzskj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ca.lnxyls.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://um.muxihuayi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://da.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://mp.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ck.panjiajie.cn

C#:   list.IndexOf(x);
来源：http://qn.nicolike.cn

[D13] 过滤（保留满足条件的）
来源：http://wr.wgjwhj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zw.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://af.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://ck.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://nw.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://pj.shtwfgs.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ru.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://im.lnxyls.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fh.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ht.jianghongdianzi.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://cp.bookmarksfly.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ga.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://br.huixinmuqiang.cn

TS:   arr.map(x => x * 2)
来源：http://pr.yuexingan06.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hj.huixiangedu.cn

Go:   // 手写循环
来源：http://kn.wgjwhj.cn

Ruby: arr.map { |x| x * 2 }
来源：http://os.yuexingan06.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://xl.shxzukj.cn

[D15] 去重
来源：http://kf.shxzukj.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hx.nicolike.cn

PHP:  array_unique($arr);
来源：http://yh.colortex.cn

JS:   [...new Set(arr)]
来源：http://tt.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://wn.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ho.nicolike.cn

Go:   // 用 map[T]struct{} 手写
来源：http://cg.nszjky.cn

Ruby: arr.uniq
来源：http://tm.yuntaijiaju.cn

C#:   list.Distinct().ToList()
来源：http://le.shtwfgs.cn

[D16] 求和与平均值
来源：http://co.nszjky.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://qb.huixiangedu.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://bv.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://qy.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ww.bjjhwx.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://eh.asd995.cn

Go:   // 手写循环累加
来源：http://ws.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wd.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://rj.hahajie.cn

[D17] 最大值与最小值
来源：http://uc.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://qh.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://uq.panjiajie.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://am.nicolike.cn

TS:   Math.max(...arr);
来源：http://qb.lnxyls.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ji.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wv.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://aw.521024.cn

C#:   list.Max();  list.Min()
来源：http://ge.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://yv.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://un.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://cc.yuntaijiaju.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ub.jctech888.com.cn

TS:   nested.flat();
来源：http://zm.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://df.yuexingan06.cn

Go:   // 手写双层循环
来源：http://cw.chemitech.net.cn

Ruby: nested.flatten
来源：http://de.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://jz.shxzskj.cn

[D19] 按字段分组
来源：http://ys.521024.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ra.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mp.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://du.colortex.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ib.haigaiapp.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vv.asd995.cn

Go:   // 手写 map[string][]T
来源：http://sc.yuexingan06.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ub.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gr.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://hz.bookmarksfly.cn

Py:   Counter(arr)
来源：http://aq.huanxung.cn

PHP:  array_count_values($arr);
来源：http://to.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sf.huanxung.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xm.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uh.521024.cn

Go:   // 手写 map[T]int
来源：http://xz.hahajie.cn

Ruby: arr.tally
来源：http://me.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ct.wgjwhj.cn

[D21] 判断是否包含某元素
来源：http://uz.haigaiapp.cn

Py:   x in arr
来源：http://co.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://uy.huixiangedu.cn

JS:   arr.includes(x)
来源：http://sr.bjjhwx.cn

TS:   arr.includes(x)
来源：http://wt.nicolike.cn

Java: list.contains(x)
来源：http://py.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://qy.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://rm.nicolike.cn

C#:   list.Contains(x)
来源：http://fa.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://sl.jctech888.com.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qh.9csxet.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xp.lnxyls.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ns.colortex.cn

TS:   [...arr];
来源：http://lz.wgjwhj.cn

Java: new ArrayList<>(list);
来源：http://hq.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mg.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://el.shxzskj.cn

C#:   new List<int>(list);
来源：http://bp.yuexingan06.cn

[D23] reduce 累积计算
来源：http://mf.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://fq.shxzskj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://lo.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qy.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rx.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://he.colortex.cn

Go:   // 手写循环
来源：http://uw.nszjky.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://me.bjjhwx.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qi.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://xp.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://yu.hahajie.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://bx.gzmigu.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qf.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kv.lnxyls.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uc.szsharing.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rg.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bi.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wu.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://sp.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jo.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://oi.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ee.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rt.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hn.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ci.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://px.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wn.szxytkj.cn

[D26] 数组转字符串
来源：http://vw.9csxet.cn

Py:   ", ".join(map(str, arr))
来源：http://sj.szsharing.cn

PHP:  implode(", ", $arr);
来源：http://rh.9csxet.cn

JS:   arr.join(", ")
来源：http://cq.wgjwhj.cn

TS:   arr.join(", ")
来源：http://kl.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ao.yuexingan06.cn

Go:   strings.Join(strs, ", ")
来源：http://ft.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://hd.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://ny.9csxet.cn

================================================================================
来源：http://th.szsharing.cn

E. 字符串处理
来源：http://fp.yuntaijiaju.cn

================================================================================
来源：http://sk.colortex.cn

[E01] 拼接字符串
来源：http://rg.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://he.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yu.nicolike.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://zc.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wb.panjiajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zb.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://fm.shxzukj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gl.yuntaijiaju.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://cw.lnxyls.cn


<!-- 参考信息 -->