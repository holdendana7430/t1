代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://ee.szsharing.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://ar.shtwfgs.cn

[D05] 访问与修改元素
来源：http://bs.jctech888.com.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://gt.asd995.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://th.yuntaijiaju.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://yf.huixinmuqiang.cn

TS:   arr[0]; arr.at(-1);
来源：http://ix.wgjwhj.cn

Java: list.get(0); list.set(0, 9);
来源：http://sv.huixinmuqiang.cn

Go:   arr[0]; arr[0] = 9
来源：http://oz.newstarts.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://fh.yuexingan06.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://bj.nszjky.cn

[D06] 数组长度
来源：http://nh.9csxet.cn

Py:   len(arr)
来源：http://ca.nszjky.cn

PHP:  count($arr);
来源：http://nr.szsharing.cn

JS:   arr.length
来源：http://ku.szxytkj.cn

TS:   arr.length
来源：http://ou.yuntaijiaju.cn

Java: list.size();
来源：http://pg.hnjuh.cn

Go:   len(arr)
来源：http://at.jianghongdianzi.cn

Ruby: arr.length; arr.size
来源：http://bu.yuexingan06.cn

C#:   list.Count;
来源：http://oo.jianghongdianzi.cn

[D07] 切片 / 取子数组
来源：http://lj.szxytkj.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://ic.panjiajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://rr.panjiajie.cn

JS:   arr.slice(1, 4);
来源：http://qe.hahajie.cn

TS:   arr.slice(1, 4);
来源：http://oo.huixinmuqiang.cn

Java: list.subList(1, 4);
来源：http://hz.huixinmuqiang.cn

Go:   arr[1:4]
来源：http://sp.yuexingan06.cn

Ruby: arr[1, 3]
来源：http://wb.yuexingan06.cn

C#:   list.GetRange(1, 3);
来源：http://wk.yuexingan06.cn

[D08] 合并两个数组
来源：http://ta.shxzukj.cn

Py:   a + b;  a.extend(b)
来源：http://wh.hahajie.cn

PHP:  array_merge($a, $b);
来源：http://wd.huanxung.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://cn.jianghongdianzi.cn

TS:   [...a, ...b];
来源：http://jr.chemitech.net.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://jb.colortex.cn

Go:   append(a, b...)
来源：http://ca.shxzukj.cn

Ruby: a + b;  a.concat(b)
来源：http://ek.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://fo.bookmarksfly.cn

[D09] 排序（升序）
来源：http://cb.bjjhwx.cn

Py:   sorted(arr);  arr.sort()
来源：http://uj.bjjhwx.cn

PHP:  sort($arr);
来源：http://gl.jctech888.com.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://gk.haigaiapp.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://eg.jianghongdianzi.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ov.jctech888.com.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://qe.gzmigu.cn

Ruby: arr.sort
来源：http://vf.szxytkj.cn

C#:   list.Sort();
来源：http://qb.huixiangedu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ua.haigaiapp.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://fn.hnjuh.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://it.bookmarksfly.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://bt.yuexingan06.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://gm.gzmigu.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://jc.asd995.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hi.hnjuh.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://sz.szsharing.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bk.lnxyls.cn

[D11] 反转数组
来源：http://rv.yuntaijiaju.cn

Py:   arr[::-1];  arr.reverse()
来源：http://op.newstarts.cn

PHP:  array_reverse($arr);
来源：http://po.panjiajie.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://ey.9csxet.cn

TS:   [...arr].reverse();
来源：http://xk.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://ng.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://pf.haigaiapp.cn

Ruby: arr.reverse
来源：http://af.wgjwhj.cn

C#:   list.Reverse();
来源：http://ke.szxytkj.cn

[D12] 查找元素下标
来源：http://qu.bookmarksfly.cn

Py:   arr.index(x);  x in arr
来源：http://am.muxihuayi.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hr.bookmarksfly.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://sz.shxzukj.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mr.chemitech.net.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sm.shxzukj.cn

Go:   slices.Index(arr, x)
来源：http://ph.colortex.cn

Ruby: arr.index(x)
来源：http://pw.bjjhwx.cn

C#:   list.IndexOf(x);
来源：http://bf.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://at.bjjhwx.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://km.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ru.szsharing.cn

