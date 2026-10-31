代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://ra.yuntaijiaju.cn

TS:   [...a, ...b];
来源：http://gz.521024.cn

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://vj.muxihuayi.cn

Go:   append(a, b...)
来源：http://yx.newstarts.cn

Ruby: a + b;  a.concat(b)
来源：http://gu.huixinmuqiang.cn

C#:   a.Concat(b).ToList()
来源：http://jz.huixiangedu.cn

[D09] 排序（升序）
来源：http://uk.chemitech.net.cn

Py:   sorted(arr);  arr.sort()
来源：http://rw.nszjky.cn

PHP:  sort($arr);
来源：http://sk.521024.cn

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://al.newstarts.cn

TS:   [...arr].sort((x, y) => x - y);
来源：http://cs.newstarts.cn

Java: Collections.sort(list);  list.sort(null);
来源：http://ba.newstarts.cn

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://db.huixinmuqiang.cn

Ruby: arr.sort
来源：http://tq.huanxung.cn

C#:   list.Sort();
来源：http://jy.gzmigu.cn

[D10] 自定义排序（按字段 / 多条件）
来源：http://fv.nicolike.cn

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://xt.asd995.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://cf.hahajie.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wj.shtwfgs.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://dh.hahajie.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://vb.shxzukj.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://ua.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://nm.yuntaijiaju.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://fi.nicolike.cn

[D11] 反转数组
来源：http://mt.shtwfgs.cn

Py:   arr[::-1];  arr.reverse()
来源：http://xu.chemitech.net.cn

PHP:  array_reverse($arr);
来源：http://zy.jctech888.com.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mk.nicolike.cn

TS:   [...arr].reverse();
来源：http://ke.lnxyls.cn

Java: Collections.reverse(list);
来源：http://qk.colortex.cn

Go:   slices.Reverse(arr)
来源：http://tk.nszjky.cn

Ruby: arr.reverse
来源：http://uz.nicolike.cn

C#:   list.Reverse();
来源：http://he.wgjwhj.cn

[D12] 查找元素下标
来源：http://mp.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://pv.bjjhwx.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://kt.szsharing.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hp.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://af.asd995.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://oz.newstarts.cn

Go:   slices.Index(arr, x)
来源：http://fn.nszjky.cn

Ruby: arr.index(x)
来源：http://kt.asd995.cn

C#:   list.IndexOf(x);
来源：http://nw.huixiangedu.cn

[D13] 过滤（保留满足条件的）
来源：http://ac.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mj.asd995.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mi.chemitech.net.cn

JS:   arr.filter(x => x > 3)
来源：http://yn.szxytkj.cn

TS:   arr.filter(x => x > 3)
来源：http://vj.wgjwhj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://gy.huanxung.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://vh.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ep.yuexingan06.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wh.bookmarksfly.cn

[D14] 映射转换（每个元素变形）
来源：http://ca.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://gi.wgjwhj.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://fj.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://hs.yuexingan06.cn

TS:   arr.map(x => x * 2)
来源：http://aw.9csxet.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ga.newstarts.cn

Go:   // 手写循环
来源：http://zz.shtwfgs.cn

Ruby: arr.map { |x| x * 2 }
来源：http://rm.asd995.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://yg.szxytkj.cn

[D15] 去重
来源：http://vu.bjjhwx.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://yd.hnjuh.cn

PHP:  array_unique($arr);
来源：http://ee.asd995.cn

JS:   [...new Set(arr)]
来源：http://vd.jctech888.com.cn

TS:   [...new Set(arr)]
来源：http://ub.wgjwhj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://rj.yuntaijiaju.cn

Go:   // 用 map[T]struct{} 手写
来源：http://wi.bookmarksfly.cn

Ruby: arr.uniq
来源：http://is.nszjky.cn

C#:   list.Distinct().ToList()
来源：http://bj.nszjky.cn

[D16] 求和与平均值
来源：http://la.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://kp.nicolike.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ac.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ow.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wd.lnxyls.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yr.huanxung.cn

Go:   // 手写循环累加
来源：http://bp.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ww.huanxung.cn

C#:   list.Sum();  list.Average()
来源：http://tx.shtwfgs.cn

[D17] 最大值与最小值
来源：http://gx.szsharing.cn

Py:   max(arr);  min(arr)
来源：http://gv.colortex.cn

PHP:  max($arr);  min($arr);
来源：http://rx.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://yy.chemitech.net.cn

TS:   Math.max(...arr);
来源：http://en.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://hu.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://fr.szxytkj.cn

Ruby: arr.max;  arr.min
来源：http://ma.panjiajie.cn

