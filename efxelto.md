代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://zq.jctech888.com.cn

Go:   func add(a, b int) int
来源：http://di.jianghongdianzi.cn

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://ic.asd995.cn

C#:   int Add(int a, int b) => a + b;
来源：http://aa.muxihuayi.cn

[C14] 泛型函数
来源：http://ha.newstarts.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://sf.asd995.cn

PHP:  // 无泛型
来源：http://yi.nszjky.cn

JS:   // 无泛型
来源：http://xr.yuntaijiaju.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://pu.hnjuh.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://rg.jianghongdianzi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://vy.shxzskj.cn

Ruby: # 无泛型
来源：http://zb.shxzskj.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://vn.jianghongdianzi.cn

[C15] 解构 / 展开参数
来源：http://pa.shtwfgs.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://gx.haigaiapp.cn

PHP:  [$a, $b] = $pair;
来源：http://rv.panjiajie.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://gq.wgjwhj.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://fr.asd995.cn

Java: // 无解构
来源：http://zo.yuexingan06.cn

Go:   // 无解构
来源：http://ic.hnjuh.cn

Ruby: a, b = pair
来源：http://lu.jianghongdianzi.cn

C#:   var (a, b) = pair;
来源：http://kc.huixiangedu.cn

[C16] 函数 / 方法重载
来源：http://kj.bookmarksfly.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://vr.521024.cn

PHP:  // 无重载
来源：http://se.szsharing.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://ol.shtwfgs.cn

TS:   // 用联合类型或重载签名声明
来源：http://iu.huixinmuqiang.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://hj.shtwfgs.cn

Go:   // 无重载：用不同函数名
来源：http://xy.haigaiapp.cn

Ruby: # 无重载：靠动态参数
来源：http://qj.bookmarksfly.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://mc.lnxyls.cn

================================================================================
来源：http://cb.wgjwhj.cn

D. 数组 / 列表 / 集合
来源：http://qr.hahajie.cn

================================================================================
来源：http://mw.521024.cn

[D01] 创建数组 / 列表
来源：http://yu.huixinmuqiang.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://zi.chemitech.net.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://vw.jctech888.com.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://px.haigaiapp.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://kt.huanxung.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://un.huixinmuqiang.cn

Go:   arr := []int{1, 2, 3}
来源：http://oo.szxytkj.cn

Ruby: arr = [1, 2, 3]
来源：http://un.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ka.haigaiapp.cn

[D02] 追加元素到末尾
来源：http://ov.huixiangedu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ug.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://bc.panjiajie.cn

JS:   arr.push(4);
来源：http://pk.jctech888.com.cn

TS:   arr.push(4);
来源：http://qx.shxzskj.cn

Java: list.add(4);
来源：http://rg.nicolike.cn

Go:   arr = append(arr, 4)
来源：http://zq.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://xp.huixinmuqiang.cn

C#:   list.Add(4);
来源：http://uw.asd995.cn

[D03] 在指定位置插入元素
来源：http://pu.huixiangedu.cn

Py:   arr.insert(0, 0)
来源：http://cl.shtwfgs.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://vp.muxihuayi.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://dk.521024.cn

TS:   arr.splice(0, 0, 0);
来源：http://jw.9csxet.cn

Java: list.add(0, 0);
来源：http://vv.yuntaijiaju.cn

Go:   arr = append([]int{0}, arr...)
来源：http://vl.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vn.huixinmuqiang.cn

C#:   list.Insert(0, 0);
来源：http://oi.gzmigu.cn

[D04] 删除元素
来源：http://fr.asd995.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sz.haigaiapp.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://ta.wgjwhj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://ph.jianghongdianzi.cn

TS:   arr.splice(0, 1);
来源：http://fn.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://oy.haigaiapp.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://oa.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://tz.panjiajie.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://vw.shtwfgs.cn

[D05] 访问与修改元素
来源：http://zc.521024.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gx.panjiajie.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ah.bookmarksfly.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://gc.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://ut.hahajie.cn

Java: list.get(0); list.set(0, 9);
来源：http://ni.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://xp.nszjky.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://pw.shxzukj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://by.yuexingan06.cn

[D06] 数组长度
来源：http://wy.bookmarksfly.cn

Py:   len(arr)
来源：http://fh.lnxyls.cn

PHP:  count($arr);
来源：http://pe.shtwfgs.cn

JS:   arr.length
来源：http://bj.bookmarksfly.cn

TS:   arr.length
来源：http://yc.shtwfgs.cn

