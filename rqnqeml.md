代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://tn.jctech888.com.cn

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://zs.shxzskj.cn

TS:   arr[0]; arr.at(-1);
来源：http://gf.jctech888.com.cn

Java: list.get(0); list.set(0, 9);
来源：http://jf.shxzukj.cn

Go:   arr[0]; arr[0] = 9
来源：http://sz.lnxyls.cn

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://rt.szxytkj.cn

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://xz.9csxet.cn

[D06] 数组长度
来源：http://nc.shxzukj.cn

Py:   len(arr)
来源：http://dq.nicolike.cn

PHP:  count($arr);
来源：http://sg.hnjuh.cn

JS:   arr.length
来源：http://bs.szsharing.cn

TS:   arr.length
来源：http://ad.521024.cn

Java: list.size();
来源：http://ib.521024.cn

Go:   len(arr)
来源：http://xw.hahajie.cn

Ruby: arr.length; arr.size
来源：http://ag.yuntaijiaju.cn

C#:   list.Count;
来源：http://fa.shxzskj.cn

[D07] 切片 / 取子数组
来源：http://ud.9csxet.cn

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://uu.hahajie.cn

PHP:  array_slice($arr, 1, 3);
来源：http://ky.hahajie.cn

JS:   arr.slice(1, 4);
来源：http://el.huanxung.cn

TS:   arr.slice(1, 4);
来源：http://ii.lnxyls.cn

Java: list.subList(1, 4);
来源：http://wh.panjiajie.cn

Go:   arr[1:4]
来源：http://fu.muxihuayi.cn

Ruby: arr[1, 3]
来源：http://in.muxihuayi.cn

C#:   list.GetRange(1, 3);
来源：http://lj.chemitech.net.cn

[D08] 合并两个数组
来源：http://so.gzmigu.cn

Py:   a + b;  a.extend(b)
来源：http://se.hnjuh.cn

PHP:  array_merge($a, $b);
来源：http://ny.panjiajie.cn

JS:   [...a, ...b];  a.concat(b);
来源：http://nw.newstarts.cn

TS:   [...a, ...b];
来源：http://sb.jctech888.com.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://im.asd995.cn

Go:   append(a, b...)
来源：http://zg.shtwfgs.cn

Ruby: a + b;  a.concat(b)
来源：http://cz.muxihuayi.cn

C#:   a.Concat(b).ToList()
来源：http://zg.jctech888.com.cn

[D09] 排序（升序）
来源：http://xy.nszjky.cn

Py:   sorted(arr);  arr.sort()
来源：http://mf.jctech888.com.cn

PHP:  sort($arr);
来源：http://sk.wgjwhj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://zk.huixiangedu.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://id.chemitech.net.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://bj.shxzukj.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://ku.huanxung.cn

Ruby: arr.sort
来源：http://vo.haigaiapp.cn

C#:   list.Sort();
来源：http://ma.521024.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://iq.shxzskj.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ec.jianghongdianzi.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://ga.szsharing.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://cw.nszjky.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://il.newstarts.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://aa.huanxung.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://kz.bjjhwx.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://qa.jianghongdianzi.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://ol.newstarts.cn

[D11] 反转数组
来源：http://mh.muxihuayi.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qv.bjjhwx.cn

PHP:  array_reverse($arr);
来源：http://zo.chemitech.net.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://or.colortex.cn

TS:   [...arr].reverse();
来源：http://vw.huixiangedu.cn

Java: Collections.reverse(list);
来源：http://ww.wgjwhj.cn

Go:   slices.Reverse(arr)
来源：http://gv.hnjuh.cn

Ruby: arr.reverse
来源：http://cs.huixinmuqiang.cn

C#:   list.Reverse();
来源：http://kz.shtwfgs.cn

[D12] 查找元素下标
来源：http://lg.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://qr.huanxung.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://rc.hnjuh.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xl.521024.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ar.shtwfgs.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://zf.huixiangedu.cn

Go:   slices.Index(arr, x)
来源：http://oj.shtwfgs.cn

Ruby: arr.index(x)
来源：http://qe.nszjky.cn

C#:   list.IndexOf(x);
来源：http://ow.hahajie.cn

[D13] 过滤（保留满足条件的）
来源：http://vi.shxzskj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ev.szsharing.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ah.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://es.yuexingan06.cn

TS:   arr.filter(x => x > 3)
来源：http://zb.szxytkj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://su.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://ml.huanxung.cn

Ruby: arr.select { |x| x > 3 }
来源：http://iq.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://vq.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://sb.wgjwhj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nm.nicolike.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uq.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://sl.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://ud.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://uf.chemitech.net.cn