JS:   arr.filter(x => x > 3)
来源：http://cn.9csxet.cn

TS:   arr.filter(x => x > 3)
来源：http://bl.muxihuayi.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://lt.huixinmuqiang.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://la.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xc.jianghongdianzi.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gs.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://ru.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zh.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ye.szsharing.cn

JS:   arr.map(x => x * 2)
来源：http://mf.huixiangedu.cn

TS:   arr.map(x => x * 2)
来源：http://ay.wgjwhj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://lq.nicolike.cn

Go:   // 手写循环
来源：http://ae.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://lm.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://rr.haigaiapp.cn

[D15] 去重
来源：http://dd.colortex.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vg.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://as.newstarts.cn

JS:   [...new Set(arr)]
来源：http://jd.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://qd.panjiajie.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://pj.shtwfgs.cn

Go:   // 用 map[T]struct{} 手写
来源：http://rf.szxytkj.cn

Ruby: arr.uniq
来源：http://az.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://tz.bjjhwx.cn

[D16] 求和与平均值
来源：http://jk.jianghongdianzi.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ep.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tk.bookmarksfly.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://kb.huixinmuqiang.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://gy.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://zp.yuexingan06.cn

Go:   // 手写循环累加
来源：http://zy.wgjwhj.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ob.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://dn.9csxet.cn

[D17] 最大值与最小值
来源：http://es.521024.cn

Py:   max(arr);  min(arr)
来源：http://wt.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://xj.yuexingan06.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://fv.panjiajie.cn

TS:   Math.max(...arr);
来源：http://uc.gzmigu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ra.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qr.nicolike.cn

Ruby: arr.max;  arr.min
来源：http://on.hnjuh.cn

C#:   list.Max();  list.Min()
来源：http://qc.colortex.cn

[D18] 扁平化嵌套数组
来源：http://sb.yuntaijiaju.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://vw.chemitech.net.cn

PHP:  array_merge(...$nested);
来源：http://ht.wgjwhj.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://as.jctech888.com.cn

TS:   nested.flat();
来源：http://fz.gzmigu.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://go.haigaiapp.cn

Go:   // 手写双层循环
来源：http://jg.shxzskj.cn

Ruby: nested.flatten
来源：http://ue.asd995.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://gc.panjiajie.cn

[D19] 按字段分组
来源：http://wx.haigaiapp.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://dt.asd995.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://qr.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ph.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rz.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ey.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://pb.shtwfgs.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://sn.jianghongdianzi.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wm.haigaiapp.cn

[D20] 统计每个元素出现次数
来源：http://zq.shxzskj.cn

Py:   Counter(arr)
来源：http://nw.521024.cn

PHP:  array_count_values($arr);
来源：http://ra.yuexingan06.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ry.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uu.szsharing.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://iz.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://hb.nszjky.cn

Ruby: arr.tally
来源：http://kc.521024.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://um.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://xb.bookmarksfly.cn

Py:   x in arr
来源：http://dk.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://fz.yuntaijiaju.cn

JS:   arr.includes(x)
来源：http://fq.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://wy.colortex.cn

Java: list.contains(x)
来源：http://vf.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://nx.521024.cn

Ruby: arr.include?(x)
来源：http://ej.huixinmuqiang.cn

C#:   list.Contains(x)
来源：http://xz.shtwfgs.cn

[D22] 复制数组（避免共享引用）
来源：http://uw.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ys.szsharing.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://sv.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mt.jianghongdianzi.cn

TS:   [...arr];
来源：http://qy.colortex.cn

Java: new ArrayList<>(list);
来源：http://pc.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://gt.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://cz.bjjhwx.cn

C#:   new List<int>(list);
来源：http://fz.colortex.cn

[D23] reduce 累积计算
来源：http://fi.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wn.huixinmuqiang.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xr.haigaiapp.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://et.bjjhwx.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uf.wgjwhj.cn

Go:   // 手写循环
来源：http://jn.huixiangedu.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://kr.shxzukj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fp.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://eh.huixiangedu.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://aa.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hx.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qt.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hc.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://uo.shxzukj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hk.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cg.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://qg.szsharing.cn

