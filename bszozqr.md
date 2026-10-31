代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://jf.colortex.cn

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://pw.shxzukj.cn

[D05] 访问与修改元素
来源：http://ww.bookmarksfly.cn

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://sl.hnjuh.cn

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://nx.wgjwhj.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://ct.szsharing.cn

TS:   arr[0]; arr.at(-1);
来源：http://bx.colortex.cn

Java: list.get(0); list.set(0, 9);
来源：http://ud.haigaiapp.cn

Go:   arr[0]; arr[0] = 9
来源：http://bq.yuexingan06.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://nf.wgjwhj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://nk.newstarts.cn

[D06] 数组长度
来源：http://ri.bookmarksfly.cn

Py:   len(arr)
来源：http://sf.jctech888.com.cn

PHP:  count($arr);
来源：http://zm.haigaiapp.cn

JS:   arr.length
来源：http://ti.chemitech.net.cn

TS:   arr.length
来源：http://yl.huanxung.cn

Java: list.size();
来源：http://nn.colortex.cn

Go:   len(arr)
来源：http://nm.huixinmuqiang.cn

Ruby: arr.length; arr.size
来源：http://rm.muxihuayi.cn

C#:   list.Count;
来源：http://xk.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://xx.bookmarksfly.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://dg.huanxung.cn

PHP:  array_slice($arr, 1, 3);
来源：http://gb.huanxung.cn

JS:   arr.slice(1, 4);
来源：http://nu.shxzskj.cn

TS:   arr.slice(1, 4);
来源：http://oi.yuntaijiaju.cn

Java: list.subList(1, 4);
来源：http://fz.huanxung.cn

Go:   arr[1:4]
来源：http://lx.colortex.cn

Ruby: arr[1, 3]
来源：http://jp.huanxung.cn

C#:   list.GetRange(1, 3);
来源：http://su.asd995.cn

[D08] 合并两个数组
来源：http://ds.newstarts.cn

Py:   a + b;  a.extend(b)
来源：http://cp.bookmarksfly.cn

PHP:  array_merge($a, $b);
来源：http://da.shxzukj.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://bw.shxzskj.cn

TS:   [...a, ...b];
来源：http://kq.asd995.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ie.nszjky.cn

Go:   append(a, b...)
来源：http://mk.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://rz.521024.cn

C#:   a.Concat(b).ToList()
来源：http://vo.panjiajie.cn

[D09] 排序（升序）
来源：http://tq.shxzukj.cn

Py:   sorted(arr);  arr.sort()
来源：http://tf.shtwfgs.cn

PHP:  sort($arr);
来源：http://ni.huanxung.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://bh.colortex.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://se.gzmigu.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ps.shxzskj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://bf.gzmigu.cn

Ruby: arr.sort
来源：http://xb.huanxung.cn

C#:   list.Sort();
来源：http://sb.haigaiapp.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://ct.colortex.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://lg.chemitech.net.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://iq.huixiangedu.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://dr.wgjwhj.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://wa.nicolike.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://ft.shxzskj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ox.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://rx.jctech888.com.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://tt.wgjwhj.cn

[D11] 反转数组
来源：http://cj.asd995.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ff.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://ud.9csxet.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://at.panjiajie.cn

TS:   [...arr].reverse();
来源：http://tt.shtwfgs.cn

Java: Collections.reverse(list);
来源：http://ri.bookmarksfly.cn

Go:   slices.Reverse(arr)
来源：http://yb.nicolike.cn

Ruby: arr.reverse
来源：http://xx.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://yl.shxzskj.cn

[D12] 查找元素下标
来源：http://sc.yuexingan06.cn

Py:   arr.index(x);  x in arr
来源：http://rs.9csxet.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xb.huixinmuqiang.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ai.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ep.bjjhwx.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://iv.nszjky.cn

Go:   slices.Index(arr, x)
来源：http://gd.521024.cn

Ruby: arr.index(x)
来源：http://gx.jianghongdianzi.cn

C#:   list.IndexOf(x);
来源：http://fy.yuntaijiaju.cn

[D13] 过滤（保留满足条件的）
来源：http://wn.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://zj.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://zj.nicolike.cn

JS:   arr.filter(x => x > 3)
来源：http://ur.nszjky.cn

TS:   arr.filter(x => x > 3)
来源：http://lp.nszjky.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://fv.hahajie.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ig.colortex.cn

Ruby: arr.select { |x| x > 3 }
来源：http://tp.9csxet.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://to.521024.cn