Go:   // 手写循环
来源：http://pb.panjiajie.cn

Ruby: arr.map { |x| x * 2 }
来源：http://qq.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://zg.colortex.cn

[D15] 去重
来源：http://ou.newstarts.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://ys.muxihuayi.cn

PHP:  array_unique($arr);
来源：http://hf.lnxyls.cn

JS:   [...new Set(arr)]
来源：http://uk.hnjuh.cn

TS:   [...new Set(arr)]
来源：http://ln.shtwfgs.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://ws.9csxet.cn

Go:   // 用 map[T]struct{} 手写
来源：http://sv.521024.cn

Ruby: arr.uniq
来源：http://jp.jianghongdianzi.cn

C#:   list.Distinct().ToList()
来源：http://lm.521024.cn

[D16] 求和与平均值
来源：http://lj.szxytkj.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://uo.huanxung.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://sp.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://fz.jctech888.com.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://xa.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://iq.asd995.cn

Go:   // 手写循环累加
来源：http://kw.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cb.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://lm.lnxyls.cn

[D17] 最大值与最小值
来源：http://ca.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://gw.huanxung.cn

PHP:  max($arr);  min($arr);
来源：http://bo.haigaiapp.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ra.szsharing.cn

TS:   Math.max(...arr);
来源：http://pw.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://zx.panjiajie.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ac.colortex.cn

Ruby: arr.max;  arr.min
来源：http://ia.chemitech.net.cn

C#:   list.Max();  list.Min()
来源：http://yy.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://sb.shtwfgs.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ay.wgjwhj.cn

PHP:  array_merge(...$nested);
来源：http://iv.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://sk.chemitech.net.cn

TS:   nested.flat();
来源：http://na.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://pq.hahajie.cn

Go:   // 手写双层循环
来源：http://tr.yuexingan06.cn

Ruby: nested.flatten
来源：http://rl.shxzskj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://so.shtwfgs.cn

[D19] 按字段分组
来源：http://vz.asd995.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://fb.gzmigu.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dk.huixiangedu.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://iq.9csxet.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://bb.colortex.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://tj.asd995.cn

Go:   // 手写 map[string][]T
来源：http://ux.szxytkj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://te.9csxet.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uj.9csxet.cn

[D20] 统计每个元素出现次数
来源：http://zo.shxzukj.cn

Py:   Counter(arr)
来源：http://mp.szxytkj.cn

PHP:  array_count_values($arr);
来源：http://pi.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://nv.nicolike.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://st.muxihuayi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://yn.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://iy.nszjky.cn

Ruby: arr.tally
来源：http://hx.yuexingan06.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gt.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://qt.szxytkj.cn

Py:   x in arr
来源：http://hn.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://yh.szsharing.cn

JS:   arr.includes(x)
来源：http://ow.521024.cn

TS:   arr.includes(x)
来源：http://ny.asd995.cn

Java: list.contains(x)
来源：http://pd.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://ko.shtwfgs.cn

Ruby: arr.include?(x)
来源：http://do.hahajie.cn

C#:   list.Contains(x)
来源：http://xz.shxzskj.cn

[D22] 复制数组（避免共享引用）
来源：http://su.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oh.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ni.newstarts.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://kk.haigaiapp.cn

TS:   [...arr];
来源：http://vr.huixiangedu.cn

Java: new ArrayList<>(list);
来源：http://bq.hahajie.cn

Go:   copied := append([]int(nil), arr...)
来源：http://se.colortex.cn

Ruby: arr.dup;  arr.clone
来源：http://ht.521024.cn

C#:   new List<int>(list);
来源：http://bf.huanxung.cn

[D23] reduce 累积计算
来源：http://iw.wgjwhj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://cd.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ef.huixinmuqiang.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sy.chemitech.net.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://uo.chemitech.net.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://oy.haigaiapp.cn

Go:   // 手写循环
来源：http://hn.nicolike.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sz.szxytkj.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://pr.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://om.huixinmuqiang.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://bm.gzmigu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://cz.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://fq.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://my.muxihuayi.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xx.bjjhwx.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bh.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://je.panjiajie.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wc.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://sg.shxzukj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://an.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://gt.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ed.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cv.gzmigu.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://df.wgjwhj.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ea.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://of.shtwfgs.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://xd.jianghongdianzi.cn

[D26] 数组转字符串
来源：http://yc.jctech888.com.cn

Py:   ", ".join(map(str, arr))
来源：http://cr.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://jb.huixiangedu.cn

