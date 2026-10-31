代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ys.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://rk.chemitech.net.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://sq.huanxung.cn

[D02] 追加元素到末尾
来源：http://db.yuexingan06.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://tj.yuexingan06.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://wp.hahajie.cn

JS:   arr.push(4);
来源：http://bt.shxzukj.cn

TS:   arr.push(4);
来源：http://tb.szsharing.cn

Java: list.add(4);
来源：http://sb.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://pr.gzmigu.cn

Ruby: arr << 4; arr.push(5)
来源：http://dq.shtwfgs.cn

C#:   list.Add(4);
来源：http://ii.szsharing.cn

[D03] 在指定位置插入元素
来源：http://su.szsharing.cn

Py:   arr.insert(0, 0)
来源：http://zb.jianghongdianzi.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://lj.szxytkj.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://me.yuntaijiaju.cn

TS:   arr.splice(0, 0, 0);
来源：http://gv.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://ih.gzmigu.cn

Go:   arr = append([]int{0}, arr...)
来源：http://zr.szxytkj.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://sm.bjjhwx.cn

C#:   list.Insert(0, 0);
来源：http://jh.panjiajie.cn

[D04] 删除元素
来源：http://cj.panjiajie.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://ga.shxzukj.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://wl.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://no.yuntaijiaju.cn

TS:   arr.splice(0, 1);
来源：http://iv.shxzukj.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://sj.bookmarksfly.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://jw.nicolike.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://cx.shxzukj.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://xw.asd995.cn

[D05] 访问与修改元素
来源：http://vr.szxytkj.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://bm.huixinmuqiang.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wp.colortex.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://wm.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://hn.yuntaijiaju.cn

Java: list.get(0); list.set(0, 9);
来源：http://sz.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://dt.huanxung.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://yn.521024.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://kv.asd995.cn

[D06] 数组长度
来源：http://cj.colortex.cn

Py:   len(arr)
来源：http://wa.shxzukj.cn

PHP:  count($arr);
来源：http://vt.shxzukj.cn

JS:   arr.length
来源：http://ki.bookmarksfly.cn

TS:   arr.length
来源：http://qu.shxzukj.cn

Java: list.size();
来源：http://ma.muxihuayi.cn

Go:   len(arr)
来源：http://ub.shxzukj.cn

Ruby: arr.length; arr.size
来源：http://ts.nicolike.cn

C#:   list.Count;
来源：http://en.szxytkj.cn

[D07] 切片 / 取子数组
来源：http://id.muxihuayi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ay.chemitech.net.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ax.asd995.cn

JS:   arr.slice(1, 4);
来源：http://xj.shtwfgs.cn

TS:   arr.slice(1, 4);
来源：http://lv.szsharing.cn

Java: list.subList(1, 4);
来源：http://to.jctech888.com.cn

Go:   arr[1:4]
来源：http://bz.newstarts.cn

Ruby: arr[1, 3]
来源：http://sk.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://bu.nicolike.cn

[D08] 合并两个数组
来源：http://dg.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://jg.szsharing.cn

PHP:  array_merge($a, $b);
来源：http://fv.hahajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ei.hnjuh.cn

TS:   [...a, ...b];
来源：http://sg.shtwfgs.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://gb.521024.cn

Go:   append(a, b...)
来源：http://hr.bookmarksfly.cn

Ruby: a + b;  a.concat(b)
来源：http://qg.lnxyls.cn

C#:   a.Concat(b).ToList()
来源：http://eh.nicolike.cn

[D09] 排序（升序）
来源：http://lz.newstarts.cn

Py:   sorted(arr);  arr.sort()
来源：http://xm.chemitech.net.cn

PHP:  sort($arr);
来源：http://yc.asd995.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://qy.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://wp.szsharing.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://uu.yuntaijiaju.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://yb.huixiangedu.cn

Ruby: arr.sort
来源：http://lp.huixinmuqiang.cn

C#:   list.Sort();
来源：http://we.szxytkj.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ln.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://pk.muxihuayi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kh.huanxung.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kr.huanxung.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wl.bookmarksfly.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://js.huixiangedu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uv.hahajie.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://am.huixinmuqiang.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://uh.asd995.cn

[D11] 反转数组
来源：http://cf.huanxung.cn

Py:   arr[::-1];  arr.reverse()
来源：http://wm.huixinmuqiang.cn

