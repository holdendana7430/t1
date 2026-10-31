代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://bh.lnxyls.cn

TS:   [...a, ...b];
来源：http://ed.colortex.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://ou.hnjuh.cn

Go:   append(a, b...)
来源：http://qh.chemitech.net.cn

Ruby: a + b;  a.concat(b)
来源：http://by.shxzskj.cn

C#:   a.Concat(b).ToList()
来源：http://dm.gzmigu.cn

[D09] 排序（升序）
来源：http://en.huixiangedu.cn

Py:   sorted(arr);  arr.sort()
来源：http://sv.shtwfgs.cn

PHP:  sort($arr);
来源：http://tv.shxzskj.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://ll.nszjky.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://ft.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ii.shtwfgs.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://kx.szxytkj.cn

Ruby: arr.sort
来源：http://un.colortex.cn

C#:   list.Sort();
来源：http://ds.yuexingan06.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://sv.newstarts.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://zd.shxzukj.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://kq.wgjwhj.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://te.muxihuayi.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hw.szxytkj.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://th.haigaiapp.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://bs.huixinmuqiang.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://ab.shxzskj.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://bt.newstarts.cn

[D11] 反转数组
来源：http://el.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://cr.szxytkj.cn

PHP:  array_reverse($arr);
来源：http://xo.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mr.jctech888.com.cn

TS:   [...arr].reverse();
来源：http://wv.wgjwhj.cn

Java: Collections.reverse(list);
来源：http://sr.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://cc.muxihuayi.cn

Ruby: arr.reverse
来源：http://bu.newstarts.cn

C#:   list.Reverse();
来源：http://iu.hahajie.cn

[D12] 查找元素下标
来源：http://oz.bjjhwx.cn

Py:   arr.index(x);  x in arr
来源：http://dz.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://ee.wgjwhj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://oe.nicolike.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ak.szsharing.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ok.lnxyls.cn

Go:   slices.Index(arr, x)
来源：http://zv.521024.cn

Ruby: arr.index(x)
来源：http://iw.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://mp.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://ec.chemitech.net.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ui.yuexingan06.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://uf.bookmarksfly.cn

JS:   arr.filter(x => x > 3)
来源：http://fa.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://js.haigaiapp.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://tq.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://nj.yuntaijiaju.cn

Ruby: arr.select { |x| x > 3 }
来源：http://hc.colortex.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://fl.newstarts.cn

[D14] 映射转换（每个元素变形）
来源：http://jn.colortex.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://lq.jctech888.com.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uz.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://hi.bjjhwx.cn

TS:   arr.map(x => x * 2)
来源：http://rj.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://wj.newstarts.cn

Go:   // 手写循环
来源：http://ox.asd995.cn

Ruby: arr.map { |x| x * 2 }
来源：http://wx.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aw.chemitech.net.cn

[D15] 去重
来源：http://yz.jctech888.com.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://gm.colortex.cn

PHP:  array_unique($arr);
来源：http://le.shxzukj.cn

JS:   [...new Set(arr)]
来源：http://og.yuntaijiaju.cn

TS:   [...new Set(arr)]
来源：http://qx.szsharing.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://yd.jianghongdianzi.cn

Go:   // 用 map[T]struct{} 手写
来源：http://us.szxytkj.cn

Ruby: arr.uniq
来源：http://bb.bjjhwx.cn

C#:   list.Distinct().ToList()
来源：http://hh.shxzukj.cn

[D16] 求和与平均值
来源：http://go.jctech888.com.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ij.szxytkj.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://tx.bjjhwx.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://zv.yuexingan06.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://qr.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ng.shxzukj.cn

Go:   // 手写循环累加
来源：http://ca.huixiangedu.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://iv.huixiangedu.cn

C#:   list.Sum();  list.Average()
来源：http://rt.521024.cn

[D17] 最大值与最小值
来源：http://vt.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://xx.panjiajie.cn

PHP:  max($arr);  min($arr);
来源：http://rw.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://jy.nszjky.cn

TS:   Math.max(...arr);
来源：http://wg.muxihuayi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://bl.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://dh.shxzukj.cn

Ruby: arr.max;  arr.min
来源：http://ty.9csxet.cn