JS:   arr.join(", ")
来源：http://de.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://zu.9csxet.cn

Java: String.join(", ", list)
来源：http://vd.hnjuh.cn

Go:   strings.Join(strs, ", ")
来源：http://bp.haigaiapp.cn

Ruby: arr.join(", ")
来源：http://zw.huanxung.cn

C#:   string.Join(", ", list)
来源：http://gd.haigaiapp.cn

================================================================================
来源：http://rr.jianghongdianzi.cn

E. 字符串处理
来源：http://mt.lnxyls.cn

================================================================================
来源：http://cp.huixiangedu.cn

[E01] 拼接字符串
来源：http://zh.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://am.yuntaijiaju.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://oi.huixinmuqiang.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://eq.nicolike.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cw.asd995.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ut.nszjky.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://on.nicolike.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://gu.gzmigu.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yi.9csxet.cn

[E02] 重复字符串
来源：http://kq.haigaiapp.cn

Py:   "ab" * 3
来源：http://ng.shxzskj.cn

PHP:  str_repeat("ab", 3);
来源：http://og.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://ns.colortex.cn

TS:   "ab".repeat(3)
来源：http://fu.gzmigu.cn

Java: "ab".repeat(3)
来源：http://cg.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://fe.asd995.cn

Ruby: "ab" * 3
来源：http://bc.hnjuh.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rg.nszjky.cn

[E03] 截取子串
来源：http://tm.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://yo.bookmarksfly.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dr.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wi.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://rt.hnjuh.cn

Java: s.substring(1, 4)
来源：http://dd.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://my.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cp.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://qf.shxzskj.cn

[E04] 查找子串位置
来源：http://se.hnjuh.cn

Py:   s.find("x");  s.index("x")
来源：http://ka.asd995.cn

PHP:  strpos($s, "x");
来源：http://gs.yuntaijiaju.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://jg.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://fe.szxytkj.cn

Java: s.indexOf("x")
来源：http://it.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://to.shxzukj.cn

Ruby: s.index("x")
来源：http://ym.gzmigu.cn

C#:   s.IndexOf("x")
来源：http://tr.hahajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ip.bookmarksfly.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://gg.colortex.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zi.muxihuayi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://qx.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fd.yuntaijiaju.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hk.wgjwhj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://bp.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wk.hnjuh.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ij.chemitech.net.cn

[E06] 替换子串
来源：http://ey.szsharing.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vp.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://sf.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ev.nszjky.cn

TS:   s.replaceAll("a", "b")
来源：http://na.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ph.lnxyls.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yd.newstarts.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nr.colortex.cn

C#:   s.Replace("a", "b")
来源：http://jj.huanxung.cn

[E07] 按分隔符拆分
来源：http://on.hnjuh.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://xi.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://rc.lnxyls.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://te.yuntaijiaju.cn

TS:   s.split(",")
来源：http://mp.jctech888.com.cn

Java: s.split(",");  s.split("\\s+")
来源：http://nf.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://lf.521024.cn

Ruby: s.split(",");  s.split
来源：http://bo.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://sk.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://lw.9csxet.cn

Py:   ",".join(items)
来源：http://gf.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://ps.shxzukj.cn

JS:   items.join(",")
来源：http://xp.colortex.cn

TS:   items.join(",")
来源：http://zr.lnxyls.cn

Java: String.join(",", items)
来源：http://as.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://cc.bookmarksfly.cn

Ruby: items.join(",")
来源：http://vq.shtwfgs.cn

C#:   string.Join(",", items)
来源：http://nq.huixinmuqiang.cn

[E09] 去除所有空白字符
来源：http://yk.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://to.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qc.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://vm.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://nb.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://he.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://bx.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bx.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mu.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://nq.huanxung.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pq.yuexingan06.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ir.521024.cn

JS:   "7".padStart(3, "0")
来源：http://ob.lnxyls.cn

TS:   "7".padStart(3, "0")
来源：http://uf.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://os.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hd.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ti.bookmarksfly.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bb.9csxet.cn

[E11] 反转字符串
来源：http://vv.huixiangedu.cn

Py:   s[::-1]
来源：http://tz.shtwfgs.cn

PHP:  strrev($s);
来源：http://hm.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://iy.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://tx.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ez.huanxung.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://jf.shxzskj.cn

Ruby: s.reverse
来源：http://xl.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://lc.bjjhwx.cn

[E12] 统计某字符出现次数
来源：http://pg.newstarts.cn

Py:   s.count("a")
来源：http://fr.yuntaijiaju.cn


<!-- 参考信息 -->