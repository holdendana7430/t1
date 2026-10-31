代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://aj.yuexingan06.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://ww.521024.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://ov.szxytkj.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://va.gzmigu.cn

Go:   arr := []int{1, 2, 3}
来源：http://ij.yuntaijiaju.cn

Ruby: arr = [1, 2, 3]
来源：http://az.huixinmuqiang.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://ml.jctech888.com.cn

[D02] 追加元素到末尾
来源：http://pn.shtwfgs.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://yl.asd995.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://cd.colortex.cn

JS:   arr.push(4);
来源：http://yk.jianghongdianzi.cn

TS:   arr.push(4);
来源：http://do.hahajie.cn

Java: list.add(4);
来源：http://kw.panjiajie.cn

Go:   arr = append(arr, 4)
来源：http://ay.asd995.cn

Ruby: arr << 4; arr.push(5)
来源：http://bs.9csxet.cn

C#:   list.Add(4);
来源：http://tz.panjiajie.cn

[D03] 在指定位置插入元素
来源：http://dh.jianghongdianzi.cn

Py:   arr.insert(0, 0)
来源：http://yn.bjjhwx.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://dm.shxzukj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://xq.muxihuayi.cn

TS:   arr.splice(0, 0, 0);
来源：http://ql.haigaiapp.cn

Java: list.add(0, 0);
来源：http://iz.huanxung.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ab.huanxung.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://if.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://xz.yuexingan06.cn

[D04] 删除元素
来源：http://rd.gzmigu.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://on.hnjuh.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://bb.nszjky.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://pp.chemitech.net.cn

TS:   arr.splice(0, 1);
来源：http://it.yuexingan06.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://qg.yuntaijiaju.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://qk.huanxung.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jv.9csxet.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://yc.asd995.cn

[D05] 访问与修改元素
来源：http://sv.nszjky.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ns.shxzskj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://kz.bjjhwx.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ve.jctech888.com.cn

TS:   arr[0]; arr.at(-1);
来源：http://lb.newstarts.cn

Java: list.get(0); list.set(0, 9);
来源：http://fk.nicolike.cn

Go:   arr[0]; arr[0] = 9
来源：http://gq.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://jg.jctech888.com.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://qe.wgjwhj.cn

[D06] 数组长度
来源：http://fh.asd995.cn

Py:   len(arr)
来源：http://yq.shtwfgs.cn

PHP:  count($arr);
来源：http://po.hahajie.cn

JS:   arr.length
来源：http://yk.gzmigu.cn

TS:   arr.length
来源：http://hb.9csxet.cn

Java: list.size();
来源：http://xa.521024.cn

Go:   len(arr)
来源：http://vu.gzmigu.cn

Ruby: arr.length; arr.size
来源：http://zi.shtwfgs.cn

C#:   list.Count;
来源：http://ru.hnjuh.cn

[D07] 切片 / 取子数组
来源：http://le.huanxung.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://nv.muxihuayi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://iu.nszjky.cn

JS:   arr.slice(1, 4);
来源：http://bd.nszjky.cn

TS:   arr.slice(1, 4);
来源：http://yr.chemitech.net.cn

Java: list.subList(1, 4);
来源：http://qh.asd995.cn

Go:   arr[1:4]
来源：http://ck.haigaiapp.cn

Ruby: arr[1, 3]
来源：http://cm.szsharing.cn

C#:   list.GetRange(1, 3);
来源：http://qw.jctech888.com.cn

[D08] 合并两个数组
来源：http://yu.lnxyls.cn

Py:   a + b;  a.extend(b)
来源：http://ak.shtwfgs.cn

PHP:  array_merge($a, $b);
来源：http://hb.jianghongdianzi.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://sw.hnjuh.cn

TS:   [...a, ...b];
来源：http://cz.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://nn.hnjuh.cn

Go:   append(a, b...)
来源：http://zg.9csxet.cn

Ruby: a + b;  a.concat(b)
来源：http://yk.shxzukj.cn

C#:   a.Concat(b).ToList()
来源：http://gl.nicolike.cn

[D09] 排序（升序）
来源：http://he.huanxung.cn

Py:   sorted(arr);  arr.sort()
来源：http://tv.colortex.cn

PHP:  sort($arr);
来源：http://zt.shxzukj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ae.nicolike.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://zx.bjjhwx.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://pq.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://el.nicolike.cn

Ruby: arr.sort
来源：http://ay.colortex.cn