Java: list.size();
来源：http://ny.szxytkj.cn

Go:   len(arr)
来源：http://nc.shxzskj.cn

Ruby: arr.length; arr.size
来源：http://wb.521024.cn

C#:   list.Count;
来源：http://ok.nszjky.cn

[D07] 切片 / 取子数组
来源：http://ca.521024.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ye.hnjuh.cn

PHP:  array_slice($arr, 1, 3);
来源：http://dd.nicolike.cn

JS:   arr.slice(1, 4);
来源：http://pn.szsharing.cn

TS:   arr.slice(1, 4);
来源：http://hd.shxzskj.cn

Java: list.subList(1, 4);
来源：http://kj.lnxyls.cn

Go:   arr[1:4]
来源：http://mc.bookmarksfly.cn

Ruby: arr[1, 3]
来源：http://oc.huixiangedu.cn

C#:   list.GetRange(1, 3);
来源：http://ad.bjjhwx.cn

[D08] 合并两个数组
来源：http://km.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://ub.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://zd.yuntaijiaju.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://gc.bjjhwx.cn

TS:   [...a, ...b];
来源：http://np.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ju.9csxet.cn

Go:   append(a, b...)
来源：http://jc.wgjwhj.cn

Ruby: a + b;  a.concat(b)
来源：http://lc.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://xs.bookmarksfly.cn

[D09] 排序（升序）
来源：http://hj.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://ay.szsharing.cn

PHP:  sort($arr);
来源：http://kb.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://jv.bookmarksfly.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://sk.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://hl.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://lo.haigaiapp.cn

Ruby: arr.sort
来源：http://lb.haigaiapp.cn

C#:   list.Sort();
来源：http://ld.9csxet.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ux.huixinmuqiang.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ee.nicolike.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://zv.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://eh.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fs.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://tx.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dx.huixiangedu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mr.szxytkj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uy.hahajie.cn

[D11] 反转数组
来源：http://wz.jianghongdianzi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://mp.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://tn.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://sv.shtwfgs.cn

TS:   [...arr].reverse();
来源：http://df.szsharing.cn

Java: Collections.reverse(list);
来源：http://rh.panjiajie.cn

Go:   slices.Reverse(arr)
来源：http://xr.szxytkj.cn

Ruby: arr.reverse
来源：http://pc.szsharing.cn

C#:   list.Reverse();
来源：http://qg.shtwfgs.cn

[D12] 查找元素下标
来源：http://he.hnjuh.cn

Py:   arr.index(x);  x in arr
来源：http://xy.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kz.shtwfgs.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://md.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zk.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ti.huanxung.cn

Go:   slices.Index(arr, x)
来源：http://du.huanxung.cn

Ruby: arr.index(x)
来源：http://if.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://md.nszjky.cn

[D13] 过滤（保留满足条件的）
来源：http://jq.hnjuh.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ei.9csxet.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ix.huanxung.cn

JS:   arr.filter(x => x > 3)
来源：http://cw.hahajie.cn

TS:   arr.filter(x => x > 3)
来源：http://qx.bookmarksfly.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lr.panjiajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qb.huixinmuqiang.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ca.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://sb.muxihuayi.cn

[D14] 映射转换（每个元素变形）
来源：http://my.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://od.yuntaijiaju.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jw.lnxyls.cn

JS:   arr.map(x => x * 2)
来源：http://bf.jctech888.com.cn

TS:   arr.map(x => x * 2)
来源：http://kf.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://zw.lnxyls.cn

Go:   // 手写循环
来源：http://sb.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://gj.lnxyls.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ll.521024.cn

[D15] 去重
来源：http://ys.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://xx.shxzukj.cn

PHP:  array_unique($arr);
来源：http://lq.521024.cn

JS:   [...new Set(arr)]
来源：http://oz.521024.cn

TS:   [...new Set(arr)]
来源：http://ro.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://cm.yuexingan06.cn

Go:   // 用 map[T]struct{} 手写
来源：http://df.haigaiapp.cn

Ruby: arr.uniq
来源：http://sy.szsharing.cn

C#:   list.Distinct().ToList()
来源：http://br.bookmarksfly.cn

[D16] 求和与平均值
来源：http://zv.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uw.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iy.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dv.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vm.szsharing.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ex.bjjhwx.cn

Go:   // 手写循环累加
来源：http://gd.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hk.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://sb.hahajie.cn

[D17] 最大值与最小值
来源：http://uq.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://pj.muxihuayi.cn

