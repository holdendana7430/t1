代发 wailian999

[C14] 泛型函数
来源：http://vw.asd995.cn

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://lc.shxzskj.cn

PHP:  // 无泛型
来源：http://qk.newstarts.cn

JS:   // 无泛型
来源：http://kr.huixinmuqiang.cn

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hn.huanxung.cn

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://nu.bjjhwx.cn

Go:   func First[T any](items []T) T { return items[0] }
来源：http://us.shxzskj.cn

Ruby: # 无泛型
来源：http://ji.haigaiapp.cn

C#:   static T First<T>(List<T> items) => items[0];
来源：http://iu.shtwfgs.cn

[C15] 解构 / 展开参数
来源：http://lj.shxzskj.cn

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://ra.panjiajie.cn

PHP:  [$a, $b] = $pair;
来源：http://xr.yuntaijiaju.cn

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://ca.panjiajie.cn

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://bf.yuexingan06.cn

Java: // 无解构
来源：http://cc.gzmigu.cn

Go:   // 无解构
来源：http://te.shtwfgs.cn

Ruby: a, b = pair
来源：http://jn.shxzskj.cn

C#:   var (a, b) = pair;
来源：http://vp.newstarts.cn

[C16] 函数 / 方法重载
来源：http://dh.521024.cn

Py:   # 无重载：用默认参数或 *args 变通
来源：http://qz.colortex.cn

PHP:  // 无重载
来源：http://rh.szxytkj.cn

JS:   // 无重载：靠 arguments.length 分支
来源：http://do.newstarts.cn

TS:   // 用联合类型或重载签名声明
来源：http://in.newstarts.cn

Java: void f(int a) {}  void f(String a) {}
来源：http://dt.hahajie.cn

Go:   // 无重载：用不同函数名
来源：http://zy.muxihuayi.cn

Ruby: # 无重载：靠动态参数
来源：http://ss.muxihuayi.cn

C#:   void F(int a) {}  void F(string a) {}
来源：http://rm.hahajie.cn

================================================================================
来源：http://qs.haigaiapp.cn

D. 数组 / 列表 / 集合
来源：http://so.huanxung.cn

================================================================================
来源：http://nk.szxytkj.cn

[D01] 创建数组 / 列表
来源：http://fo.jctech888.com.cn

Py:   arr = [1, 2, 3];  empty = []
来源：http://ym.hahajie.cn

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://wp.huixiangedu.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://td.jianghongdianzi.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://bm.yuexingan06.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://jl.lnxyls.cn

Go:   arr := []int{1, 2, 3}
来源：http://tv.shxzskj.cn

Ruby: arr = [1, 2, 3]
来源：http://co.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://yc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ye.gzmigu.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://zf.jianghongdianzi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wt.bjjhwx.cn

JS:   arr.push(4);
来源：http://ej.muxihuayi.cn

TS:   arr.push(4);
来源：http://mt.lnxyls.cn

Java: list.add(4);
来源：http://ik.yuntaijiaju.cn

Go:   arr = append(arr, 4)
来源：http://os.shxzukj.cn

Ruby: arr << 4; arr.push(5)
来源：http://kx.gzmigu.cn

C#:   list.Add(4);
来源：http://ny.9csxet.cn

[D03] 在指定位置插入元素
来源：http://tm.yuntaijiaju.cn

Py:   arr.insert(0, 0)
来源：http://ev.hahajie.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://oi.huixiangedu.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://py.nicolike.cn

TS:   arr.splice(0, 0, 0);
来源：http://hz.chemitech.net.cn

Java: list.add(0, 0);
来源：http://uq.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://fb.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sd.yuntaijiaju.cn

C#:   list.Insert(0, 0);
来源：http://ru.hnjuh.cn

[D04] 删除元素
来源：http://is.bookmarksfly.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://yn.huanxung.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://td.hnjuh.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://sm.shxzskj.cn

TS:   arr.splice(0, 1);
来源：http://qs.newstarts.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://pw.szxytkj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://wc.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://bb.nicolike.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://zt.nicolike.cn

[D05] 访问与修改元素
来源：http://qk.nicolike.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://qe.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://sp.jianghongdianzi.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://sq.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://sq.huanxung.cn

Java: list.get(0); list.set(0, 9);
来源：http://nx.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://lv.muxihuayi.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://km.yuntaijiaju.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://dy.521024.cn

[D06] 数组长度
来源：http://xj.hahajie.cn

Py:   len(arr)
来源：http://vr.jctech888.com.cn

PHP:  count($arr);
来源：http://uf.521024.cn

JS:   arr.length
来源：http://ad.nszjky.cn

TS:   arr.length
来源：http://jx.colortex.cn

