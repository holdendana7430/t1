代发 wailian999

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://qw.hnjuh.cn

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://si.jctech888.com.cn

TS:   const arr: number[] = [1, 2, 3];
来源：http://pt.nicolike.cn

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://uf.nicolike.cn

Go:   arr := []int{1, 2, 3}
来源：http://aw.nszjky.cn

Ruby: arr = [1, 2, 3]
来源：http://io.colortex.cn

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://cc.yuntaijiaju.cn

[D02] 追加元素到末尾
来源：http://ul.bookmarksfly.cn

Py:   arr.append(4); arr.extend([5, 6])
来源：http://ms.muxihuayi.cn

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://ox.hahajie.cn

JS:   arr.push(4);
来源：http://ho.wgjwhj.cn

TS:   arr.push(4);
来源：http://cn.hnjuh.cn

Java: list.add(4);
来源：http://kz.lnxyls.cn

Go:   arr = append(arr, 4)
来源：http://xn.haigaiapp.cn

Ruby: arr << 4; arr.push(5)
来源：http://mb.szsharing.cn

C#:   list.Add(4);
来源：http://mt.newstarts.cn

[D03] 在指定位置插入元素
来源：http://dq.9csxet.cn

Py:   arr.insert(0, 0)
来源：http://rk.hnjuh.cn

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://ka.colortex.cn

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://cx.huixinmuqiang.cn

TS:   arr.splice(0, 0, 0);
来源：http://sl.bookmarksfly.cn

Java: list.add(0, 0);
来源：http://rz.szsharing.cn

Go:   arr = append([]int{0}, arr...)
来源：http://jr.bjjhwx.cn

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://aq.shxzukj.cn

C#:   list.Insert(0, 0);
来源：http://tk.gzmigu.cn

[D04] 删除元素
来源：http://ay.bjjhwx.cn

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://sf.newstarts.cn

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://nb.jianghongdianzi.cn

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://lw.shxzukj.cn

TS:   arr.splice(0, 1);
来源：http://bh.521024.cn

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://fa.muxihuayi.cn

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://mx.bjjhwx.cn

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ts.newstarts.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://bw.wgjwhj.cn

[D05] 访问与修改元素
来源：http://hv.newstarts.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://ed.521024.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://wk.nicolike.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://fz.panjiajie.cn

TS:   arr[0]; arr.at(-1);
来源：http://ye.shtwfgs.cn

Java: list.get(0); list.set(0, 9);
来源：http://bf.shxzskj.cn

Go:   arr[0]; arr[0] = 9
来源：http://px.shxzskj.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fr.haigaiapp.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://lk.hahajie.cn

[D06] 数组长度
来源：http://qq.shxzukj.cn

Py:   len(arr)
来源：http://fs.szxytkj.cn

PHP:  count($arr);
来源：http://gx.asd995.cn

JS:   arr.length
来源：http://fa.yuexingan06.cn

TS:   arr.length
来源：http://gj.huixinmuqiang.cn

Java: list.size();
来源：http://bu.yuexingan06.cn

Go:   len(arr)
来源：http://wp.haigaiapp.cn

Ruby: arr.length; arr.size
来源：http://ka.shxzskj.cn

C#:   list.Count;
来源：http://ud.huanxung.cn

[D07] 切片 / 取子数组
来源：http://zz.jianghongdianzi.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://fh.jianghongdianzi.cn

PHP:  array_slice($arr, 1, 3);
来源：http://qo.wgjwhj.cn

JS:   arr.slice(1, 4);
来源：http://bp.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://ys.yuexingan06.cn

Java: list.subList(1, 4);
来源：http://vj.jctech888.com.cn

Go:   arr[1:4]
来源：http://gq.gzmigu.cn

Ruby: arr[1, 3]
来源：http://as.panjiajie.cn

C#:   list.GetRange(1, 3);
来源：http://rx.521024.cn

[D08] 合并两个数组
来源：http://jw.jctech888.com.cn

Py:   a + b;  a.extend(b)
来源：http://am.szxytkj.cn

PHP:  array_merge($a, $b);
来源：http://ol.wgjwhj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://ja.haigaiapp.cn

TS:   [...a, ...b];
来源：http://xe.szsharing.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://lj.yuexingan06.cn

Go:   append(a, b...)
来源：http://df.szxytkj.cn

Ruby: a + b;  a.concat(b)
来源：http://ml.hnjuh.cn

C#:   a.Concat(b).ToList()
来源：http://qe.bookmarksfly.cn

[D09] 排序（升序）
来源：http://mg.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://xx.lnxyls.cn