[D14] 映射转换（每个元素变形）
来源：http://rn.gzmigu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://qc.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://os.szxytkj.cn

JS:   arr.map(x => x * 2)
来源：http://ww.colortex.cn

TS:   arr.map(x => x * 2)
来源：http://mv.nszjky.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uw.jianghongdianzi.cn

Go:   // 手写循环
来源：http://xg.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://ma.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dl.yuexingan06.cn

[D15] 去重
来源：http://gd.huixinmuqiang.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yz.panjiajie.cn

PHP:  array_unique($arr);
来源：http://td.9csxet.cn

JS:   [...new Set(arr)]
来源：http://ai.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://nl.huanxung.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ow.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://lu.bjjhwx.cn

Ruby: arr.uniq
来源：http://rf.shxzskj.cn

C#:   list.Distinct().ToList()
来源：http://un.szxytkj.cn

[D16] 求和与平均值
来源：http://ia.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jf.bookmarksfly.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://iz.szsharing.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ah.jianghongdianzi.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://fv.shtwfgs.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ve.wgjwhj.cn

Go:   // 手写循环累加
来源：http://pv.yuexingan06.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://kz.nicolike.cn

C#:   list.Sum();  list.Average()
来源：http://mq.shxzukj.cn

[D17] 最大值与最小值
来源：http://yk.yuexingan06.cn

Py:   max(arr);  min(arr)
来源：http://lq.wgjwhj.cn

PHP:  max($arr);  min($arr);
来源：http://ys.bookmarksfly.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jf.huixiangedu.cn

TS:   Math.max(...arr);
来源：http://ou.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://dd.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qt.521024.cn

Ruby: arr.max;  arr.min
来源：http://qf.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://gc.yuntaijiaju.cn

[D18] 扁平化嵌套数组
来源：http://oe.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://eo.bjjhwx.cn

PHP:  array_merge(...$nested);
来源：http://mv.colortex.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://xs.asd995.cn

TS:   nested.flat();
来源：http://nw.nicolike.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://iy.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://hf.szxytkj.cn

Ruby: nested.flatten
来源：http://bz.9csxet.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qc.chemitech.net.cn

[D19] 按字段分组
来源：http://pi.bookmarksfly.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://tt.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ch.hahajie.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://kb.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vd.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://av.521024.cn

Go:   // 手写 map[string][]T
来源：http://qf.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://au.jctech888.com.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://fx.newstarts.cn

[D20] 统计每个元素出现次数
来源：http://zq.lnxyls.cn

Py:   Counter(arr)
来源：http://vg.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://lg.yuntaijiaju.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nm.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://cx.bjjhwx.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uk.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://gc.yuexingan06.cn

Ruby: arr.tally
来源：http://qp.chemitech.net.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://jc.haigaiapp.cn

[D21] 判断是否包含某元素
来源：http://xh.huixinmuqiang.cn

Py:   x in arr
来源：http://xq.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://on.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://vz.newstarts.cn

TS:   arr.includes(x)
来源：http://kc.bookmarksfly.cn

Java: list.contains(x)
来源：http://md.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://bk.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://cw.shtwfgs.cn

C#:   list.Contains(x)
来源：http://wx.haigaiapp.cn

[D22] 复制数组（避免共享引用）
来源：http://sh.shxzskj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ah.521024.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ci.shxzukj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://cs.haigaiapp.cn

TS:   [...arr];
来源：http://ao.asd995.cn

Java: new ArrayList<>(list);
来源：http://gv.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ac.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ra.521024.cn

C#:   new List<int>(list);
来源：http://vu.jctech888.com.cn

[D23] reduce 累积计算
来源：http://ea.muxihuayi.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://sp.yuntaijiaju.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://la.hahajie.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fw.bjjhwx.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kb.hnjuh.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://nh.shtwfgs.cn

Go:   // 手写循环
来源：http://ql.shxzskj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://fj.huanxung.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fa.bookmarksfly.cn

[D24] 字典 / Map 基本操作
来源：http://wo.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://xd.hnjuh.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ut.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vn.szsharing.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://pb.bookmarksfly.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ri.yuntaijiaju.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lu.bjjhwx.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://cw.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://es.nicolike.cn

[D25] Set 集合去重与交并差
来源：http://dq.huixiangedu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dy.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ip.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hn.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://uh.chemitech.net.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xl.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ky.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://gy.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://uo.nszjky.cn

[D26] 数组转字符串
来源：http://hr.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://xm.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://dh.huixinmuqiang.cn