C#:   list.Max();  list.Min()
来源：http://bh.chemitech.net.cn

[D18] 扁平化嵌套数组
来源：http://qs.gzmigu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://sj.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://va.hnjuh.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://od.panjiajie.cn

TS:   nested.flat();
来源：http://xx.huixinmuqiang.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://fe.bjjhwx.cn

Go:   // 手写双层循环
来源：http://tn.bookmarksfly.cn

Ruby: nested.flatten
来源：http://rf.hahajie.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ao.jctech888.com.cn

[D19] 按字段分组
来源：http://ks.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://yq.shxzskj.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://ha.haigaiapp.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://qv.szxytkj.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ol.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://gs.bookmarksfly.cn

Go:   // 手写 map[string][]T
来源：http://xd.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://jr.colortex.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ak.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://jm.shxzskj.cn

Py:   Counter(arr)
来源：http://hl.wgjwhj.cn

PHP:  array_count_values($arr);
来源：http://vp.panjiajie.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://pb.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://na.szxytkj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://kg.szsharing.cn

Go:   // 手写 map[T]int
来源：http://uk.muxihuayi.cn

Ruby: arr.tally
来源：http://lb.muxihuayi.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://pw.chemitech.net.cn

[D21] 判断是否包含某元素
来源：http://tv.huixinmuqiang.cn

Py:   x in arr
来源：http://wx.hahajie.cn

PHP:  in_array($x, $arr, true);
来源：http://iz.colortex.cn

JS:   arr.includes(x)
来源：http://ps.huixiangedu.cn

TS:   arr.includes(x)
来源：http://tw.lnxyls.cn

Java: list.contains(x)
来源：http://sz.colortex.cn

Go:   slices.Contains(arr, x)
来源：http://sa.yuntaijiaju.cn

Ruby: arr.include?(x)
来源：http://ay.nszjky.cn

C#:   list.Contains(x)
来源：http://ry.asd995.cn

[D22] 复制数组（避免共享引用）
来源：http://vg.shxzukj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yv.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://fc.asd995.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://yq.huanxung.cn

TS:   [...arr];
来源：http://qm.yuntaijiaju.cn

Java: new ArrayList<>(list);
来源：http://oa.lnxyls.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ro.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://cn.huanxung.cn

C#:   new List<int>(list);
来源：http://lv.nicolike.cn

[D23] reduce 累积计算
来源：http://hl.yuntaijiaju.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xl.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nv.huixiangedu.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://af.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dv.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://pl.9csxet.cn

Go:   // 手写循环
来源：http://js.hahajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ay.nicolike.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ps.gzmigu.cn

[D24] 字典 / Map 基本操作
来源：http://wc.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://re.shxzukj.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xe.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ju.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ta.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://up.nszjky.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shxzukj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://bj.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ar.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://ba.shxzskj.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ry.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://sh.hahajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://xk.wgjwhj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://cc.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://az.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://lv.yuexingan06.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://uj.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://oy.szsharing.cn

[D26] 数组转字符串
来源：http://dh.yuexingan06.cn

Py:   ", ".join(map(str, arr))
来源：http://vh.huanxung.cn

PHP:  implode(", ", $arr);
来源：http://nl.nicolike.cn

JS:   arr.join(", ")
来源：http://ax.hnjuh.cn

TS:   arr.join(", ")
来源：http://nf.muxihuayi.cn

Java: String.join(", ", list)
来源：http://ag.chemitech.net.cn

Go:   strings.Join(strs, ", ")
来源：http://me.lnxyls.cn

Ruby: arr.join(", ")
来源：http://hh.szsharing.cn

C#:   string.Join(", ", list)
来源：http://tm.chemitech.net.cn

================================================================================
来源：http://gf.muxihuayi.cn

E. 字符串处理
来源：http://mv.9csxet.cn

================================================================================
来源：http://in.nicolike.cn

[E01] 拼接字符串
来源：http://tq.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://qn.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wx.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://sn.huixiangedu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wy.shtwfgs.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zp.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uh.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://id.yuexingan06.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hq.shxzukj.cn

[E02] 重复字符串
来源：http://st.bjjhwx.cn

Py:   "ab" * 3
来源：http://xm.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://ss.asd995.cn

JS:   "ab".repeat(3)
来源：http://jr.wgjwhj.cn

TS:   "ab".repeat(3)
来源：http://ej.szxytkj.cn

Java: "ab".repeat(3)
来源：http://kx.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://ap.nicolike.cn

Ruby: "ab" * 3
来源：http://oq.jianghongdianzi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xa.nszjky.cn