Java: list.size();
来源：http://nw.huanxung.cn

Go:   len(arr)
来源：http://rz.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://cp.jctech888.com.cn

C#:   list.Count;
来源：http://uf.nszjky.cn

[D07] 切片 / 取子数组
来源：http://sn.huixinmuqiang.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fl.nszjky.cn

PHP:  array_slice($arr, 1, 3);
来源：http://pm.gzmigu.cn

JS:   arr.slice(1, 4);
来源：http://di.9csxet.cn

TS:   arr.slice(1, 4);
来源：http://cu.bjjhwx.cn

Java: list.subList(1, 4);
来源：http://fh.shxzskj.cn

Go:   arr[1:4]
来源：http://cv.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://tb.bookmarksfly.cn

C#:   list.GetRange(1, 3);
来源：http://mt.shxzukj.cn

[D08] 合并两个数组
来源：http://uo.9csxet.cn

Py:   a + b;  a.extend(b)
来源：http://tp.haigaiapp.cn

PHP:  array_merge($a, $b);
来源：http://lj.szsharing.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://wh.nicolike.cn

TS:   [...a, ...b];
来源：http://mm.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zb.bjjhwx.cn

Go:   append(a, b...)
来源：http://up.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://xr.colortex.cn

C#:   a.Concat(b).ToList()
来源：http://ua.jctech888.com.cn

[D09] 排序（升序）
来源：http://so.shxzskj.cn

Py:   sorted(arr);  arr.sort()
来源：http://ai.haigaiapp.cn

PHP:  sort($arr);
来源：http://xd.panjiajie.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://pz.jctech888.com.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ci.nszjky.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://rr.wgjwhj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dh.shxzskj.cn

Ruby: arr.sort
来源：http://kd.jctech888.com.cn

C#:   list.Sort();
来源：http://vp.yuntaijiaju.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fu.9csxet.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://rg.bookmarksfly.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rc.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://gg.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://nj.bjjhwx.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ia.hahajie.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hr.yuntaijiaju.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ul.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://it.shtwfgs.cn

[D11] 反转数组
来源：http://rd.bjjhwx.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gu.yuexingan06.cn

PHP:  array_reverse($arr);
来源：http://mq.yuexingan06.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://fl.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://ty.jctech888.com.cn

Java: Collections.reverse(list);
来源：http://gj.521024.cn

Go:   slices.Reverse(arr)
来源：http://gy.9csxet.cn

Ruby: arr.reverse
来源：http://ir.lnxyls.cn

C#:   list.Reverse();
来源：http://eg.9csxet.cn

[D12] 查找元素下标
来源：http://tz.shtwfgs.cn

Py:   arr.index(x);  x in arr
来源：http://wx.wgjwhj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://te.panjiajie.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ka.colortex.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://un.huixinmuqiang.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://li.asd995.cn

Go:   slices.Index(arr, x)
来源：http://lz.muxihuayi.cn

Ruby: arr.index(x)
来源：http://uz.hahajie.cn

C#:   list.IndexOf(x);
来源：http://ze.jianghongdianzi.cn

[D13] 过滤（保留满足条件的）
来源：http://gy.szxytkj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://pq.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://cj.nszjky.cn

JS:   arr.filter(x => x > 3)
来源：http://bv.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://ta.jianghongdianzi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://aj.gzmigu.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://lu.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://vb.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://nz.huixinmuqiang.cn

[D14] 映射转换（每个元素变形）
来源：http://fr.9csxet.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://os.521024.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ji.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://hk.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://dy.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ff.9csxet.cn

Go:   // 手写循环
来源：http://ux.lnxyls.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cu.huanxung.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://oz.huixinmuqiang.cn

[D15] 去重
来源：http://me.jianghongdianzi.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ed.shxzskj.cn

PHP:  array_unique($arr);
来源：http://dy.nszjky.cn

JS:   [...new Set(arr)]
来源：http://os.szxytkj.cn

TS:   [...new Set(arr)]
来源：http://ec.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://bz.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ma.gzmigu.cn

Ruby: arr.uniq
来源：http://ig.haigaiapp.cn

C#:   list.Distinct().ToList()
来源：http://ci.szxytkj.cn

[D16] 求和与平均值
来源：http://kc.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ig.lnxyls.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tr.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://av.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ar.hnjuh.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://xr.9csxet.cn

Go:   // 手写循环累加
来源：http://md.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://dm.jianghongdianzi.cn

C#:   list.Sum();  list.Average()
来源：http://wm.shxzukj.cn

[D17] 最大值与最小值
来源：http://ie.haigaiapp.cn

