代发 wailian999

[C14] 泛型函数
来源：http://me.shtwfgs.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://ax.colortex.cn

PHP:  // 无泛型
来源：http://zr.newstarts.cn

JS:   // 无泛型
来源：http://zq.521024.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://jo.jianghongdianzi.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://ab.muxihuayi.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://xb.jianghongdianzi.cn

Ruby: # 无泛型
来源：http://aa.jctech888.com.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://lz.huixinmuqiang.cn

[C15] 解构 / 展开参数
来源：http://zx.521024.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ql.gzmigu.cn

PHP:  [$a, $b] = $pair;
来源：http://gz.hnjuh.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://qr.colortex.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://ko.yuntaijiaju.cn

Java: // 无解构
来源：http://xn.shtwfgs.cn

Go:   // 无解构
来源：http://cq.chemitech.net.cn

Ruby: a, b = pair
来源：http://pw.panjiajie.cn

C#:   var (a, b) = pair;
来源：http://oo.asd995.cn

[C16] 函数 / 方法重载
来源：http://xv.huanxung.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://mi.wgjwhj.cn

PHP:  // 无重载
来源：http://ty.521024.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://qs.muxihuayi.cn

TS:   // 用联合类型或重载签名声明
来源：http://mv.colortex.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://ee.panjiajie.cn

Go:   // 无重载：用不同函数名
来源：http://js.chemitech.net.cn

Ruby: # 无重载：靠动态参数
来源：http://kk.hahajie.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://yr.szxytkj.cn

================================================================================
来源：http://nl.huanxung.cn

D. 数组 / 列表 / 集合
来源：http://xe.asd995.cn

================================================================================
来源：http://jf.lnxyls.cn

[D01] 创建数组 / 列表
来源：http://fi.hnjuh.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://tb.bjjhwx.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://tx.colortex.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://xh.szsharing.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://uo.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://wb.huixiangedu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ij.asd995.cn

Ruby: arr = [1, 2, 3]
来源：http://eo.bjjhwx.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://kn.nszjky.cn

[D02] 追加元素到末尾
来源：http://cm.colortex.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://qv.yuntaijiaju.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fc.szxytkj.cn

JS:   arr.push(4);
来源：http://aw.shtwfgs.cn

TS:   arr.push(4);
来源：http://pt.bjjhwx.cn

Java: list.add(4);
来源：http://ot.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://xz.hnjuh.cn

Ruby: arr << 4; arr.push(5)
来源：http://ye.shtwfgs.cn

C#:   list.Add(4);
来源：http://zo.muxihuayi.cn

[D03] 在指定位置插入元素
来源：http://wj.gzmigu.cn

Py:   arr.insert(0, 0)
来源：http://yw.nszjky.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://cp.shxzskj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://iy.gzmigu.cn

TS:   arr.splice(0, 0, 0);
来源：http://le.hahajie.cn

Java: list.add(0, 0);
来源：http://yq.bookmarksfly.cn

Go:   arr = append([]int{0}, arr...)
来源：http://tr.nszjky.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://vm.nszjky.cn

C#:   list.Insert(0, 0);
来源：http://pq.jctech888.com.cn

[D04] 删除元素
来源：http://cf.colortex.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://cb.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://xy.shxzskj.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pv.asd995.cn

TS:   arr.splice(0, 1);
来源：http://aa.bjjhwx.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bm.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://lx.newstarts.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ta.jctech888.com.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zb.huixinmuqiang.cn

[D05] 访问与修改元素
来源：http://xd.9csxet.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://eo.huixiangedu.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://ua.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ct.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://ci.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://ax.asd995.cn

Go:   arr[0]; arr[0] = 9
来源：http://uu.nicolike.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fz.huanxung.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://si.panjiajie.cn

[D06] 数组长度
来源：http://dc.jianghongdianzi.cn

Py:   len(arr)
来源：http://ub.chemitech.net.cn

PHP:  count($arr);
来源：http://dw.panjiajie.cn

JS:   arr.length
来源：http://vx.nicolike.cn

TS:   arr.length
来源：http://wy.huanxung.cn

Java: list.size();
来源：http://kq.huanxung.cn

Go:   len(arr)
来源：http://ju.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://ym.haigaiapp.cn

C#:   list.Count;
来源：http://iy.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://wv.bjjhwx.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://yw.szxytkj.cn

PHP:  array_slice($arr, 1, 3);
来源：http://fx.asd995.cn

JS:   arr.slice(1, 4);
来源：http://vu.bjjhwx.cn

TS:   arr.slice(1, 4);
来源：http://ps.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://gv.gzmigu.cn

