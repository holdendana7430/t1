代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://dz.hnjuh.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://uo.yuexingan06.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://oh.huixiangedu.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://em.huixinmuqiang.cn

[D11] 反转数组
来源：http://ob.nicolike.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ir.jianghongdianzi.cn

PHP:  array_reverse($arr);
来源：http://dy.asd995.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://th.muxihuayi.cn

TS:   [...arr].reverse();
来源：http://pb.lnxyls.cn

Java: Collections.reverse(list);
来源：http://ei.jianghongdianzi.cn

Go:   slices.Reverse(arr)
来源：http://xs.shxzukj.cn

Ruby: arr.reverse
来源：http://tz.szxytkj.cn

C#:   list.Reverse();
来源：http://nx.shtwfgs.cn

[D12] 查找元素下标
来源：http://wh.shxzukj.cn

Py:   arr.index(x);  x in arr
来源：http://fx.haigaiapp.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://eb.yuexingan06.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rf.gzmigu.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://nr.panjiajie.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://ti.yuntaijiaju.cn

Go:   slices.Index(arr, x)
来源：http://ow.szxytkj.cn

Ruby: arr.index(x)
来源：http://qa.shxzukj.cn

C#:   list.IndexOf(x);
来源：http://ps.9csxet.cn

[D13] 过滤（保留满足条件的）
来源：http://cn.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://fc.bookmarksfly.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hv.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://le.newstarts.cn

TS:   arr.filter(x => x > 3)
来源：http://kd.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://iu.muxihuayi.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://fz.521024.cn

Ruby: arr.select { |x| x > 3 }
来源：http://xq.hahajie.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ga.nszjky.cn

[D14] 映射转换（每个元素变形）
来源：http://ui.szsharing.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://nc.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wm.huixinmuqiang.cn

JS:   arr.map(x => x * 2)
来源：http://rh.wgjwhj.cn

TS:   arr.map(x => x * 2)
来源：http://fz.szxytkj.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://kq.jianghongdianzi.cn

Go:   // 手写循环
来源：http://gn.colortex.cn

Ruby: arr.map { |x| x * 2 }
来源：http://my.wgjwhj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://aq.panjiajie.cn

[D15] 去重
来源：http://tm.haigaiapp.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://rx.newstarts.cn

PHP:  array_unique($arr);
来源：http://qe.jianghongdianzi.cn

JS:   [...new Set(arr)]
来源：http://ag.nicolike.cn

TS:   [...new Set(arr)]
来源：http://sf.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://em.shxzukj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://jo.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://re.huixinmuqiang.cn

C#:   list.Distinct().ToList()
来源：http://uv.shtwfgs.cn

[D16] 求和与平均值
来源：http://kd.newstarts.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://nu.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://fa.yuexingan06.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ro.lnxyls.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ox.yuexingan06.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ta.yuntaijiaju.cn

Go:   // 手写循环累加
来源：http://hi.nszjky.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://bl.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://pi.nszjky.cn

[D17] 最大值与最小值
来源：http://hm.huixiangedu.cn

Py:   max(arr);  min(arr)
来源：http://oc.521024.cn

PHP:  max($arr);  min($arr);
来源：http://pb.9csxet.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ca.shxzskj.cn

TS:   Math.max(...arr);
来源：http://tr.chemitech.net.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://kb.shxzskj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ot.wgjwhj.cn

Ruby: arr.max;  arr.min
来源：http://ff.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://tb.shxzukj.cn

[D18] 扁平化嵌套数组
来源：http://rc.jctech888.com.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ha.nicolike.cn

PHP:  array_merge(...$nested);
来源：http://wi.muxihuayi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tv.huixinmuqiang.cn

TS:   nested.flat();
来源：http://ou.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ch.colortex.cn

Go:   // 手写双层循环
来源：http://mf.521024.cn

Ruby: nested.flatten
来源：http://al.521024.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lj.yuntaijiaju.cn

[D19] 按字段分组
来源：http://df.yuntaijiaju.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://cc.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://vl.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://ic.muxihuayi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://rc.jctech888.com.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://lc.huixinmuqiang.cn