[D25] Set 集合去重与交并差
来源：http://fj.shtwfgs.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://in.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://bq.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ya.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://pp.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gg.panjiajie.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://yb.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zg.yuntaijiaju.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://jc.shtwfgs.cn

[D26] 数组转字符串
来源：http://ox.wgjwhj.cn

Py:   ", ".join(map(str, arr))
来源：http://rr.panjiajie.cn

PHP:  implode(", ", $arr);
来源：http://fa.szxytkj.cn

JS:   arr.join(", ")
来源：http://dp.asd995.cn

TS:   arr.join(", ")
来源：http://bd.jctech888.com.cn

Java: String.join(", ", list)
来源：http://hr.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://lh.shxzukj.cn

Ruby: arr.join(", ")
来源：http://wj.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://wo.shxzskj.cn

================================================================================
来源：http://sv.521024.cn

E. 字符串处理
来源：http://wn.lnxyls.cn

================================================================================
来源：http://pa.shxzskj.cn

[E01] 拼接字符串
来源：http://ca.panjiajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lw.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://cm.jianghongdianzi.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qh.hnjuh.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://em.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://no.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zu.haigaiapp.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://cw.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://se.9csxet.cn

[E02] 重复字符串
来源：http://zu.gzmigu.cn

Py:   "ab" * 3
来源：http://kh.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://jm.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://hq.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://zb.asd995.cn

Java: "ab".repeat(3)
来源：http://bl.szsharing.cn

Go:   strings.Repeat("ab", 3)
来源：http://mn.lnxyls.cn

Ruby: "ab" * 3
来源：http://mn.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://yk.colortex.cn

[E03] 截取子串
来源：http://ds.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rz.shxzukj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://if.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pp.jctech888.com.cn

TS:   s.slice(1, 4)
来源：http://dl.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://wu.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bm.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ie.9csxet.cn

C#:   s.Substring(1, 3)
来源：http://yt.shxzskj.cn

[E04] 查找子串位置
来源：http://ot.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://fp.bookmarksfly.cn

PHP:  strpos($s, "x");
来源：http://ud.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ih.wgjwhj.cn

TS:   s.indexOf("x")
来源：http://tk.nszjky.cn

Java: s.indexOf("x")
来源：http://yu.muxihuayi.cn

Go:   strings.Index(s, "x")
来源：http://eo.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://pl.nszjky.cn

C#:   s.IndexOf("x")
来源：http://jy.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ej.szsharing.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gj.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kc.newstarts.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ry.9csxet.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ss.wgjwhj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kk.shxzskj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://so.lnxyls.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rh.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dt.szxytkj.cn

[E06] 替换子串
来源：http://jo.521024.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zw.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://ug.jianghongdianzi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vx.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://vb.nicolike.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sh.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://xs.nszjky.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://av.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://qr.asd995.cn

[E07] 按分隔符拆分
来源：http://br.huixiangedu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://fd.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hk.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ay.huanxung.cn

TS:   s.split(",")
来源：http://xu.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://la.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://na.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://yo.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://kf.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://kn.szsharing.cn

Py:   ",".join(items)
来源：http://kj.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://vc.hahajie.cn

JS:   items.join(",")
来源：http://xr.yuexingan06.cn

TS:   items.join(",")
来源：http://wp.huixiangedu.cn

Java: String.join(",", items)
来源：http://cu.9csxet.cn

Go:   strings.Join(items, ",")
来源：http://tm.wgjwhj.cn

Ruby: items.join(",")
来源：http://kp.nszjky.cn

C#:   string.Join(",", items)
来源：http://nc.szxytkj.cn

[E09] 去除所有空白字符
来源：http://qe.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jn.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yo.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://fm.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://cv.colortex.cn

Java: s.replaceAll("\\s+", "")
来源：http://pz.huixiangedu.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://tw.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rm.jianghongdianzi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fc.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://ii.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://th.huanxung.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://px.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://om.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://vo.chemitech.net.cn

Java: String.format("%03d", 7)
来源：http://nb.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cl.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uj.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ok.nicolike.cn

[E11] 反转字符串
来源：http://jj.shxzskj.cn

Py:   s[::-1]
来源：http://nn.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://zk.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://ox.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://po.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pj.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lx.huixiangedu.cn


<!-- 参考信息 -->