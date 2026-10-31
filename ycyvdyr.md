代发 wailian999

Go:   arr := []int{1, 2, 3}
来源：http://ho.lnxyls.cn

Ruby: arr = [1, 2, 3]
来源：http://vq.wgjwhj.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://vs.newstarts.cn

[D02] 追加元素到末尾
来源：http://yb.nicolike.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://it.521024.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://fk.huixiangedu.cn

JS:   arr.push(4);
来源：http://vq.haigaiapp.cn

TS:   arr.push(4);
来源：http://qg.szxytkj.cn

Java: list.add(4);
来源：http://ku.newstarts.cn

Go:   arr = append(arr, 4)
来源：http://mr.chemitech.net.cn

Ruby: arr << 4; arr.push(5)
来源：http://hc.colortex.cn

C#:   list.Add(4);
来源：http://gs.gzmigu.cn

[D03] 在指定位置插入元素
来源：http://qw.wgjwhj.cn

Py:   arr.insert(0, 0)
来源：http://vs.gzmigu.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://np.hahajie.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://uc.hnjuh.cn

TS:   arr.splice(0, 0, 0);
来源：http://ea.panjiajie.cn

Java: list.add(0, 0);
来源：http://pc.newstarts.cn

Go:   arr = append([]int{0}, arr...)
来源：http://ui.9csxet.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://id.shxzskj.cn

C#:   list.Insert(0, 0);
来源：http://kq.yuntaijiaju.cn

[D04] 删除元素
来源：http://wu.yuexingan06.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://tp.huixiangedu.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://fb.haigaiapp.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://wr.521024.cn

TS:   arr.splice(0, 1);
来源：http://me.nicolike.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://bj.shxzukj.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://rx.colortex.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ww.shtwfgs.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://su.wgjwhj.cn

[D05] 访问与修改元素
来源：http://jn.bjjhwx.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://yx.szxytkj.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://pa.newstarts.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://cp.yuntaijiaju.cn

TS:   arr[0]; arr.at(-1);
来源：http://fx.szxytkj.cn

Java: list.get(0); list.set(0, 9);
来源：http://hs.bookmarksfly.cn

Go:   arr[0]; arr[0] = 9
来源：http://uj.wgjwhj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://xm.shxzskj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://ce.bjjhwx.cn

[D06] 数组长度
来源：http://oc.9csxet.cn

Py:   len(arr)
来源：http://bp.9csxet.cn

PHP:  count($arr);
来源：http://od.hahajie.cn

JS:   arr.length
来源：http://zd.shxzukj.cn

TS:   arr.length
来源：http://dn.asd995.cn

Java: list.size();
来源：http://lv.shtwfgs.cn

Go:   len(arr)
来源：http://rz.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://jv.jctech888.com.cn

C#:   list.Count;
来源：http://ss.huixinmuqiang.cn

[D07] 切片 / 取子数组
来源：http://mv.colortex.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fd.521024.cn

PHP:  array_slice($arr, 1, 3);
来源：http://mg.bookmarksfly.cn

JS:   arr.slice(1, 4);
来源：http://qt.bookmarksfly.cn

TS:   arr.slice(1, 4);
来源：http://mc.muxihuayi.cn

Java: list.subList(1, 4);
来源：http://ae.chemitech.net.cn

Go:   arr[1:4]
来源：http://ua.hnjuh.cn

Ruby: arr[1, 3]
来源：http://om.newstarts.cn

C#:   list.GetRange(1, 3);
来源：http://wh.shtwfgs.cn

[D08] 合并两个数组
来源：http://na.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://af.newstarts.cn

PHP:  array_merge($a, $b);
来源：http://fv.newstarts.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://km.asd995.cn

TS:   [...a, ...b];
来源：http://zb.bjjhwx.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://es.shxzukj.cn

Go:   append(a, b...)
来源：http://bt.bjjhwx.cn

Ruby: a + b;  a.concat(b)
来源：http://nf.szxytkj.cn

C#:   a.Concat(b).ToList()
来源：http://yr.shxzskj.cn

[D09] 排序（升序）
来源：http://jc.hahajie.cn

Py:   sorted(arr);  arr.sort()
来源：http://vx.huixiangedu.cn

PHP:  sort($arr);
来源：http://bm.chemitech.net.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ro.panjiajie.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://lk.nicolike.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://yl.yuexingan06.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://sm.haigaiapp.cn

Ruby: arr.sort
来源：http://un.huixinmuqiang.cn

