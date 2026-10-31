代发 wailian999

[D11] 反转数组
来源：http://fh.colortex.cn

Py:   arr[::-1];  arr.reverse()
来源：http://lz.jctech888.com.cn

PHP:  array_reverse($arr);
来源：http://nv.huanxung.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://pm.hnjuh.cn

TS:   [...arr].reverse();
来源：http://xg.haigaiapp.cn

Java: Collections.reverse(list);
来源：http://tz.asd995.cn

Go:   slices.Reverse(arr)
来源：http://tp.yuntaijiaju.cn

Ruby: arr.reverse
来源：http://yl.jctech888.com.cn

C#:   list.Reverse();
来源：http://ii.bookmarksfly.cn

[D12] 查找元素下标
来源：http://uo.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://lb.bookmarksfly.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://bg.chemitech.net.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://tv.shtwfgs.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://db.jctech888.com.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://sw.hnjuh.cn

Go:   slices.Index(arr, x)
来源：http://rv.jianghongdianzi.cn

Ruby: arr.index(x)
来源：http://pl.hnjuh.cn

C#:   list.IndexOf(x);
来源：http://bi.shxzukj.cn

[D13] 过滤（保留满足条件的）
来源：http://cb.yuntaijiaju.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ek.hnjuh.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ld.521024.cn

JS:   arr.filter(x => x > 3)
来源：http://le.bookmarksfly.cn

TS:   arr.filter(x => x > 3)
来源：http://ag.gzmigu.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wn.shxzukj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://iv.wgjwhj.cn

Ruby: arr.select { |x| x > 3 }
来源：http://qd.shxzukj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ks.jianghongdianzi.cn

[D14] 映射转换（每个元素变形）
来源：http://wq.yuntaijiaju.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://en.shtwfgs.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ef.bjjhwx.cn

JS:   arr.map(x => x * 2)
来源：http://dk.chemitech.net.cn

TS:   arr.map(x => x * 2)
来源：http://st.nicolike.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://cf.chemitech.net.cn

Go:   // 手写循环
来源：http://vb.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzmigu.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pp.bjjhwx.cn

[D15] 去重
来源：http://dg.lnxyls.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://la.huixinmuqiang.cn

PHP:  array_unique($arr);
来源：http://mo.huanxung.cn

JS:   [...new Set(arr)]
来源：http://sf.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://ok.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://is.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ci.jianghongdianzi.cn

Ruby: arr.uniq
来源：http://zb.wgjwhj.cn

C#:   list.Distinct().ToList()
来源：http://df.colortex.cn

[D16] 求和与平均值
来源：http://lh.haigaiapp.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://gr.asd995.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ic.asd995.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://is.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ne.hahajie.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://yl.panjiajie.cn

Go:   // 手写循环累加
来源：http://rv.muxihuayi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://vg.bookmarksfly.cn

C#:   list.Sum();  list.Average()
来源：http://ay.nicolike.cn

[D17] 最大值与最小值
来源：http://js.colortex.cn

Py:   max(arr);  min(arr)
来源：http://ts.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://bj.jctech888.com.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://bm.jctech888.com.cn

TS:   Math.max(...arr);
来源：http://zb.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://id.lnxyls.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://on.gzmigu.cn

Ruby: arr.max;  arr.min
来源：http://rb.hahajie.cn

C#:   list.Max();  list.Min()
来源：http://ms.lnxyls.cn

[D18] 扁平化嵌套数组
来源：http://pa.szsharing.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://rs.jianghongdianzi.cn

PHP:  array_merge(...$nested);
来源：http://pk.huixinmuqiang.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://tt.shxzukj.cn

TS:   nested.flat();
来源：http://eq.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wa.nszjky.cn

Go:   // 手写双层循环
来源：http://sd.lnxyls.cn

Ruby: nested.flatten
来源：http://xs.haigaiapp.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://xy.lnxyls.cn

[D19] 按字段分组
来源：http://cr.jianghongdianzi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://pq.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cj.nszjky.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://vw.huixiangedu.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vv.huixiangedu.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://fd.shtwfgs.cn

Go:   // 手写 map[string][]T
来源：http://wr.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://bp.gzmigu.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://gm.521024.cn

[D20] 统计每个元素出现次数
来源：http://yi.shxzukj.cn