Go:   arr[1:4]
来源：http://gy.huanxung.cn

Ruby: arr[1, 3]
来源：http://df.nicolike.cn

C#:   list.GetRange(1, 3);
来源：http://ci.newstarts.cn

[D08] 合并两个数组
来源：http://wg.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://fb.jianghongdianzi.cn

PHP:  array_merge($a, $b);
来源：http://ci.hnjuh.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ib.szxytkj.cn

TS:   [...a, ...b];
来源：http://cq.hahajie.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://to.shtwfgs.cn

Go:   append(a, b...)
来源：http://vw.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://dy.jianghongdianzi.cn

C#:   a.Concat(b).ToList()
来源：http://sv.jctech888.com.cn

[D09] 排序（升序）
来源：http://yu.jctech888.com.cn

Py:   sorted(arr);  arr.sort()
来源：http://im.521024.cn

PHP:  sort($arr);
来源：http://qp.nszjky.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://op.muxihuayi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ck.huixinmuqiang.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://xc.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bu.huixiangedu.cn

Ruby: arr.sort
来源：http://lu.shtwfgs.cn

C#:   list.Sort();
来源：http://dt.huanxung.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://re.nszjky.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://tt.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kd.yuexingan06.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://da.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://he.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wf.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://gv.shxzukj.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://lf.bookmarksfly.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wf.panjiajie.cn

[D11] 反转数组
来源：http://bj.lnxyls.cn

Py:   arr[::-1];  arr.reverse()
来源：http://hm.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://in.huixiangedu.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vz.nszjky.cn

TS:   [...arr].reverse();
来源：http://mp.nszjky.cn

Java: Collections.reverse(list);
来源：http://nf.huanxung.cn

Go:   slices.Reverse(arr)
来源：http://hr.yuexingan06.cn

Ruby: arr.reverse
来源：http://ow.shxzukj.cn

C#:   list.Reverse();
来源：http://ar.newstarts.cn

[D12] 查找元素下标
来源：http://wb.gzmigu.cn

Py:   arr.index(x);  x in arr
来源：http://vp.yuntaijiaju.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xp.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mx.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sg.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://gh.521024.cn

Go:   slices.Index(arr, x)
来源：http://hb.yuexingan06.cn

Ruby: arr.index(x)
来源：http://xt.wgjwhj.cn

C#:   list.IndexOf(x);
来源：http://me.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://ku.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://jl.nszjky.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dr.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://tj.jianghongdianzi.cn

TS:   arr.filter(x => x > 3)
来源：http://uy.lnxyls.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xm.wgjwhj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://gs.nicolike.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zp.nszjky.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://hb.wgjwhj.cn

[D14] 映射转换（每个元素变形）
来源：http://cb.panjiajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://kf.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://jr.shxzukj.cn

JS:   arr.map(x => x * 2)
来源：http://af.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://nh.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://dg.shtwfgs.cn

Go:   // 手写循环
来源：http://xf.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://at.9csxet.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://wa.shxzskj.cn

[D15] 去重
来源：http://bp.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://fo.hnjuh.cn

PHP:  array_unique($arr);
来源：http://uz.hnjuh.cn

JS:   [...new Set(arr)]
来源：http://dd.shxzukj.cn

TS:   [...new Set(arr)]
来源：http://dz.bjjhwx.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://re.jctech888.com.cn

Go:   // 用 map[T]struct{} 手写
来源：http://fx.shxzskj.cn

Ruby: arr.uniq
来源：http://oe.521024.cn

C#:   list.Distinct().ToList()
来源：http://dl.nicolike.cn

[D16] 求和与平均值
来源：http://wb.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jy.hahajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://uk.colortex.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dm.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://km.bookmarksfly.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://cn.lnxyls.cn

Go:   // 手写循环累加
来源：http://lp.szxytkj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tx.muxihuayi.cn

C#:   list.Sum();  list.Average()
来源：http://gs.jctech888.com.cn

[D17] 最大值与最小值
来源：http://jj.colortex.cn

Py:   max(arr);  min(arr)
来源：http://up.shxzskj.cn

PHP:  max($arr);  min($arr);
来源：http://as.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ug.huixinmuqiang.cn

TS:   Math.max(...arr);
来源：http://df.bookmarksfly.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ye.asd995.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://rc.9csxet.cn

Ruby: arr.max;  arr.min
来源：http://ss.lnxyls.cn

C#:   list.Max();  list.Min()
来源：http://mc.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://va.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ao.hahajie.cn

