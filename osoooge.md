代发 wailian999

[D03] 在指定位置插入元素
来源：http://xm.newstarts.cn

Py:   arr.insert(0, 0)
来源：http://lr.szsharing.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://fo.nszjky.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://eu.jianghongdianzi.cn

TS:   arr.splice(0, 0, 0);
来源：http://jh.9csxet.cn

Java: list.add(0, 0);
来源：http://lm.nszjky.cn

Go:   arr = append([]int{0}, arr...)
来源：http://da.shtwfgs.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://dy.hahajie.cn

C#:   list.Insert(0, 0);
来源：http://hn.shxzukj.cn

[D04] 删除元素
来源：http://hn.jianghongdianzi.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://py.shxzskj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://kc.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://qp.colortex.cn

TS:   arr.splice(0, 1);
来源：http://jw.yuntaijiaju.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://eb.hahajie.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://ya.chemitech.net.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://og.wgjwhj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://jb.jianghongdianzi.cn

[D05] 访问与修改元素
来源：http://di.chemitech.net.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ts.szsharing.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nt.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://bd.muxihuayi.cn

TS:   arr[0]; arr.at(-1);
来源：http://mc.521024.cn

Java: list.get(0); list.set(0, 9);
来源：http://fv.muxihuayi.cn

Go:   arr[0]; arr[0] = 9
来源：http://vp.huixiangedu.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://qj.newstarts.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://cn.shxzukj.cn

[D06] 数组长度
来源：http://ge.nicolike.cn

Py:   len(arr)
来源：http://dy.bjjhwx.cn

PHP:  count($arr);
来源：http://ia.9csxet.cn

JS:   arr.length
来源：http://jb.shxzukj.cn

TS:   arr.length
来源：http://ca.hnjuh.cn

Java: list.size();
来源：http://le.muxihuayi.cn

Go:   len(arr)
来源：http://vy.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://zp.haigaiapp.cn

C#:   list.Count;
来源：http://mc.huixiangedu.cn

[D07] 切片 / 取子数组
来源：http://fi.shtwfgs.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uw.haigaiapp.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ut.yuexingan06.cn

JS:   arr.slice(1, 4);
来源：http://kf.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://jj.hnjuh.cn

Java: list.subList(1, 4);
来源：http://ew.yuntaijiaju.cn

Go:   arr[1:4]
来源：http://ov.shtwfgs.cn

Ruby: arr[1, 3]
来源：http://zr.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://fx.yuntaijiaju.cn

[D08] 合并两个数组
来源：http://lv.huixinmuqiang.cn

Py:   a + b;  a.extend(b)
来源：http://gy.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://vg.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sq.panjiajie.cn

TS:   [...a, ...b];
来源：http://lw.jianghongdianzi.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://zl.newstarts.cn

Go:   append(a, b...)
来源：http://ku.haigaiapp.cn

Ruby: a + b;  a.concat(b)
来源：http://sk.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://hy.jianghongdianzi.cn

[D09] 排序（升序）
来源：http://bf.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://am.hnjuh.cn

PHP:  sort($arr);
来源：http://ac.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wq.jianghongdianzi.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://gy.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://we.nicolike.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://dw.wgjwhj.cn

Ruby: arr.sort
来源：http://co.szxytkj.cn

C#:   list.Sort();
来源：http://vx.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://yx.asd995.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://df.szxytkj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ws.nszjky.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yx.haigaiapp.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://py.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://an.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://dh.panjiajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nc.nicolike.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://yc.shxzukj.cn

[D11] 反转数组
来源：http://un.hnjuh.cn

Py:   arr[::-1];  arr.reverse()
来源：http://gp.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://gx.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ud.asd995.cn

TS:   [...arr].reverse();
来源：http://zk.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://ea.colortex.cn

Go:   slices.Reverse(arr)
来源：http://hi.szsharing.cn

Ruby: arr.reverse
来源：http://dm.bjjhwx.cn

C#:   list.Reverse();
来源：http://pp.nszjky.cn

[D12] 查找元素下标
来源：http://pi.newstarts.cn

Py:   arr.index(x);  x in arr
来源：http://oz.jianghongdianzi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hy.asd995.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ke.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ea.hahajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://uu.chemitech.net.cn