C#:   list.Sort();
来源：http://eo.chemitech.net.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ah.521024.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ww.gzmigu.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://on.colortex.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://zy.yuntaijiaju.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://je.jctech888.com.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://fm.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bp.gzmigu.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://fl.panjiajie.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wd.bookmarksfly.cn

[D11] 反转数组
来源：http://tf.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://sx.muxihuayi.cn

PHP:  array_reverse($arr);
来源：http://uh.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://xx.gzmigu.cn

TS:   [...arr].reverse();
来源：http://cq.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://xm.szsharing.cn

Go:   slices.Reverse(arr)
来源：http://vr.szxytkj.cn

Ruby: arr.reverse
来源：http://ot.hnjuh.cn

C#:   list.Reverse();
来源：http://hw.nicolike.cn

[D12] 查找元素下标
来源：http://fz.colortex.cn

Py:   arr.index(x);  x in arr
来源：http://ae.hahajie.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ob.newstarts.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://og.hahajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://in.shxzskj.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://xy.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://zn.shxzskj.cn

Ruby: arr.index(x)
来源：http://bx.nszjky.cn

C#:   list.IndexOf(x);
来源：http://yu.newstarts.cn

[D13] 过滤（保留满足条件的）
来源：http://sa.newstarts.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://wy.huixiangedu.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zb.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://sr.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://pf.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://xe.colortex.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://rj.jctech888.com.cn

Ruby: arr.select { |x| x > 3 }
来源：http://wc.haigaiapp.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://yj.panjiajie.cn

[D14] 映射转换（每个元素变形）
来源：http://dx.chemitech.net.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gu.colortex.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://qt.yuexingan06.cn

JS:   arr.map(x => x * 2)
来源：http://xz.asd995.cn

TS:   arr.map(x => x * 2)
来源：http://nw.shtwfgs.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://tc.szsharing.cn

Go:   // 手写循环
来源：http://bo.jianghongdianzi.cn

Ruby: arr.map { |x| x * 2 }
来源：http://cb.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://ox.nszjky.cn

[D15] 去重
来源：http://vc.yuexingan06.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://cc.wgjwhj.cn

PHP:  array_unique($arr);
来源：http://vs.wgjwhj.cn

JS:   [...new Set(arr)]
来源：http://oe.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://nw.colortex.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://vp.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ja.hahajie.cn

Ruby: arr.uniq
来源：http://dn.hahajie.cn

C#:   list.Distinct().ToList()
来源：http://cm.szsharing.cn

[D16] 求和与平均值
来源：http://rg.hahajie.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hd.huixinmuqiang.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://vl.wgjwhj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://bv.shtwfgs.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://vx.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ib.huixinmuqiang.cn

Go:   // 手写循环累加
来源：http://zf.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://sf.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://vw.newstarts.cn

[D17] 最大值与最小值
来源：http://wg.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://ml.521024.cn

PHP:  max($arr);  min($arr);
来源：http://dc.jianghongdianzi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gw.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://sy.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bi.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ch.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://qh.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://gl.muxihuayi.cn

[D18] 扁平化嵌套数组
来源：http://vv.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://xc.bookmarksfly.cn

PHP:  array_merge(...$nested);
来源：http://zv.jctech888.com.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mh.gzmigu.cn

TS:   nested.flat();
来源：http://fz.521024.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ta.huixinmuqiang.cn

Go:   // 手写双层循环
来源：http://ea.lnxyls.cn

Ruby: nested.flatten
来源：http://nd.hnjuh.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://st.wgjwhj.cn

[D19] 按字段分组
来源：http://fc.wgjwhj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vz.yuexingan06.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://au.bookmarksfly.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vw.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://gl.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xb.nszjky.cn

Go:   // 手写 map[string][]T
来源：http://pn.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jx.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://kj.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://hn.panjiajie.cn

Py:   Counter(arr)
来源：http://jm.newstarts.cn

PHP:  array_count_values($arr);
来源：http://ku.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fk.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nu.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wg.huanxung.cn

Go:   // 手写 map[T]int
来源：http://lu.colortex.cn

Ruby: arr.tally
来源：http://zp.lnxyls.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xu.521024.cn

[D21] 判断是否包含某元素
来源：http://dx.bookmarksfly.cn

Py:   x in arr
来源：http://il.shxzskj.cn

PHP:  in_array($x, $arr, true);
来源：http://ok.nszjky.cn

JS:   arr.includes(x)
来源：http://ou.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://qt.chemitech.net.cn

Java: list.contains(x)
来源：http://zg.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://zq.colortex.cn