PHP:  array_merge(...$nested);
来源：http://ct.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://pk.hnjuh.cn

TS:   nested.flat();
来源：http://ga.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://sr.nszjky.cn

Go:   // 手写双层循环
来源：http://xq.shxzukj.cn

Ruby: nested.flatten
来源：http://jn.yuntaijiaju.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://pp.shxzukj.cn

[D19] 按字段分组
来源：http://gb.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hv.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hp.muxihuayi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vy.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://hn.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ej.jianghongdianzi.cn

Go:   // 手写 map[string][]T
来源：http://hp.huixiangedu.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://eo.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wg.huanxung.cn

[D20] 统计每个元素出现次数
来源：http://rw.wgjwhj.cn

Py:   Counter(arr)
来源：http://nl.nicolike.cn

PHP:  array_count_values($arr);
来源：http://po.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bm.panjiajie.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://zx.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cz.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://eg.nszjky.cn

Ruby: arr.tally
来源：http://sp.shxzukj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://zu.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://gq.haigaiapp.cn

Py:   x in arr
来源：http://ak.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://gw.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://uq.huixiangedu.cn

TS:   arr.includes(x)
来源：http://td.nszjky.cn

Java: list.contains(x)
来源：http://hi.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://qr.lnxyls.cn

Ruby: arr.include?(x)
来源：http://cn.shxzukj.cn

C#:   list.Contains(x)
来源：http://nu.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://qo.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://cz.muxihuayi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vn.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ib.shxzukj.cn

TS:   [...arr];
来源：http://bv.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://ox.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://mu.panjiajie.cn

Ruby: arr.dup;  arr.clone
来源：http://zd.szsharing.cn

C#:   new List<int>(list);
来源：http://dy.bookmarksfly.cn

[D23] reduce 累积计算
来源：http://ds.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xm.9csxet.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gy.shxzskj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mv.shxzskj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://jp.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yz.lnxyls.cn

Go:   // 手写循环
来源：http://gd.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qr.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://gi.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://gq.yuntaijiaju.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ao.szxytkj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hu.szsharing.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xm.gzmigu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ka.shxzukj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://dh.huixiangedu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ba.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qo.huixinmuqiang.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://np.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://ds.newstarts.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://pv.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://kd.szsharing.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bo.lnxyls.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xx.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lb.colortex.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://if.521024.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ef.hnjuh.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yu.bookmarksfly.cn

[D26] 数组转字符串
来源：http://ig.muxihuayi.cn

Py:   ", ".join(map(str, arr))
来源：http://dp.szxytkj.cn

PHP:  implode(", ", $arr);
来源：http://iy.bjjhwx.cn

JS:   arr.join(", ")
来源：http://gx.shxzskj.cn

TS:   arr.join(", ")
来源：http://wn.9csxet.cn

Java: String.join(", ", list)
来源：http://ms.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://ki.colortex.cn

Ruby: arr.join(", ")
来源：http://fp.huanxung.cn

C#:   string.Join(", ", list)
来源：http://uh.yuntaijiaju.cn

================================================================================
来源：http://eh.lnxyls.cn

E. 字符串处理
来源：http://dc.lnxyls.cn

================================================================================
来源：http://wp.gzmigu.cn

[E01] 拼接字符串
来源：http://ge.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://no.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://vs.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wt.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://xu.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ys.gzmigu.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://xb.colortex.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://od.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://bg.yuexingan06.cn

[E02] 重复字符串
来源：http://qh.szxytkj.cn

Py:   "ab" * 3
来源：http://zc.chemitech.net.cn

PHP:  str_repeat("ab", 3);
来源：http://zg.nicolike.cn

JS:   "ab".repeat(3)
来源：http://nn.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://wv.huixiangedu.cn

Java: "ab".repeat(3)
来源：http://ux.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://lz.hahajie.cn

Ruby: "ab" * 3
来源：http://ak.nicolike.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rb.haigaiapp.cn

[E03] 截取子串
来源：http://an.haigaiapp.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nt.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vd.hahajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://dr.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://hx.nicolike.cn

Java: s.substring(1, 4)
来源：http://hs.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://rz.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://jg.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://cq.shxzukj.cn

[E04] 查找子串位置
来源：http://op.gzmigu.cn

Py:   s.find("x");  s.index("x")
来源：http://xk.yuexingan06.cn

PHP:  strpos($s, "x");
来源：http://wl.shxzskj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ym.muxihuayi.cn

TS:   s.indexOf("x")
来源：http://bs.nicolike.cn

Java: s.indexOf("x")
来源：http://ih.nszjky.cn


<!-- 参考信息 -->