JS:   arr.join(", ")
来源：http://vc.521024.cn

TS:   arr.join(", ")
来源：http://xd.shxzukj.cn

Java: String.join(", ", list)
来源：http://du.hahajie.cn

Go:   strings.Join(strs, ", ")
来源：http://gg.panjiajie.cn

Ruby: arr.join(", ")
来源：http://wy.jianghongdianzi.cn

C#:   string.Join(", ", list)
来源：http://vp.haigaiapp.cn

================================================================================
来源：http://kh.wgjwhj.cn

E. 字符串处理
来源：http://mi.szsharing.cn

================================================================================
来源：http://rx.lnxyls.cn

[E01] 拼接字符串
来源：http://xr.chemitech.net.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://lv.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://fp.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://xn.bookmarksfly.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bk.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qe.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cb.asd995.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dq.bjjhwx.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://dt.colortex.cn

[E02] 重复字符串
来源：http://qb.9csxet.cn

Py:   "ab" * 3
来源：http://vg.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://ba.wgjwhj.cn

JS:   "ab".repeat(3)
来源：http://kl.nszjky.cn

TS:   "ab".repeat(3)
来源：http://qi.asd995.cn

Java: "ab".repeat(3)
来源：http://os.yuexingan06.cn

Go:   strings.Repeat("ab", 3)
来源：http://kg.521024.cn

Ruby: "ab" * 3
来源：http://oj.jctech888.com.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ki.colortex.cn

[E03] 截取子串
来源：http://vh.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hk.shtwfgs.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://gh.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://cq.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://ma.shxzukj.cn

Java: s.substring(1, 4)
来源：http://hc.muxihuayi.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vq.newstarts.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yy.shxzskj.cn

C#:   s.Substring(1, 3)
来源：http://ne.szxytkj.cn

[E04] 查找子串位置
来源：http://xx.szxytkj.cn

Py:   s.find("x");  s.index("x")
来源：http://ik.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://hu.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tp.szxytkj.cn

TS:   s.indexOf("x")
来源：http://mh.asd995.cn

Java: s.indexOf("x")
来源：http://rn.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://va.muxihuayi.cn

Ruby: s.index("x")
来源：http://ld.asd995.cn

C#:   s.IndexOf("x")
来源：http://fh.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://nc.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://um.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kj.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qx.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ev.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wo.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ws.yuntaijiaju.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ux.hahajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://oi.521024.cn

[E06] 替换子串
来源：http://mo.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ac.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://mu.wgjwhj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://nt.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://wn.asd995.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ld.bookmarksfly.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hh.chemitech.net.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ji.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://tc.bjjhwx.cn

[E07] 按分隔符拆分
来源：http://yw.szsharing.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sr.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ve.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ni.jianghongdianzi.cn

TS:   s.split(",")
来源：http://ob.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dc.szxytkj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://tk.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://qi.yuexingan06.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mz.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://tl.wgjwhj.cn

Py:   ",".join(items)
来源：http://jn.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://co.lnxyls.cn

JS:   items.join(",")
来源：http://qn.huixinmuqiang.cn

TS:   items.join(",")
来源：http://np.nszjky.cn

Java: String.join(",", items)
来源：http://wu.shxzukj.cn

Go:   strings.Join(items, ",")
来源：http://te.huixiangedu.cn

Ruby: items.join(",")
来源：http://mk.bookmarksfly.cn

C#:   string.Join(",", items)
来源：http://ae.shtwfgs.cn

[E09] 去除所有空白字符
来源：http://zm.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wj.muxihuayi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mo.chemitech.net.cn

JS:   s.replace(/\s+/g, "")
来源：http://qw.bjjhwx.cn

TS:   s.replace(/\s+/g, "")
来源：http://cx.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://rs.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yg.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sa.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kj.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://ei.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://jt.jianghongdianzi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qg.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ue.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://ul.szsharing.cn

Java: String.format("%03d", 7)
来源：http://wo.wgjwhj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pr.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://km.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yp.jctech888.com.cn

[E11] 反转字符串
来源：http://sq.nszjky.cn

Py:   s[::-1]
来源：http://pc.nicolike.cn

PHP:  strrev($s);
来源：http://hf.nszjky.cn

JS:   [...s].reverse().join("")
来源：http://iz.lnxyls.cn

TS:   [...s].reverse().join("")
来源：http://gb.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://lx.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://kx.wgjwhj.cn


<!-- 参考信息 -->