PHP:  sort($arr);
来源：http://zm.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://de.yuexingan06.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://co.wgjwhj.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://sq.gzmigu.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://gr.chemitech.net.cn

Ruby: arr.sort
来源：http://md.jctech888.com.cn

C#:   list.Sort();
来源：http://wq.asd995.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://tx.chemitech.net.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zf.lnxyls.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ai.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://kc.szxytkj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://mh.huixinmuqiang.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://sf.gzmigu.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://yk.jianghongdianzi.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zt.colortex.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ev.yuntaijiaju.cn

[D11] 反转数组
来源：http://dy.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://pl.bookmarksfly.cn

PHP:  array_reverse($arr);
来源：http://sc.shxzskj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://nw.bookmarksfly.cn

TS:   [...arr].reverse();
来源：http://ys.bookmarksfly.cn

Java: Collections.reverse(list);
来源：http://vt.szxytkj.cn

Go:   slices.Reverse(arr)
来源：http://jh.hnjuh.cn

Ruby: arr.reverse
来源：http://ot.shxzskj.cn

C#:   list.Reverse();
来源：http://lq.huixiangedu.cn

[D12] 查找元素下标
来源：http://eh.huanxung.cn

Py:   arr.index(x);  x in arr
来源：http://bi.shxzskj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://fo.bjjhwx.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ny.szsharing.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://fa.jianghongdianzi.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://bx.asd995.cn

Go:   slices.Index(arr, x)
来源：http://cx.9csxet.cn

Ruby: arr.index(x)
来源：http://bb.haigaiapp.cn

C#:   list.IndexOf(x);
来源：http://nt.gzmigu.cn

[D13] 过滤（保留满足条件的）
来源：http://pm.nicolike.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mc.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wj.panjiajie.cn

JS:   arr.filter(x => x > 3)
来源：http://sa.huixinmuqiang.cn

TS:   arr.filter(x => x > 3)
来源：http://dy.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://cr.yuexingan06.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://uz.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hp.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://dj.bjjhwx.cn

[D14] 映射转换（每个元素变形）
来源：http://vi.szxytkj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nc.hahajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://px.jianghongdianzi.cn

JS:   arr.map(x => x * 2)
来源：http://rr.shxzskj.cn

TS:   arr.map(x => x * 2)
来源：http://cc.szsharing.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://mu.9csxet.cn

Go:   // 手写循环
来源：http://km.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://dt.panjiajie.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://hy.muxihuayi.cn

[D15] 去重
来源：http://ua.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gs.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://ns.nszjky.cn

JS:   [...new Set(arr)]
来源：http://iz.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://yk.huixiangedu.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wg.bjjhwx.cn

Go:   // 用 map[T]struct{} 手写
来源：http://xz.bookmarksfly.cn

Ruby: arr.uniq
来源：http://ml.colortex.cn

C#:   list.Distinct().ToList()
来源：http://pn.9csxet.cn

[D16] 求和与平均值
来源：http://zv.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://rz.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://vm.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://yx.haigaiapp.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://tj.haigaiapp.cn

Go:   // 手写循环累加
来源：http://ra.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://xh.colortex.cn

C#:   list.Sum();  list.Average()
来源：http://lz.nicolike.cn

[D17] 最大值与最小值
来源：http://eq.asd995.cn

Py:   max(arr);  min(arr)
来源：http://nz.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://jg.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dg.bjjhwx.cn

TS:   Math.max(...arr);
来源：http://sb.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://oa.hahajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://xs.asd995.cn

Ruby: arr.max;  arr.min
来源：http://bl.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://nn.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://fj.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://tj.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://vc.shxzukj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://el.panjiajie.cn

TS:   nested.flat();
来源：http://bt.lnxyls.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ul.521024.cn

Go:   // 手写双层循环
来源：http://vp.nszjky.cn

Ruby: nested.flatten
来源：http://va.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gh.9csxet.cn

[D19] 按字段分组
来源：http://ij.huanxung.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://od.9csxet.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://sj.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xb.521024.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://lr.shxzukj.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://dv.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://ts.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://yt.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ut.lnxyls.cn

[D20] 统计每个元素出现次数
来源：http://nu.nszjky.cn

Py:   Counter(arr)
来源：http://mr.hahajie.cn

PHP:  array_count_values($arr);
来源：http://yc.521024.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://qp.jianghongdianzi.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ff.hahajie.cn

Go:   // 手写 map[T]int
来源：http://qf.9csxet.cn

Ruby: arr.tally
来源：http://xg.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://fz.muxihuayi.cn

[D21] 判断是否包含某元素
来源：http://uj.chemitech.net.cn

Py:   x in arr
来源：http://kh.haigaiapp.cn