PHP:  array_reverse($arr);
来源：http://ti.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://vu.huixinmuqiang.cn

TS:   [...arr].reverse();
来源：http://je.hahajie.cn

Java: Collections.reverse(list);
来源：http://ny.haigaiapp.cn

Go:   slices.Reverse(arr)
来源：http://sa.colortex.cn

Ruby: arr.reverse
来源：http://tg.521024.cn

C#:   list.Reverse();
来源：http://ja.521024.cn

[D12] 查找元素下标
来源：http://dv.wgjwhj.cn

Py:   arr.index(x);  x in arr
来源：http://wb.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://sb.jctech888.com.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ex.huixiangedu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wu.yuexingan06.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sm.jianghongdianzi.cn

Go:   slices.Index(arr, x)
来源：http://js.huixinmuqiang.cn

Ruby: arr.index(x)
来源：http://fq.yuntaijiaju.cn

C#:   list.IndexOf(x);
来源：http://aw.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://bs.szsharing.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://te.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://da.hnjuh.cn

JS:   arr.filter(x => x > 3)
来源：http://zu.shtwfgs.cn

TS:   arr.filter(x => x > 3)
来源：http://ab.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fr.jctech888.com.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vq.bookmarksfly.cn

Ruby: arr.select { |x| x > 3 }
来源：http://yp.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://at.huanxung.cn

[D14] 映射转换（每个元素变形）
来源：http://ni.huixinmuqiang.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://ga.bjjhwx.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://vi.nszjky.cn

JS:   arr.map(x => x * 2)
来源：http://ra.shtwfgs.cn

TS:   arr.map(x => x * 2)
来源：http://vg.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://sz.asd995.cn

Go:   // 手写循环
来源：http://wf.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://eh.chemitech.net.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dy.colortex.cn

[D15] 去重
来源：http://on.gzmigu.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wv.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://rl.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ga.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://mj.nicolike.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://kd.shxzskj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://tr.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://bs.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://wd.newstarts.cn

[D16] 求和与平均值
来源：http://ql.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mt.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://zd.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ih.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gq.gzmigu.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://gw.hnjuh.cn

Go:   // 手写循环累加
来源：http://ew.newstarts.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://yh.lnxyls.cn

C#:   list.Sum();  list.Average()
来源：http://jh.szsharing.cn

[D17] 最大值与最小值
来源：http://pb.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://sk.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://in.huanxung.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ey.yuexingan06.cn

TS:   Math.max(...arr);
来源：http://df.nicolike.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dg.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://le.newstarts.cn

Ruby: arr.max;  arr.min
来源：http://hw.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://xp.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://ie.szxytkj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kk.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://vv.yuexingan06.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xs.asd995.cn

TS:   nested.flat();
来源：http://az.asd995.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://qx.nicolike.cn

Go:   // 手写双层循环
来源：http://nr.szsharing.cn

Ruby: nested.flatten
来源：http://km.huixiangedu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ew.panjiajie.cn

[D19] 按字段分组
来源：http://qg.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://gk.colortex.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ox.521024.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://aw.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vt.hahajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://zw.yuntaijiaju.cn

Go:   // 手写 map[string][]T
来源：http://gi.shxzskj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://mb.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gc.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://tq.yuntaijiaju.cn

Py:   Counter(arr)
来源：http://tt.asd995.cn

PHP:  array_count_values($arr);
来源：http://lr.newstarts.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vz.gzmigu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vk.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wf.9csxet.cn

Go:   // 手写 map[T]int
来源：http://zi.newstarts.cn

Ruby: arr.tally
来源：http://vm.9csxet.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://lj.shtwfgs.cn

[D21] 判断是否包含某元素
来源：http://en.huixinmuqiang.cn

Py:   x in arr
来源：http://ho.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ib.shtwfgs.cn

JS:   arr.includes(x)
来源：http://ov.nszjky.cn

TS:   arr.includes(x)
来源：http://ro.shxzskj.cn

Java: list.contains(x)
来源：http://dj.521024.cn

Go:   slices.Contains(arr, x)
来源：http://og.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://ue.lnxyls.cn

C#:   list.Contains(x)
来源：http://uo.colortex.cn

[D22] 复制数组（避免共享引用）
来源：http://fc.yuexingan06.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://nw.hnjuh.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://oa.shxzskj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pc.huixinmuqiang.cn