Py:   max(arr);  min(arr)
来源：http://ud.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://vv.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fv.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://am.haigaiapp.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pd.huixiangedu.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wx.nszjky.cn

Ruby: arr.max;  arr.min
来源：http://xp.newstarts.cn

C#:   list.Max();  list.Min()
来源：http://hn.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://ti.nszjky.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hn.shxzskj.cn

PHP:  array_merge(...$nested);
来源：http://au.panjiajie.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://fw.nszjky.cn

TS:   nested.flat();
来源：http://ji.hnjuh.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://uz.newstarts.cn

Go:   // 手写双层循环
来源：http://yl.huixiangedu.cn

Ruby: nested.flatten
来源：http://ku.nicolike.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://nb.asd995.cn

[D19] 按字段分组
来源：http://mc.chemitech.net.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://xi.huixinmuqiang.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hr.newstarts.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vw.huixinmuqiang.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ic.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://vo.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ja.hahajie.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ne.shtwfgs.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://oq.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://qn.shxzukj.cn

Py:   Counter(arr)
来源：http://uc.huanxung.cn

PHP:  array_count_values($arr);
来源：http://tq.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uf.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oq.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://er.huanxung.cn

Go:   // 手写 map[T]int
来源：http://wx.panjiajie.cn

Ruby: arr.tally
来源：http://ch.panjiajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://dz.bjjhwx.cn

[D21] 判断是否包含某元素
来源：http://wn.hnjuh.cn

Py:   x in arr
来源：http://ps.chemitech.net.cn

PHP:  in_array($x, $arr, true);
来源：http://ye.panjiajie.cn

JS:   arr.includes(x)
来源：http://na.shxzskj.cn

TS:   arr.includes(x)
来源：http://wc.haigaiapp.cn

Java: list.contains(x)
来源：http://jx.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://om.panjiajie.cn

Ruby: arr.include?(x)
来源：http://dr.szxytkj.cn

C#:   list.Contains(x)
来源：http://uv.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://hj.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://tu.yuexingan06.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sz.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ah.521024.cn

TS:   [...arr];
来源：http://pl.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://ee.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ng.szsharing.cn

Ruby: arr.dup;  arr.clone
来源：http://vj.521024.cn

C#:   new List<int>(list);
来源：http://tu.huixiangedu.cn

[D23] reduce 累积计算
来源：http://mj.huixinmuqiang.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eq.szxytkj.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://kd.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hs.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ui.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://yd.newstarts.cn

Go:   // 手写循环
来源：http://js.lnxyls.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mz.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wh.hahajie.cn

[D24] 字典 / Map 基本操作
来源：http://nj.yuexingan06.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://oj.jianghongdianzi.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ts.hnjuh.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hd.yuexingan06.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://kk.szxytkj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://vg.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sv.nicolike.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hw.yuntaijiaju.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qv.shtwfgs.cn

[D25] Set 集合去重与交并差
来源：http://il.chemitech.net.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ta.muxihuayi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://uk.asd995.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://tl.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rk.hnjuh.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://si.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://rk.shtwfgs.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hu.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eb.colortex.cn

[D26] 数组转字符串
来源：http://je.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://rj.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://fc.panjiajie.cn

JS:   arr.join(", ")
来源：http://sd.huixiangedu.cn

TS:   arr.join(", ")
来源：http://ws.nszjky.cn

Java: String.join(", ", list)
来源：http://kt.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://yd.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://ny.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://zy.bjjhwx.cn

================================================================================
来源：http://av.521024.cn

E. 字符串处理
来源：http://pi.shtwfgs.cn

================================================================================
来源：http://dj.huanxung.cn

[E01] 拼接字符串
来源：http://um.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://zo.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://sl.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://it.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ju.shxzskj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://jo.9csxet.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://lh.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cf.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://se.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ri.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://xc.nicolike.cn

PHP:  str_repeat("ab", 3);
来源：http://ux.jctech888.com.cn

JS:   "ab".repeat(3)
来源：http://hu.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://py.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://nw.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://qz.9csxet.cn

Ruby: "ab" * 3
来源：http://dh.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xc.bjjhwx.cn

[E03] 截取子串
来源：http://on.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ma.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://re.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wo.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://ud.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ku.huanxung.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sb.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mu.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://zy.huixiangedu.cn

[E04] 查找子串位置
来源：http://qc.bookmarksfly.cn

Py:   s.find("x");  s.index("x")
来源：http://sx.9csxet.cn

PHP:  strpos($s, "x");
来源：http://pj.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vr.shxzukj.cn

TS:   s.indexOf("x")
来源：http://rg.shxzukj.cn

Java: s.indexOf("x")
来源：http://th.yuexingan06.cn


<!-- 参考信息 -->