Ruby: arr.include?(x)
来源：http://hq.muxihuayi.cn

C#:   list.Contains(x)
来源：http://bk.nszjky.cn

[D22] 复制数组（避免共享引用）
来源：http://wz.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://vj.shxzskj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xf.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ee.colortex.cn

TS:   [...arr];
来源：http://pf.asd995.cn

Java: new ArrayList<>(list);
来源：http://ww.huixiangedu.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cc.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://jn.panjiajie.cn

C#:   new List<int>(list);
来源：http://bw.newstarts.cn

[D23] reduce 累积计算
来源：http://ql.hnjuh.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lv.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://fx.szsharing.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mv.wgjwhj.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://rj.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://mi.szsharing.cn

Go:   // 手写循环
来源：http://fe.huanxung.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hx.wgjwhj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://xq.newstarts.cn

[D24] 字典 / Map 基本操作
来源：http://rh.nicolike.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rs.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rc.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ju.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://oz.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yh.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://dy.521024.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ge.lnxyls.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jr.521024.cn

[D25] Set 集合去重与交并差
来源：http://ey.yuexingan06.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wj.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://yd.nszjky.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://gk.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hb.huixiangedu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vq.lnxyls.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ld.yuntaijiaju.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hd.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://fp.panjiajie.cn

[D26] 数组转字符串
来源：http://wi.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://uv.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://hg.szsharing.cn

JS:   arr.join(", ")
来源：http://vz.gzmigu.cn

TS:   arr.join(", ")
来源：http://pa.9csxet.cn

Java: String.join(", ", list)
来源：http://ai.huanxung.cn

Go:   strings.Join(strs, ", ")
来源：http://tl.lnxyls.cn

Ruby: arr.join(", ")
来源：http://zz.jctech888.com.cn

C#:   string.Join(", ", list)
来源：http://yt.hahajie.cn

================================================================================
来源：http://ix.haigaiapp.cn

E. 字符串处理
来源：http://jt.huixiangedu.cn

================================================================================
来源：http://qi.szxytkj.cn

[E01] 拼接字符串
来源：http://za.szxytkj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cs.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mp.newstarts.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://dd.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://vj.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ik.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://is.jianghongdianzi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://kp.huixiangedu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://il.muxihuayi.cn

[E02] 重复字符串
来源：http://au.panjiajie.cn

Py:   "ab" * 3
来源：http://iz.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://ml.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://ci.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://ad.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://ej.shxzukj.cn

Go:   strings.Repeat("ab", 3)
来源：http://lu.asd995.cn

Ruby: "ab" * 3
来源：http://rw.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rk.hahajie.cn

[E03] 截取子串
来源：http://um.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sg.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://cb.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ic.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://ub.muxihuayi.cn

Java: s.substring(1, 4)
来源：http://rm.nszjky.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ij.521024.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pj.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://km.9csxet.cn

[E04] 查找子串位置
来源：http://fr.521024.cn

Py:   s.find("x");  s.index("x")
来源：http://rn.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://vw.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rw.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://iy.shtwfgs.cn

Java: s.indexOf("x")
来源：http://aj.bookmarksfly.cn

Go:   strings.Index(s, "x")
来源：http://wk.colortex.cn

Ruby: s.index("x")
来源：http://rn.chemitech.net.cn

C#:   s.IndexOf("x")
来源：http://me.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ya.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://sk.shtwfgs.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ax.yuexingan06.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://id.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fk.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://og.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://nw.shxzskj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xp.wgjwhj.cn

[E06] 替换子串
来源：http://vp.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yu.newstarts.cn

PHP:  str_replace("a", "b", $s);
来源：http://es.haigaiapp.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wt.szxytkj.cn

TS:   s.replaceAll("a", "b")
来源：http://qp.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yj.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://rz.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://vk.yuntaijiaju.cn

C#:   s.Replace("a", "b")
来源：http://lo.szxytkj.cn

[E07] 按分隔符拆分
来源：http://il.nszjky.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ng.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://id.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gu.nicolike.cn

TS:   s.split(",")
来源：http://fa.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ep.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://dj.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://gm.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wi.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://wn.nszjky.cn

Py:   ",".join(items)
来源：http://zt.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://cz.shtwfgs.cn

JS:   items.join(",")
来源：http://gs.newstarts.cn

TS:   items.join(",")
来源：http://nf.szxytkj.cn

Java: String.join(",", items)
来源：http://wb.shxzukj.cn


<!-- 参考信息 -->