PHP:  max($arr);  min($arr);
来源：http://ll.colortex.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://iq.muxihuayi.cn

TS:   Math.max(...arr);
来源：http://iq.yuexingan06.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mx.jianghongdianzi.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rj.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ok.nszjky.cn

C#:   list.Max();  list.Min()
来源：http://gk.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://ib.nicolike.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://dg.yuntaijiaju.cn

PHP:  array_merge(...$nested);
来源：http://zn.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://gz.hahajie.cn

TS:   nested.flat();
来源：http://kf.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fk.muxihuayi.cn

Go:   // 手写双层循环
来源：http://ui.haigaiapp.cn

Ruby: nested.flatten
来源：http://yz.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://iy.9csxet.cn

[D19] 按字段分组
来源：http://ed.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ys.bjjhwx.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://jb.gzmigu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ta.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vy.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ly.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://ms.shxzukj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wx.bjjhwx.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hn.huixinmuqiang.cn

[D20] 统计每个元素出现次数
来源：http://ic.newstarts.cn

Py:   Counter(arr)
来源：http://of.nicolike.cn

PHP:  array_count_values($arr);
来源：http://bh.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lp.muxihuayi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dv.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://na.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://ij.newstarts.cn

Ruby: arr.tally
来源：http://ye.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://na.szxytkj.cn

[D21] 判断是否包含某元素
来源：http://fn.huixiangedu.cn

Py:   x in arr
来源：http://cp.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://su.szsharing.cn

JS:   arr.includes(x)
来源：http://bk.jctech888.com.cn

TS:   arr.includes(x)
来源：http://gz.asd995.cn

Java: list.contains(x)
来源：http://eo.jctech888.com.cn

Go:   slices.Contains(arr, x)
来源：http://ff.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://as.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://cx.chemitech.net.cn

[D22] 复制数组（避免共享引用）
来源：http://kp.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yi.hahajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ok.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ab.bookmarksfly.cn

TS:   [...arr];
来源：http://ry.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://vn.yuntaijiaju.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ww.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://rt.panjiajie.cn

C#:   new List<int>(list);
来源：http://bs.nicolike.cn

[D23] reduce 累积计算
来源：http://ag.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gt.nszjky.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hi.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sn.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ia.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://fo.9csxet.cn

Go:   // 手写循环
来源：http://gf.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://se.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vg.9csxet.cn

[D24] 字典 / Map 基本操作
来源：http://vc.hahajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pf.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://il.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nd.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ac.521024.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qt.asd995.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://qp.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tb.asd995.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ym.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://nh.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://qf.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://vx.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xc.panjiajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ag.hahajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yf.521024.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sx.bjjhwx.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gw.gzmigu.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qk.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ht.lnxyls.cn

Py:   ", ".join(map(str, arr))
来源：http://mr.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://gx.nszjky.cn

JS:   arr.join(", ")
来源：http://qs.yuntaijiaju.cn

TS:   arr.join(", ")
来源：http://el.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://in.shtwfgs.cn

Go:   strings.Join(strs, ", ")
来源：http://xn.huixinmuqiang.cn

Ruby: arr.join(", ")
来源：http://lq.9csxet.cn

C#:   string.Join(", ", list)
来源：http://qc.huanxung.cn

================================================================================
来源：http://ps.haigaiapp.cn

E. 字符串处理
来源：http://en.szxytkj.cn

================================================================================
来源：http://um.newstarts.cn

[E01] 拼接字符串
来源：http://ql.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://eb.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://om.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://om.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jo.gzmigu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://uu.jctech888.com.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ct.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wb.jctech888.com.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://no.gzmigu.cn

[E02] 重复字符串
来源：http://uf.haigaiapp.cn

Py:   "ab" * 3
来源：http://ad.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://mf.nszjky.cn

JS:   "ab".repeat(3)
来源：http://br.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://et.newstarts.cn

Java: "ab".repeat(3)
来源：http://ly.huixinmuqiang.cn

Go:   strings.Repeat("ab", 3)
来源：http://td.huanxung.cn

Ruby: "ab" * 3
来源：http://nl.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yu.huixinmuqiang.cn

[E03] 截取子串
来源：http://wj.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hy.nszjky.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cu.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ws.panjiajie.cn

TS:   s.slice(1, 4)
来源：http://rf.521024.cn

Java: s.substring(1, 4)
来源：http://ea.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ez.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ke.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://mq.9csxet.cn

[E04] 查找子串位置
来源：http://em.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://ck.panjiajie.cn


<!-- 参考信息 -->