Py:   Counter(arr)
来源：http://xi.huanxung.cn

PHP:  array_count_values($arr);
来源：http://bc.9csxet.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://vr.colortex.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://yw.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://so.panjiajie.cn

Go:   // 手写 map[T]int
来源：http://nz.asd995.cn

Ruby: arr.tally
来源：http://fz.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://eh.gzmigu.cn

[D21] 判断是否包含某元素
来源：http://dx.yuntaijiaju.cn

Py:   x in arr
来源：http://je.hnjuh.cn

PHP:  in_array($x, $arr, true);
来源：http://zi.wgjwhj.cn

JS:   arr.includes(x)
来源：http://gy.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://et.hahajie.cn

Java: list.contains(x)
来源：http://gw.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://ht.huixiangedu.cn

Ruby: arr.include?(x)
来源：http://nz.colortex.cn

C#:   list.Contains(x)
来源：http://xj.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://uk.panjiajie.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://lb.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://vr.huanxung.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hy.wgjwhj.cn

TS:   [...arr];
来源：http://ee.lnxyls.cn

Java: new ArrayList<>(list);
来源：http://dw.shxzskj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://dy.chemitech.net.cn

Ruby: arr.dup;  arr.clone
来源：http://ay.nszjky.cn

C#:   new List<int>(list);
来源：http://zx.muxihuayi.cn

[D23] reduce 累积计算
来源：http://ff.huixiangedu.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://ab.muxihuayi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://gj.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://aa.asd995.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://on.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://vd.lnxyls.cn

Go:   // 手写循环
来源：http://ah.panjiajie.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://lh.hahajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://nv.jctech888.com.cn

[D24] 字典 / Map 基本操作
来源：http://od.shtwfgs.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://gq.yuntaijiaju.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ro.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hn.colortex.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://da.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://qk.gzmigu.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://gt.asd995.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://kn.chemitech.net.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://oe.nszjky.cn

[D25] Set 集合去重与交并差
来源：http://ok.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://xu.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://py.huixiangedu.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://os.huixiangedu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://fc.shxzukj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://lr.jianghongdianzi.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ol.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://oc.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://gz.huanxung.cn

[D26] 数组转字符串
来源：http://iw.shxzskj.cn

Py:   ", ".join(map(str, arr))
来源：http://fw.nicolike.cn

PHP:  implode(", ", $arr);
来源：http://eh.panjiajie.cn

JS:   arr.join(", ")
来源：http://yv.hnjuh.cn

TS:   arr.join(", ")
来源：http://wu.yuntaijiaju.cn

Java: String.join(", ", list)
来源：http://ts.yuntaijiaju.cn

Go:   strings.Join(strs, ", ")
来源：http://xj.szsharing.cn

Ruby: arr.join(", ")
来源：http://dp.wgjwhj.cn

C#:   string.Join(", ", list)
来源：http://az.colortex.cn

================================================================================
来源：http://rs.bookmarksfly.cn

E. 字符串处理
来源：http://qh.muxihuayi.cn

================================================================================
来源：http://aj.newstarts.cn

[E01] 拼接字符串
来源：http://mh.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ze.bookmarksfly.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pa.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://vq.jctech888.com.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ra.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cw.bjjhwx.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ag.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://je.lnxyls.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rd.nszjky.cn

[E02] 重复字符串
来源：http://xf.lnxyls.cn

Py:   "ab" * 3
来源：http://mk.asd995.cn

PHP:  str_repeat("ab", 3);
来源：http://uf.yuntaijiaju.cn

JS:   "ab".repeat(3)
来源：http://pt.jianghongdianzi.cn

TS:   "ab".repeat(3)
来源：http://cx.panjiajie.cn

Java: "ab".repeat(3)
来源：http://il.jianghongdianzi.cn

Go:   strings.Repeat("ab", 3)
来源：http://cp.chemitech.net.cn

Ruby: "ab" * 3
来源：http://xb.bookmarksfly.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ig.huixinmuqiang.cn

[E03] 截取子串
来源：http://gb.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vg.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hd.huixinmuqiang.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ab.asd995.cn

TS:   s.slice(1, 4)
来源：http://gz.szsharing.cn

Java: s.substring(1, 4)
来源：http://ss.bjjhwx.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://qe.wgjwhj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://cr.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://bm.haigaiapp.cn