Go:   slices.Index(arr, x)
来源：http://dp.lnxyls.cn

Ruby: arr.index(x)
来源：http://xa.nszjky.cn

C#:   list.IndexOf(x);
来源：http://pt.jctech888.com.cn

[D13] 过滤（保留满足条件的）
来源：http://lp.jctech888.com.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ug.jianghongdianzi.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ew.wgjwhj.cn

JS:   arr.filter(x => x > 3)
来源：http://qy.gzmigu.cn

TS:   arr.filter(x => x > 3)
来源：http://db.nicolike.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hd.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qt.9csxet.cn

Ruby: arr.select { |x| x > 3 }
来源：http://bl.newstarts.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://el.nicolike.cn

[D14] 映射转换（每个元素变形）
来源：http://kx.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wm.huanxung.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ey.muxihuayi.cn

JS:   arr.map(x => x * 2)
来源：http://so.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://fn.chemitech.net.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://va.bjjhwx.cn

Go:   // 手写循环
来源：http://jr.bookmarksfly.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yg.muxihuayi.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ir.newstarts.cn

[D15] 去重
来源：http://xy.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://tl.szxytkj.cn

PHP:  array_unique($arr);
来源：http://kx.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://wy.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ua.hnjuh.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qq.huanxung.cn

Go:   // 用 map[T]struct{} 手写
来源：http://zq.huanxung.cn

Ruby: arr.uniq
来源：http://ae.521024.cn

C#:   list.Distinct().ToList()
来源：http://yc.hnjuh.cn

[D16] 求和与平均值
来源：http://mq.yuntaijiaju.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jo.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://of.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://mv.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ay.nszjky.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ey.shtwfgs.cn

Go:   // 手写循环累加
来源：http://za.szsharing.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://lj.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://la.wgjwhj.cn

[D17] 最大值与最小值
来源：http://rx.muxihuayi.cn

Py:   max(arr);  min(arr)
来源：http://ar.yuexingan06.cn

PHP:  max($arr);  min($arr);
来源：http://ja.newstarts.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ln.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://af.yuntaijiaju.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://mp.bookmarksfly.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xh.yuntaijiaju.cn

Ruby: arr.max;  arr.min
来源：http://cw.yuexingan06.cn

C#:   list.Max();  list.Min()
来源：http://ns.szxytkj.cn

[D18] 扁平化嵌套数组
来源：http://kd.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://et.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://ol.nszjky.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://nw.chemitech.net.cn

TS:   nested.flat();
来源：http://ty.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://jm.wgjwhj.cn

Go:   // 手写双层循环
来源：http://ld.muxihuayi.cn

Ruby: nested.flatten
来源：http://pq.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ra.muxihuayi.cn

[D19] 按字段分组
来源：http://wf.9csxet.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ce.shtwfgs.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://zl.szxytkj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://im.jctech888.com.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://dj.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xz.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://vf.asd995.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bl.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fy.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://hf.shxzukj.cn

Py:   Counter(arr)
来源：http://rh.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://xt.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lx.huixinmuqiang.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dl.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://km.huixinmuqiang.cn

Go:   // 手写 map[T]int
来源：http://gz.nicolike.cn

Ruby: arr.tally
来源：http://bd.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://bf.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://yb.panjiajie.cn

Py:   x in arr
来源：http://qb.huixinmuqiang.cn

PHP:  in_array($x, $arr, true);
来源：http://ee.hahajie.cn

JS:   arr.includes(x)
来源：http://va.colortex.cn

TS:   arr.includes(x)
来源：http://ie.gzmigu.cn

Java: list.contains(x)
来源：http://lk.gzmigu.cn

Go:   slices.Contains(arr, x)
来源：http://bw.szsharing.cn

Ruby: arr.include?(x)
来源：http://cv.shtwfgs.cn

C#:   list.Contains(x)
来源：http://dv.bookmarksfly.cn

[D22] 复制数组（避免共享引用）
来源：http://na.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ho.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ci.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wh.shtwfgs.cn

TS:   [...arr];
来源：http://qu.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://la.asd995.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ku.huixinmuqiang.cn

Ruby: arr.dup;  arr.clone
来源：http://ng.szxytkj.cn