C#:   list.Max();  list.Min()
来源：http://ua.asd995.cn

[D18] 扁平化嵌套数组
来源：http://el.lnxyls.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sn.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://ut.nicolike.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mq.colortex.cn

TS:   nested.flat();
来源：http://az.shtwfgs.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lt.bookmarksfly.cn

Go:   // 手写双层循环
来源：http://tr.jctech888.com.cn

Ruby: nested.flatten
来源：http://ss.huixinmuqiang.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://te.nicolike.cn

[D19] 按字段分组
来源：http://pw.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://kp.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ox.wgjwhj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zr.szsharing.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ci.panjiajie.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ay.yuexingan06.cn

Go:   // 手写 map[string][]T
来源：http://nn.521024.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://nv.521024.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://uv.colortex.cn

[D20] 统计每个元素出现次数
来源：http://ui.huixiangedu.cn

Py:   Counter(arr)
来源：http://pc.9csxet.cn

PHP:  array_count_values($arr);
来源：http://qo.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://az.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tg.lnxyls.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://be.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://jx.szxytkj.cn

Ruby: arr.tally
来源：http://ro.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://qg.yuntaijiaju.cn

[D21] 判断是否包含某元素
来源：http://nd.nicolike.cn

Py:   x in arr
来源：http://yo.nszjky.cn

PHP:  in_array($x, $arr, true);
来源：http://jo.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://hs.huixinmuqiang.cn

TS:   arr.includes(x)
来源：http://jy.hnjuh.cn

Java: list.contains(x)
来源：http://wg.shxzskj.cn

Go:   slices.Contains(arr, x)
来源：http://sl.lnxyls.cn

Ruby: arr.include?(x)
来源：http://zo.muxihuayi.cn

C#:   list.Contains(x)
来源：http://is.yuexingan06.cn

[D22] 复制数组（避免共享引用）
来源：http://cx.hnjuh.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://sb.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ee.chemitech.net.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://dd.newstarts.cn

TS:   [...arr];
来源：http://br.hnjuh.cn

Java: new ArrayList<>(list);
来源：http://zg.hnjuh.cn

Go:   copied := append([]int(nil), arr...)
来源：http://oj.muxihuayi.cn

Ruby: arr.dup;  arr.clone
来源：http://gm.bjjhwx.cn

C#:   new List<int>(list);
来源：http://uq.shxzskj.cn

[D23] reduce 累积计算
来源：http://yo.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xe.szsharing.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ag.muxihuayi.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ny.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ky.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://or.lnxyls.cn

Go:   // 手写循环
来源：http://za.yuexingan06.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ew.gzmigu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ne.bjjhwx.cn

[D24] 字典 / Map 基本操作
来源：http://ax.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hr.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hl.bookmarksfly.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://lu.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qr.shxzskj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ll.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://bp.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://oc.szsharing.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jh.haigaiapp.cn

[D25] Set 集合去重与交并差
来源：http://av.haigaiapp.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ov.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tk.newstarts.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ng.bjjhwx.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://xx.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://yd.gzmigu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://vu.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oq.asd995.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://eq.muxihuayi.cn

[D26] 数组转字符串
来源：http://di.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://uh.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://np.muxihuayi.cn

JS:   arr.join(", ")
来源：http://ef.shtwfgs.cn

TS:   arr.join(", ")
来源：http://wy.asd995.cn

Java: String.join(", ", list)
来源：http://ba.jctech888.com.cn

Go:   strings.Join(strs, ", ")
来源：http://uw.newstarts.cn

Ruby: arr.join(", ")
来源：http://wu.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://lc.nicolike.cn

================================================================================
来源：http://sd.panjiajie.cn

E. 字符串处理
来源：http://wm.yuntaijiaju.cn

================================================================================
来源：http://hp.hahajie.cn

[E01] 拼接字符串
来源：http://nm.shxzskj.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xi.bjjhwx.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://se.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vd.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://re.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cq.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://vz.huanxung.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://da.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wa.shxzukj.cn

[E02] 重复字符串
来源：http://nl.shxzskj.cn

Py:   "ab" * 3
来源：http://hd.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://ju.huixinmuqiang.cn

JS:   "ab".repeat(3)
来源：http://in.bookmarksfly.cn