[E04] 查找子串位置
来源：http://zn.newstarts.cn

Py:   s.find("x");  s.index("x")
来源：http://fr.9csxet.cn

PHP:  strpos($s, "x");
来源：http://yd.shtwfgs.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xh.bookmarksfly.cn

TS:   s.indexOf("x")
来源：http://ts.huixiangedu.cn

Java: s.indexOf("x")
来源：http://pe.huixiangedu.cn

Go:   strings.Index(s, "x")
来源：http://ki.hnjuh.cn

Ruby: s.index("x")
来源：http://nm.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://ms.colortex.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://zx.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://jb.shxzukj.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zu.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zt.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ag.gzmigu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eq.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gv.nszjky.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://qv.muxihuayi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ba.521024.cn

[E06] 替换子串
来源：http://xt.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ci.asd995.cn

PHP:  str_replace("a", "b", $s);
来源：http://sl.shxzskj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wu.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://fs.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tz.shxzukj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tc.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://lf.jianghongdianzi.cn

C#:   s.Replace("a", "b")
来源：http://aw.newstarts.cn

[E07] 按分隔符拆分
来源：http://xr.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://zt.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://is.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://jo.nicolike.cn

TS:   s.split(",")
来源：http://mn.jianghongdianzi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://av.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://uz.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://zs.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://op.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://mh.9csxet.cn

Py:   ",".join(items)
来源：http://wb.wgjwhj.cn

PHP:  implode(",", $items);
来源：http://dh.shxzskj.cn

JS:   items.join(",")
来源：http://gp.jianghongdianzi.cn

TS:   items.join(",")
来源：http://br.hnjuh.cn

Java: String.join(",", items)
来源：http://gd.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://af.szxytkj.cn

Ruby: items.join(",")
来源：http://cw.asd995.cn

C#:   string.Join(",", items)
来源：http://qk.jianghongdianzi.cn

[E09] 去除所有空白字符
来源：http://pd.szxytkj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yj.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kp.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://xq.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://ih.bjjhwx.cn

Java: s.replaceAll("\\s+", "")
来源：http://wh.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ef.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uw.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ts.hnjuh.cn

[E10] 左侧补零 / 定长填充
来源：http://oa.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fy.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://zp.colortex.cn

JS:   "7".padStart(3, "0")
来源：http://jn.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://tc.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://jo.nszjky.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://lt.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pj.shxzskj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vh.jctech888.com.cn

[E11] 反转字符串
来源：http://dx.muxihuayi.cn

Py:   s[::-1]
来源：http://ls.huixinmuqiang.cn

PHP:  strrev($s);
来源：http://tt.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://nu.nicolike.cn

TS:   [...s].reverse().join("")
来源：http://ir.hnjuh.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qb.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gp.9csxet.cn

Ruby: s.reverse
来源：http://gi.gzmigu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://nj.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://qp.colortex.cn

Py:   s.count("a")
来源：http://rb.hnjuh.cn

PHP:  substr_count($s, "a");
来源：http://dw.asd995.cn

JS:   s.split("a").length - 1
来源：http://rs.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://ew.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://yj.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://uc.bjjhwx.cn

Ruby: s.count("a")
来源：http://vf.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://fn.szsharing.cn

[E13] 逐字符遍历
来源：http://cx.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://rz.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wf.yuntaijiaju.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ui.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ps.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fo.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ow.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bc.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://yp.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://zk.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qo.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ty.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://pn.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xn.hnjuh.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://av.hahajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qp.chemitech.net.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jh.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://gt.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://el.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mx.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nl.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lh.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ig.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hv.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pi.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://eb.bookmarksfly.cn

[E16] 数字千分位
来源：http://ou.yuexingan06.cn

Py:   f"{1234567:,}"
来源：http://zc.gzmigu.cn

PHP:  number_format(1234567);
来源：http://hs.huixinmuqiang.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://br.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bs.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://sz.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lm.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hl.huanxung.cn

C#:   1234567.ToString("N0")
来源：http://au.yuexingan06.cn

[E17] 首字母大写
来源：http://re.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dj.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ue.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ig.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dn.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jf.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qn.hnjuh.cn

Ruby: s.capitalize
来源：http://ip.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fx.shtwfgs.cn


<!-- 参考信息 -->