C#:   new List<int>(list);
来源：http://ea.huanxung.cn

[D23] reduce 累积计算
来源：http://je.gzmigu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xy.yuexingan06.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gf.shxzukj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gm.nszjky.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dk.asd995.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://om.huanxung.cn

Go:   // 手写循环
来源：http://tg.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://qu.yuexingan06.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://zr.huanxung.cn

[D24] 字典 / Map 基本操作
来源：http://xf.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://pj.lnxyls.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://aq.yuexingan06.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ne.wgjwhj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://li.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jz.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://pp.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mb.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hf.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://dy.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://sb.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ol.lnxyls.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://em.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://qf.jianghongdianzi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lj.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://sl.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://qg.haigaiapp.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://nc.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://tg.hahajie.cn

Py:   ", ".join(map(str, arr))
来源：http://gq.shtwfgs.cn

PHP:  implode(", ", $arr);
来源：http://lj.huixiangedu.cn

JS:   arr.join(", ")
来源：http://kt.9csxet.cn

TS:   arr.join(", ")
来源：http://mi.asd995.cn

Java: String.join(", ", list)
来源：http://xu.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://vd.jctech888.com.cn

Ruby: arr.join(", ")
来源：http://pa.yuntaijiaju.cn

C#:   string.Join(", ", list)
来源：http://od.nicolike.cn

================================================================================
来源：http://sx.newstarts.cn

E. 字符串处理
来源：http://kj.asd995.cn

================================================================================
来源：http://se.521024.cn

[E01] 拼接字符串
来源：http://py.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://jl.newstarts.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://qn.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sx.lnxyls.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ky.nszjky.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hk.asd995.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mf.huixiangedu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://sy.haigaiapp.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wq.bookmarksfly.cn

[E02] 重复字符串
来源：http://bi.colortex.cn

Py:   "ab" * 3
来源：http://ye.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://pb.gzmigu.cn

JS:   "ab".repeat(3)
来源：http://jn.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://jv.nszjky.cn

Java: "ab".repeat(3)
来源：http://ky.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://vz.newstarts.cn

Ruby: "ab" * 3
来源：http://ic.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xz.wgjwhj.cn

[E03] 截取子串
来源：http://zj.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rm.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ci.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://tm.newstarts.cn

TS:   s.slice(1, 4)
来源：http://tq.huixiangedu.cn

Java: s.substring(1, 4)
来源：http://wh.shxzukj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ns.szxytkj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ye.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://ep.szxytkj.cn

[E04] 查找子串位置
来源：http://ss.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://bh.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://dr.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://la.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://hs.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://jh.shxzskj.cn

Go:   strings.Index(s, "x")
来源：http://qe.hnjuh.cn

Ruby: s.index("x")
来源：http://rt.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://pl.wgjwhj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ou.yuntaijiaju.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lm.newstarts.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cu.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bv.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://da.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ip.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zo.muxihuayi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gd.nszjky.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dg.shxzukj.cn

[E06] 替换子串
来源：http://yx.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ja.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://kt.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://eo.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://aw.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://aw.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sq.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pi.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://kk.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://eg.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kh.muxihuayi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wu.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sl.huanxung.cn

TS:   s.split(",")
来源：http://xd.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ic.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ea.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://ng.9csxet.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://fv.colortex.cn

[E08] 数组按分隔符合并
来源：http://za.panjiajie.cn

Py:   ",".join(items)
来源：http://oc.jianghongdianzi.cn

PHP:  implode(",", $items);
来源：http://bd.hnjuh.cn

JS:   items.join(",")
来源：http://mu.9csxet.cn

TS:   items.join(",")
来源：http://aw.asd995.cn

Java: String.join(",", items)
来源：http://rg.szsharing.cn

Go:   strings.Join(items, ",")
来源：http://ry.lnxyls.cn

Ruby: items.join(",")
来源：http://pk.9csxet.cn

C#:   string.Join(",", items)
来源：http://uz.hnjuh.cn

[E09] 去除所有空白字符
来源：http://ou.jianghongdianzi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://oe.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rr.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://rn.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://lt.lnxyls.cn

Java: s.replaceAll("\\s+", "")
来源：http://uz.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://en.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://oa.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://sz.bjjhwx.cn


<!-- 参考信息 -->