TS:   "ab".repeat(3)
来源：http://as.gzmigu.cn

Java: "ab".repeat(3)
来源：http://yn.chemitech.net.cn

Go:   strings.Repeat("ab", 3)
来源：http://jt.jianghongdianzi.cn

Ruby: "ab" * 3
来源：http://ak.asd995.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xe.szxytkj.cn

[E03] 截取子串
来源：http://cc.lnxyls.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://sn.chemitech.net.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hx.muxihuayi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://sg.wgjwhj.cn

TS:   s.slice(1, 4)
来源：http://ak.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://hj.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pp.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ma.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ty.gzmigu.cn

[E04] 查找子串位置
来源：http://gs.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://pc.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://ps.szsharing.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ff.lnxyls.cn

TS:   s.indexOf("x")
来源：http://py.newstarts.cn

Java: s.indexOf("x")
来源：http://tj.huixinmuqiang.cn

Go:   strings.Index(s, "x")
来源：http://qo.haigaiapp.cn

Ruby: s.index("x")
来源：http://li.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://ua.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rk.muxihuayi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fq.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xr.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xq.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://oc.bjjhwx.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pd.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cu.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rf.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mb.lnxyls.cn

[E06] 替换子串
来源：http://uo.yuexingan06.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ia.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://my.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ej.lnxyls.cn

TS:   s.replaceAll("a", "b")
来源：http://sv.521024.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://py.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mo.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xu.muxihuayi.cn

C#:   s.Replace("a", "b")
来源：http://pl.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://ly.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kk.yuexingan06.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gm.shtwfgs.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ng.nszjky.cn

TS:   s.split(",")
来源：http://ru.szxytkj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hx.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ry.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://aj.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://eo.gzmigu.cn

[E08] 数组按分隔符合并
来源：http://uc.shxzukj.cn

Py:   ",".join(items)
来源：http://pb.521024.cn

PHP:  implode(",", $items);
来源：http://zb.huanxung.cn

JS:   items.join(",")
来源：http://rh.newstarts.cn

TS:   items.join(",")
来源：http://hh.yuntaijiaju.cn

Java: String.join(",", items)
来源：http://id.jctech888.com.cn

Go:   strings.Join(items, ",")
来源：http://sb.bjjhwx.cn

Ruby: items.join(",")
来源：http://iz.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://ir.shxzukj.cn

[E09] 去除所有空白字符
来源：http://qr.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pv.huanxung.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ox.hnjuh.cn

JS:   s.replace(/\s+/g, "")
来源：http://rw.haigaiapp.cn

TS:   s.replace(/\s+/g, "")
来源：http://ec.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://tt.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://mj.jianghongdianzi.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uj.9csxet.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cb.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://is.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://oe.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ai.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://xj.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://qk.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://mo.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jr.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ig.huixiangedu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://dq.521024.cn

[E11] 反转字符串
来源：http://ja.chemitech.net.cn

Py:   s[::-1]
来源：http://od.9csxet.cn

PHP:  strrev($s);
来源：http://ax.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://wr.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://bb.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gr.shxzukj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fa.panjiajie.cn

Ruby: s.reverse
来源：http://sb.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ej.haigaiapp.cn

[E12] 统计某字符出现次数
来源：http://ss.nszjky.cn

Py:   s.count("a")
来源：http://wb.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://fn.asd995.cn

JS:   s.split("a").length - 1
来源：http://wd.jctech888.com.cn

TS:   s.split("a").length - 1
来源：http://uq.chemitech.net.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hg.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://iy.muxihuayi.cn

Ruby: s.count("a")
来源：http://qy.chemitech.net.cn

C#:   s.Count(c => c == 'a')
来源：http://hg.asd995.cn

[E13] 逐字符遍历
来源：http://aq.asd995.cn

Py:   for ch in s: print(ch)
来源：http://dy.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://iq.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://va.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xh.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vi.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lb.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://sy.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lm.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://zi.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sj.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://on.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://zn.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fr.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://qy.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jb.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oj.huixinmuqiang.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jh.hnjuh.cn

[E15] HTML 转义 / 反转义
来源：http://oc.lnxyls.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pc.shxzukj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bv.hnjuh.cn


<!-- 参考信息 -->