Go:   // 手写 map[string][]T
来源：http://ac.wgjwhj.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ff.huixiangedu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://zv.jianghongdianzi.cn

[D20] 统计每个元素出现次数
来源：http://cb.huixinmuqiang.cn

Py:   Counter(arr)
来源：http://sb.gzmigu.cn

PHP:  array_count_values($arr);
来源：http://uz.asd995.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tm.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://ut.wgjwhj.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://gx.szxytkj.cn

Go:   // 手写 map[T]int
来源：http://cr.shxzukj.cn

Ruby: arr.tally
来源：http://th.hahajie.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://xb.9csxet.cn

[D21] 判断是否包含某元素
来源：http://dx.huanxung.cn

Py:   x in arr
来源：http://hd.shxzukj.cn

PHP:  in_array($x, $arr, true);
来源：http://gz.9csxet.cn

JS:   arr.includes(x)
来源：http://mk.panjiajie.cn

TS:   arr.includes(x)
来源：http://ma.shxzskj.cn

Java: list.contains(x)
来源：http://vq.huanxung.cn

Go:   slices.Contains(arr, x)
来源：http://ea.haigaiapp.cn

Ruby: arr.include?(x)
来源：http://ng.chemitech.net.cn

C#:   list.Contains(x)
来源：http://zh.szxytkj.cn

[D22] 复制数组（避免共享引用）
来源：http://ag.nicolike.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qm.jctech888.com.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xi.szxytkj.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://uk.jctech888.com.cn

TS:   [...arr];
来源：http://qg.shxzukj.cn

Java: new ArrayList<>(list);
来源：http://mq.huixinmuqiang.cn

Go:   copied := append([]int(nil), arr...)
来源：http://xe.newstarts.cn

Ruby: arr.dup;  arr.clone
来源：http://hu.9csxet.cn

C#:   new List<int>(list);
来源：http://ec.521024.cn

[D23] reduce 累积计算
来源：http://ou.shtwfgs.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xo.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://xi.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fk.jctech888.com.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://zl.hahajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ep.huixinmuqiang.cn

Go:   // 手写循环
来源：http://ve.521024.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://aw.hnjuh.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://db.chemitech.net.cn

[D24] 字典 / Map 基本操作
来源：http://yy.szxytkj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://dd.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://lm.shxzskj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://la.lnxyls.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://qn.asd995.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wb.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://tq.huixinmuqiang.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mh.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ry.hahajie.cn

[D25] Set 集合去重与交并差
来源：http://mh.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tn.wgjwhj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://nv.muxihuayi.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://en.chemitech.net.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://rv.haigaiapp.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://vg.haigaiapp.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://de.panjiajie.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://kj.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hp.colortex.cn

[D26] 数组转字符串
来源：http://ot.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://wn.wgjwhj.cn

PHP:  implode(", ", $arr);
来源：http://jo.shxzukj.cn

JS:   arr.join(", ")
来源：http://vl.jianghongdianzi.cn

TS:   arr.join(", ")
来源：http://qk.bookmarksfly.cn

Java: String.join(", ", list)
来源：http://vh.bookmarksfly.cn

Go:   strings.Join(strs, ", ")
来源：http://sx.szsharing.cn

Ruby: arr.join(", ")
来源：http://pw.9csxet.cn

C#:   string.Join(", ", list)
来源：http://tf.szsharing.cn

================================================================================
来源：http://eg.huixinmuqiang.cn

E. 字符串处理
来源：http://dr.9csxet.cn

================================================================================
来源：http://yu.panjiajie.cn

[E01] 拼接字符串
来源：http://do.colortex.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://rx.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ca.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://qd.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sa.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://zv.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://tf.huixinmuqiang.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lb.chemitech.net.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://oj.shxzukj.cn

[E02] 重复字符串
来源：http://ac.panjiajie.cn

Py:   "ab" * 3
来源：http://lh.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://zn.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://tt.szsharing.cn

TS:   "ab".repeat(3)
来源：http://yy.yuntaijiaju.cn

Java: "ab".repeat(3)
来源：http://oy.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://xq.nszjky.cn

Ruby: "ab" * 3
来源：http://gj.huixinmuqiang.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://as.szsharing.cn