PHP:  in_array($x, $arr, true);
来源：http://ku.chemitech.net.cn

JS:   arr.includes(x)
来源：http://lj.colortex.cn

TS:   arr.includes(x)
来源：http://vp.521024.cn

Java: list.contains(x)
来源：http://lb.yuntaijiaju.cn

Go:   slices.Contains(arr, x)
来源：http://dl.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://xr.szxytkj.cn

C#:   list.Contains(x)
来源：http://xz.huixinmuqiang.cn

[D22] 复制数组（避免共享引用）
来源：http://vj.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://fb.panjiajie.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ei.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9csxet.cn

TS:   [...arr];
来源：http://re.nicolike.cn

Java: new ArrayList<>(list);
来源：http://ve.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lk.nicolike.cn

Ruby: arr.dup;  arr.clone
来源：http://lh.lnxyls.cn

C#:   new List<int>(list);
来源：http://vu.shtwfgs.cn

[D23] reduce 累积计算
来源：http://wb.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://lv.521024.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jj.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://yb.lnxyls.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uf.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vr.asd995.cn

Go:   // 手写循环
来源：http://rm.colortex.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vb.chemitech.net.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vt.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://lh.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://it.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://rk.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://py.521024.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://rn.gzmigu.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ax.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://rm.chemitech.net.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wm.bookmarksfly.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://lk.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ln.nszjky.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://zy.huixinmuqiang.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://xr.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://nz.jianghongdianzi.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://yx.shxzskj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://oj.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tu.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zx.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://yp.bjjhwx.cn

[D26] 数组转字符串
来源：http://xn.newstarts.cn

Py:   ", ".join(map(str, arr))
来源：http://zy.yuntaijiaju.cn

PHP:  implode(", ", $arr);
来源：http://hw.panjiajie.cn

JS:   arr.join(", ")
来源：http://mc.jctech888.com.cn

TS:   arr.join(", ")
来源：http://pd.nszjky.cn

Java: String.join(", ", list)
来源：http://mb.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://zi.lnxyls.cn

Ruby: arr.join(", ")
来源：http://uo.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://no.nicolike.cn

================================================================================
来源：http://jo.nszjky.cn

E. 字符串处理
来源：http://ht.shxzskj.cn

================================================================================
来源：http://vj.jianghongdianzi.cn

[E01] 拼接字符串
来源：http://yn.muxihuayi.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yy.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ic.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://lo.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hs.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qg.nicolike.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://jo.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://pj.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://gz.yuntaijiaju.cn

[E02] 重复字符串
来源：http://fh.haigaiapp.cn

Py:   "ab" * 3
来源：http://nt.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://ld.asd995.cn

JS:   "ab".repeat(3)
来源：http://ca.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://xp.asd995.cn

Java: "ab".repeat(3)
来源：http://ll.nszjky.cn

Go:   strings.Repeat("ab", 3)
来源：http://ub.huixinmuqiang.cn

Ruby: "ab" * 3
来源：http://tr.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xv.jianghongdianzi.cn

[E03] 截取子串
来源：http://bf.bookmarksfly.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://fz.muxihuayi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://zr.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://aw.newstarts.cn

TS:   s.slice(1, 4)
来源：http://my.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://px.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://kp.muxihuayi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yi.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://ya.chemitech.net.cn

[E04] 查找子串位置
来源：http://gk.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://ci.newstarts.cn

PHP:  strpos($s, "x");
来源：http://zu.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.haigaiapp.cn

TS:   s.indexOf("x")
来源：http://vs.hahajie.cn

Java: s.indexOf("x")
来源：http://mk.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://wk.bjjhwx.cn

Ruby: s.index("x")
来源：http://vu.lnxyls.cn

C#:   s.IndexOf("x")
来源：http://xb.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://oi.shxzskj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dy.hnjuh.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://yl.huanxung.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ai.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sx.shxzskj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dn.chemitech.net.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zw.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vy.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://xf.asd995.cn

[E06] 替换子串
来源：http://ce.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ez.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://of.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ip.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://uk.bookmarksfly.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vt.nszjky.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mk.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fc.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://si.shxzskj.cn

[E07] 按分隔符拆分
来源：http://ze.lnxyls.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://bw.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ep.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://cl.yuntaijiaju.cn

TS:   s.split(",")
来源：http://sd.gzmigu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ji.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gz.9csxet.cn

Ruby: s.split(",");  s.split
来源：http://hk.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ak.asd995.cn

[E08] 数组按分隔符合并
来源：http://ty.chemitech.net.cn

Py:   ",".join(items)
来源：http://xc.chemitech.net.cn


<!-- 参考信息 -->