TS:   [...arr];
来源：http://ei.bookmarksfly.cn

Java: new ArrayList<>(list);
来源：http://qp.gzmigu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ng.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://gd.9csxet.cn

C#:   new List<int>(list);
来源：http://vi.huanxung.cn

[D23] reduce 累积计算
来源：http://km.colortex.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ol.bjjhwx.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://rl.hnjuh.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ei.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xt.yuntaijiaju.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://li.shxzukj.cn

Go:   // 手写循环
来源：http://al.huixinmuqiang.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ds.lnxyls.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wg.szsharing.cn

[D24] 字典 / Map 基本操作
来源：http://ss.haigaiapp.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ml.521024.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ym.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wf.panjiajie.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://np.nszjky.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qk.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.panjiajie.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pf.szxytkj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wm.shxzukj.cn

[D25] Set 集合去重与交并差
来源：http://pl.lnxyls.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://gd.521024.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lm.yuntaijiaju.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://vh.nicolike.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://bd.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://qf.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://pq.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://pj.shxzukj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zj.haigaiapp.cn

[D26] 数组转字符串
来源：http://ko.bookmarksfly.cn

Py:   ", ".join(map(str, arr))
来源：http://qi.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://sp.chemitech.net.cn

JS:   arr.join(", ")
来源：http://kg.nicolike.cn

TS:   arr.join(", ")
来源：http://ya.szsharing.cn

Java: String.join(", ", list)
来源：http://xc.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://rh.panjiajie.cn

Ruby: arr.join(", ")
来源：http://hc.huixinmuqiang.cn

C#:   string.Join(", ", list)
来源：http://kp.muxihuayi.cn

================================================================================
来源：http://wi.muxihuayi.cn

E. 字符串处理
来源：http://nl.szsharing.cn

================================================================================
来源：http://gq.yuexingan06.cn

[E01] 拼接字符串
来源：http://dm.hnjuh.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://bp.521024.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ga.muxihuayi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://de.huixinmuqiang.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://jg.huanxung.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gq.shxzskj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://kf.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ub.colortex.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://qb.gzmigu.cn

[E02] 重复字符串
来源：http://qo.9csxet.cn

Py:   "ab" * 3
来源：http://hl.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://ty.newstarts.cn

JS:   "ab".repeat(3)
来源：http://gd.shxzukj.cn

TS:   "ab".repeat(3)
来源：http://vs.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://jz.521024.cn

Go:   strings.Repeat("ab", 3)
来源：http://lp.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://fw.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://no.9csxet.cn

[E03] 截取子串
来源：http://gq.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yn.newstarts.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://uu.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ph.nszjky.cn

TS:   s.slice(1, 4)
来源：http://sm.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://lb.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sg.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hz.huixiangedu.cn

C#:   s.Substring(1, 3)
来源：http://ty.wgjwhj.cn

[E04] 查找子串位置
来源：http://xt.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://ie.jctech888.com.cn

PHP:  strpos($s, "x");
来源：http://yu.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gt.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://pf.szsharing.cn

Java: s.indexOf("x")
来源：http://xj.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://zl.colortex.cn

Ruby: s.index("x")
来源：http://cb.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://lm.nicolike.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://io.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://eu.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cl.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sw.panjiajie.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fi.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://up.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jt.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xy.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ri.huixinmuqiang.cn

[E06] 替换子串
来源：http://kv.panjiajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://un.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://ld.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ka.jctech888.com.cn

TS:   s.replaceAll("a", "b")
来源：http://mg.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xj.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wu.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://st.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://qt.huixinmuqiang.cn

[E07] 按分隔符拆分
来源：http://kd.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sl.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vs.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ac.gzmigu.cn

TS:   s.split(",")
来源：http://js.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ox.shxzukj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qw.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://tq.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dc.521024.cn

[E08] 数组按分隔符合并
来源：http://zx.shtwfgs.cn

Py:   ",".join(items)
来源：http://au.szxytkj.cn

PHP:  implode(",", $items);
来源：http://zt.haigaiapp.cn

JS:   items.join(",")
来源：http://yn.szxytkj.cn

TS:   items.join(",")
来源：http://xi.521024.cn

Java: String.join(",", items)
来源：http://rf.haigaiapp.cn


<!-- 参考信息 -->