C#:   list.Sort();
来源：http://hs.shxzukj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://kn.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://do.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ub.shxzukj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wj.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://fe.hnjuh.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://zr.bookmarksfly.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qh.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fz.lnxyls.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://lt.szxytkj.cn

[D11] 反转数组
来源：http://js.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://dk.nszjky.cn

PHP:  array_reverse($arr);
来源：http://rr.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ix.yuexingan06.cn

TS:   [...arr].reverse();
来源：http://gv.lnxyls.cn

Java: Collections.reverse(list);
来源：http://xv.bjjhwx.cn

Go:   slices.Reverse(arr)
来源：http://pm.shtwfgs.cn

Ruby: arr.reverse
来源：http://eb.bookmarksfly.cn

C#:   list.Reverse();
来源：http://qy.hnjuh.cn

[D12] 查找元素下标
来源：http://ba.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://gx.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://td.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://cu.shxzskj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ot.lnxyls.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://qh.muxihuayi.cn

Go:   slices.Index(arr, x)
来源：http://iw.muxihuayi.cn

Ruby: arr.index(x)
来源：http://iw.gzmigu.cn

C#:   list.IndexOf(x);
来源：http://ud.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://ib.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://kj.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zp.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://wj.shxzukj.cn

TS:   arr.filter(x => x > 3)
来源：http://ue.9csxet.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://jm.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://bc.asd995.cn

Ruby: arr.select { |x| x > 3 }
来源：http://zf.hnjuh.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://om.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://lj.huanxung.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://do.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://pb.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://gs.hnjuh.cn

TS:   arr.map(x => x * 2)
来源：http://pp.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://eh.yuntaijiaju.cn

Go:   // 手写循环
来源：http://dz.yuexingan06.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qo.jctech888.com.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://fp.muxihuayi.cn

[D15] 去重
来源：http://xb.hnjuh.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://su.9csxet.cn

PHP:  array_unique($arr);
来源：http://zp.asd995.cn

JS:   [...new Set(arr)]
来源：http://cm.huixiangedu.cn

TS:   [...new Set(arr)]
来源：http://hl.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qa.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wm.9csxet.cn

Ruby: arr.uniq
来源：http://ps.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://ry.nszjky.cn

[D16] 求和与平均值
来源：http://qm.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ez.jianghongdianzi.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://lt.nszjky.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://gp.muxihuayi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jv.huanxung.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://br.9csxet.cn

Go:   // 手写循环累加
来源：http://my.gzmigu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iq.nszjky.cn

C#:   list.Sum();  list.Average()
来源：http://hx.hnjuh.cn

[D17] 最大值与最小值
来源：http://in.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://fy.szsharing.cn

PHP:  max($arr);  min($arr);
来源：http://hd.lnxyls.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yl.nicolike.cn

TS:   Math.max(...arr);
来源：http://hs.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dg.hnjuh.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qy.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://nm.asd995.cn

C#:   list.Max();  list.Min()
来源：http://wn.jctech888.com.cn

[D18] 扁平化嵌套数组
来源：http://xv.9csxet.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://yz.szsharing.cn

PHP:  array_merge(...$nested);
来源：http://pg.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ql.panjiajie.cn

TS:   nested.flat();
来源：http://ng.szxytkj.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oa.gzmigu.cn

Go:   // 手写双层循环
来源：http://pz.bookmarksfly.cn

Ruby: nested.flatten
来源：http://xm.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lg.chemitech.net.cn

[D19] 按字段分组
来源：http://ii.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://rj.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://rq.szsharing.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://dr.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://cf.bookmarksfly.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://sc.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://nq.hnjuh.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ir.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://pm.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://di.panjiajie.cn

Py:   Counter(arr)
来源：http://eg.yuntaijiaju.cn

PHP:  array_count_values($arr);
来源：http://lp.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vi.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hh.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wl.yuexingan06.cn

Go:   // 手写 map[T]int
来源：http://yg.chemitech.net.cn

Ruby: arr.tally
来源：http://wa.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lb.asd995.cn

[D21] 判断是否包含某元素
来源：http://ys.nszjky.cn

Py:   x in arr
来源：http://pb.huanxung.cn

PHP:  in_array($x, $arr, true);
来源：http://sf.jianghongdianzi.cn

JS:   arr.includes(x)
来源：http://ae.huixiangedu.cn

TS:   arr.includes(x)
来源：http://ps.shtwfgs.cn