[E03] 截取子串
来源：http://op.9csxet.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ud.bjjhwx.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ow.521024.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://km.nicolike.cn

TS:   s.slice(1, 4)
来源：http://bg.shxzukj.cn

Java: s.substring(1, 4)
来源：http://ly.bookmarksfly.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://lc.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ko.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://xv.yuntaijiaju.cn

[E04] 查找子串位置
来源：http://bd.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://vi.huanxung.cn

PHP:  strpos($s, "x");
来源：http://th.yuexingan06.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://pq.jctech888.com.cn

TS:   s.indexOf("x")
来源：http://zi.huixinmuqiang.cn

Java: s.indexOf("x")
来源：http://zk.521024.cn

Go:   strings.Index(s, "x")
来源：http://fp.wgjwhj.cn

Ruby: s.index("x")
来源：http://pn.newstarts.cn

C#:   s.IndexOf("x")
来源：http://zf.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mr.panjiajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jz.yuntaijiaju.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hy.bjjhwx.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sb.gzmigu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xy.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ci.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ab.hahajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lp.szxytkj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://nf.shxzskj.cn

[E06] 替换子串
来源：http://lp.wgjwhj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://lx.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://en.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://vq.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://gx.9csxet.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kk.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://iy.gzmigu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ct.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://ee.huanxung.cn

[E07] 按分隔符拆分
来源：http://ll.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://qp.haigaiapp.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ah.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://et.jianghongdianzi.cn

TS:   s.split(",")
来源：http://ct.huixinmuqiang.cn

Java: s.split(",");  s.split("\\s+")
来源：http://tm.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://fo.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://ma.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://gv.hahajie.cn

[E08] 数组按分隔符合并
来源：http://uk.gzmigu.cn

Py:   ",".join(items)
来源：http://hv.szxytkj.cn

PHP:  implode(",", $items);
来源：http://ij.shxzskj.cn

JS:   items.join(",")
来源：http://ds.shxzukj.cn

TS:   items.join(",")
来源：http://dt.wgjwhj.cn

Java: String.join(",", items)
来源：http://dc.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://cu.jctech888.com.cn

Ruby: items.join(",")
来源：http://rs.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://de.hahajie.cn

[E09] 去除所有空白字符
来源：http://el.chemitech.net.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ob.nszjky.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mc.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://tz.newstarts.cn

TS:   s.replace(/\s+/g, "")
来源：http://nz.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://yr.colortex.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wo.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zy.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kq.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://or.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nr.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qi.muxihuayi.cn

JS:   "7".padStart(3, "0")
来源：http://rz.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://ti.szsharing.cn

Java: String.format("%03d", 7)
来源：http://ud.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://wi.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://fq.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mk.521024.cn

[E11] 反转字符串
来源：http://de.shxzukj.cn

Py:   s[::-1]
来源：http://wk.nicolike.cn

PHP:  strrev($s);
来源：http://mh.panjiajie.cn

JS:   [...s].reverse().join("")
来源：http://nr.yuexingan06.cn

TS:   [...s].reverse().join("")
来源：http://av.shxzukj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gs.muxihuayi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ir.hahajie.cn

Ruby: s.reverse
来源：http://vw.9csxet.cn

C#:   new string(s.Reverse().ToArray())
来源：http://tl.colortex.cn

[E12] 统计某字符出现次数
来源：http://fj.hnjuh.cn

Py:   s.count("a")
来源：http://xh.lnxyls.cn

PHP:  substr_count($s, "a");
来源：http://vd.9csxet.cn

JS:   s.split("a").length - 1
来源：http://ko.shxzukj.cn

TS:   s.split("a").length - 1
来源：http://wm.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ih.panjiajie.cn

Go:   strings.Count(s, "a")
来源：http://rd.bjjhwx.cn

Ruby: s.count("a")
来源：http://yk.nicolike.cn

C#:   s.Count(c => c == 'a')
来源：http://uq.yuntaijiaju.cn

[E13] 逐字符遍历
来源：http://cy.szsharing.cn

Py:   for ch in s: print(ch)
来源：http://yp.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cy.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fq.jctech888.com.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hb.gzmigu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://sh.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wp.colortex.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xu.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ns.521024.cn

[E14] URL 编码与 Base64
来源：http://qk.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ps.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://zv.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ai.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://us.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://po.lnxyls.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ld.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lr.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fd.szsharing.cn

[E15] HTML 转义 / 反转义
来源：http://zm.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pz.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://yx.jianghongdianzi.cn


<!-- 参考信息 -->