[E03] 截取子串
来源：http://il.jctech888.com.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://da.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ep.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://xj.huanxung.cn

TS:   s.slice(1, 4)
来源：http://qx.asd995.cn

Java: s.substring(1, 4)
来源：http://is.9csxet.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nb.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://vz.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://ad.hnjuh.cn

[E04] 查找子串位置
来源：http://ts.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://im.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://xa.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ry.panjiajie.cn

TS:   s.indexOf("x")
来源：http://xl.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ic.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://el.jianghongdianzi.cn

Ruby: s.index("x")
来源：http://ya.szsharing.cn

C#:   s.IndexOf("x")
来源：http://qg.jianghongdianzi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://lw.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pn.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ij.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rb.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sp.asd995.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ac.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lc.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://xy.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://rh.yuexingan06.cn

[E06] 替换子串
来源：http://op.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wl.nicolike.cn

PHP:  str_replace("a", "b", $s);
来源：http://uc.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fe.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://mc.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dc.muxihuayi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sa.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://dr.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://bi.yuexingan06.cn

[E07] 按分隔符拆分
来源：http://bu.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hw.szxytkj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gu.hahajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bc.szxytkj.cn

TS:   s.split(",")
来源：http://dp.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://eq.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ov.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://wk.colortex.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ua.jianghongdianzi.cn

[E08] 数组按分隔符合并
来源：http://mw.hnjuh.cn

Py:   ",".join(items)
来源：http://ar.shxzskj.cn

PHP:  implode(",", $items);
来源：http://vn.yuexingan06.cn

JS:   items.join(",")
来源：http://tm.521024.cn

TS:   items.join(",")
来源：http://xm.newstarts.cn

Java: String.join(",", items)
来源：http://hc.yuexingan06.cn

Go:   strings.Join(items, ",")
来源：http://od.panjiajie.cn

Ruby: items.join(",")
来源：http://qz.asd995.cn

C#:   string.Join(",", items)
来源：http://sv.nszjky.cn

[E09] 去除所有空白字符
来源：http://ww.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pd.nicolike.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bj.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://yt.huixiangedu.cn

TS:   s.replace(/\s+/g, "")
来源：http://eb.gzmigu.cn

Java: s.replaceAll("\\s+", "")
来源：http://kh.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://jm.jctech888.com.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ny.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jt.haigaiapp.cn

[E10] 左侧补零 / 定长填充
来源：http://vu.shxzukj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tn.haigaiapp.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hr.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://jn.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://jt.nszjky.cn

Java: String.format("%03d", 7)
来源：http://ms.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kt.shxzskj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://qc.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://au.newstarts.cn

[E11] 反转字符串
来源：http://io.521024.cn

Py:   s[::-1]
来源：http://ko.wgjwhj.cn

PHP:  strrev($s);
来源：http://vv.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://oi.asd995.cn

TS:   [...s].reverse().join("")
来源：http://hb.asd995.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ka.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bb.colortex.cn

Ruby: s.reverse
来源：http://od.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://dd.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://ym.jctech888.com.cn

Py:   s.count("a")
来源：http://th.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://dq.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://kn.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://vb.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dw.shtwfgs.cn

Go:   strings.Count(s, "a")
来源：http://au.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://hk.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://ia.gzmigu.cn

[E13] 逐字符遍历
来源：http://pd.shxzskj.cn

Py:   for ch in s: print(ch)
来源：http://yi.yuntaijiaju.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ke.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://md.szsharing.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sw.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ya.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pp.szsharing.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ju.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://dz.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://fc.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hr.shtwfgs.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jr.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mv.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://na.jianghongdianzi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yb.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ip.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://jo.colortex.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xa.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://sa.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lu.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vf.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ee.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ml.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gp.lnxyls.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oi.wgjwhj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fb.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cp.9csxet.cn

[E16] 数字千分位
来源：http://px.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://st.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://pb.hnjuh.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wd.yuntaijiaju.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://oy.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sh.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://eu.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zx.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://xl.wgjwhj.cn

[E17] 首字母大写
来源：http://tj.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://tu.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sd.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ge.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ri.huanxung.cn


<!-- 参考信息 -->