Java: list.contains(x)
来源：http://om.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://je.9csxet.cn

Ruby: arr.include?(x)
来源：http://pt.huixiangedu.cn

C#:   list.Contains(x)
来源：http://pf.muxihuayi.cn

[D22] 复制数组（避免共享引用）
来源：http://gm.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://se.colortex.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://qw.hahajie.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yn.wgjwhj.cn

TS:   [...arr];
来源：http://to.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://nn.nszjky.cn

Go:   copied := append([]int(nil), arr...)
来源：http://kb.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://sk.wgjwhj.cn

C#:   new List<int>(list);
来源：http://kj.chemitech.net.cn

[D23] reduce 累积计算
来源：http://mo.bjjhwx.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sz.jctech888.com.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xy.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vn.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sq.wgjwhj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pq.lnxyls.cn

Go:   // 手写循环
来源：http://gm.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ky.huixinmuqiang.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://qe.haigaiapp.cn

[D24] 字典 / Map 基本操作
来源：http://ug.asd995.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mw.bjjhwx.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ck.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://eu.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rj.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://re.bookmarksfly.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://cs.lnxyls.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oz.yuexingan06.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ld.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://te.9csxet.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kn.shtwfgs.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ut.shxzukj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ac.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vp.yuntaijiaju.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xj.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://oy.lnxyls.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ug.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://bw.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://wj.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://gk.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://ze.hahajie.cn

JS:   arr.join(", ")
来源：http://ln.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://yu.bjjhwx.cn

Java: String.join(", ", list)
来源：http://qa.haigaiapp.cn

Go:   strings.Join(strs, ", ")
来源：http://ss.muxihuayi.cn

Ruby: arr.join(", ")
来源：http://by.hahajie.cn

C#:   string.Join(", ", list)
来源：http://qw.nszjky.cn

================================================================================
来源：http://sf.muxihuayi.cn

E. 字符串处理
来源：http://rj.gzmigu.cn

================================================================================
来源：http://wb.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://ur.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fd.muxihuayi.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://gu.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ey.shxzukj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://su.hnjuh.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oi.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://pa.newstarts.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hm.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yj.huanxung.cn

[E02] 重复字符串
来源：http://ro.jianghongdianzi.cn

Py:   "ab" * 3
来源：http://yr.haigaiapp.cn

PHP:  str_repeat("ab", 3);
来源：http://ad.shxzukj.cn

JS:   "ab".repeat(3)
来源：http://cj.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://xn.colortex.cn

Java: "ab".repeat(3)
来源：http://st.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://an.nszjky.cn

Ruby: "ab" * 3
来源：http://ej.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ni.bookmarksfly.cn

[E03] 截取子串
来源：http://dk.newstarts.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://cn.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qf.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wo.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://tj.huixinmuqiang.cn

Java: s.substring(1, 4)
来源：http://wp.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://zd.shtwfgs.cn

Ruby: s[1, 3];  s[1..3]
来源：http://at.nicolike.cn

C#:   s.Substring(1, 3)
来源：http://ro.wgjwhj.cn

[E04] 查找子串位置
来源：http://iz.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://ug.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://od.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jx.shxzskj.cn

TS:   s.indexOf("x")
来源：http://bu.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://ml.nicolike.cn

Go:   strings.Index(s, "x")
来源：http://dv.yuexingan06.cn

Ruby: s.index("x")
来源：http://km.hnjuh.cn

C#:   s.IndexOf("x")
来源：http://kf.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fm.haigaiapp.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ks.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kv.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ws.wgjwhj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ur.nicolike.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uo.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://fj.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://sd.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kb.huixiangedu.cn

[E06] 替换子串
来源：http://ww.jianghongdianzi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://id.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://vn.huixinmuqiang.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pd.haigaiapp.cn

TS:   s.replaceAll("a", "b")
来源：http://kp.chemitech.net.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jx.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zf.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ym.huixiangedu.cn

C#:   s.Replace("a", "b")
来源：http://bn.huanxung.cn

[E07] 按分隔符拆分
来源：http://eg.newstarts.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://lg.huixinmuqiang.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://zn.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://dj.newstarts.cn

TS:   s.split(",")
来源：http://pm.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ws.huanxung.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://vf.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://kl.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ew.nszjky.cn

[E08] 数组按分隔符合并
来源：http://si.colortex.cn

Py:   ",".join(items)
来源：http://ys.521024.cn


<!-- 参考信息 -->