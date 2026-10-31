代发 wailian999

C#:   list.Reverse();
来源：http://ws.521024.cn

[D12] 查找元素下标
来源：http://uw.9csxet.cn

Py:   arr.index(x);  x in arr
来源：http://sz.shxzukj.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://vh.shxzukj.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://xc.panjiajie.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://uw.bookmarksfly.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://vv.nicolike.cn

Go:   slices.Index(arr, x)
来源：http://lz.huixiangedu.cn

Ruby: arr.index(x)
来源：http://ir.yuexingan06.cn

C#:   list.IndexOf(x);
来源：http://zw.wgjwhj.cn

[D13] 过滤（保留满足条件的）
来源：http://si.shxzukj.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://yb.hahajie.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://dg.colortex.cn

JS:   arr.filter(x => x > 3)
来源：http://iy.hnjuh.cn

TS:   arr.filter(x => x > 3)
来源：http://hs.chemitech.net.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://ej.nszjky.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://yj.panjiajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://em.shxzskj.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://gv.yuexingan06.cn

[D14] 映射转换（每个元素变形）
来源：http://li.shxzukj.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dj.nszjky.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ze.wgjwhj.cn

JS:   arr.map(x => x * 2)
来源：http://dk.muxihuayi.cn

TS:   arr.map(x => x * 2)
来源：http://tj.521024.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://hg.asd995.cn

Go:   // 手写循环
来源：http://jm.huixinmuqiang.cn

Ruby: arr.map { |x| x * 2 }
来源：http://vq.hnjuh.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://pg.jianghongdianzi.cn

[D15] 去重
来源：http://jq.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://jo.shxzskj.cn

PHP:  array_unique($arr);
来源：http://pg.yuexingan06.cn

JS:   [...new Set(arr)]
来源：http://cu.shxzskj.cn

TS:   [...new Set(arr)]
来源：http://kp.9csxet.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sa.521024.cn

Go:   // 用 map[T]struct{} 手写
来源：http://ac.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://oy.shxzukj.cn

C#:   list.Distinct().ToList()
来源：http://js.bjjhwx.cn

[D16] 求和与平均值
来源：http://pp.yuexingan06.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bb.panjiajie.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://gv.muxihuayi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ey.hahajie.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://zm.9csxet.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lz.wgjwhj.cn

Go:   // 手写循环累加
来源：http://iq.jianghongdianzi.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://cc.chemitech.net.cn

C#:   list.Sum();  list.Average()
来源：http://vp.chemitech.net.cn

[D17] 最大值与最小值
来源：http://ie.gzmigu.cn

Py:   max(arr);  min(arr)
来源：http://vh.9csxet.cn

PHP:  max($arr);  min($arr);
来源：http://xz.muxihuayi.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://xx.panjiajie.cn

TS:   Math.max(...arr);
来源：http://mk.jianghongdianzi.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://wy.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://pt.521024.cn

Ruby: arr.max;  arr.min
来源：http://av.szsharing.cn

C#:   list.Max();  list.Min()
来源：http://xq.wgjwhj.cn

[D18] 扁平化嵌套数组
来源：http://pe.huixiangedu.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://iq.lnxyls.cn

PHP:  array_merge(...$nested);
来源：http://jk.jianghongdianzi.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://cx.colortex.cn

TS:   nested.flat();
来源：http://fs.yuexingan06.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://ju.chemitech.net.cn

Go:   // 手写双层循环
来源：http://ws.hahajie.cn

Ruby: nested.flatten
来源：http://th.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://qs.haigaiapp.cn

[D19] 按字段分组
来源：http://qk.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://ct.yuntaijiaju.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://dr.yuntaijiaju.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://yt.huanxung.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ww.yuntaijiaju.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://qp.szxytkj.cn

Go:   // 手写 map[string][]T
来源：http://ka.huanxung.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://wp.newstarts.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://ez.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://sx.muxihuayi.cn

Py:   Counter(arr)
来源：http://la.shxzskj.cn

PHP:  array_count_values($arr);
来源：http://ma.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kw.shxzskj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://bb.shtwfgs.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://bd.newstarts.cn

Go:   // 手写 map[T]int
来源：http://tf.szsharing.cn

Ruby: arr.tally
来源：http://de.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://df.9csxet.cn

[D21] 判断是否包含某元素
来源：http://qm.hahajie.cn

Py:   x in arr
来源：http://jl.521024.cn

PHP:  in_array($x, $arr, true);
来源：http://hq.shxzskj.cn

JS:   arr.includes(x)
来源：http://nr.colortex.cn

TS:   arr.includes(x)
来源：http://vc.asd995.cn

Java: list.contains(x)
来源：http://mz.jianghongdianzi.cn

Go:   slices.Contains(arr, x)
来源：http://tx.yuexingan06.cn

Ruby: arr.include?(x)
来源：http://cx.521024.cn

C#:   list.Contains(x)
来源：http://ks.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://tj.newstarts.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://jb.lnxyls.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://lv.hnjuh.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://fr.asd995.cn

TS:   [...arr];
来源：http://wk.nicolike.cn

Java: new ArrayList<>(list);
来源：http://bm.9csxet.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ew.shtwfgs.cn

Ruby: arr.dup;  arr.clone
来源：http://ot.shtwfgs.cn

C#:   new List<int>(list);
来源：http://qv.hnjuh.cn

[D23] reduce 累积计算
来源：http://lv.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://bs.lnxyls.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://jt.9csxet.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vl.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://sm.9csxet.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://jt.lnxyls.cn

Go:   // 手写循环
来源：http://zk.shxzukj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://sk.huixiangedu.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vg.muxihuayi.cn

[D24] 字典 / Map 基本操作
来源：http://az.bookmarksfly.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://cz.shtwfgs.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://jc.lnxyls.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://ta.jianghongdianzi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://dj.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://jd.lnxyls.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://lb.huanxung.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://pq.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://kk.bjjhwx.cn

[D25] Set 集合去重与交并差
来源：http://cx.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://id.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://un.shtwfgs.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://ly.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mq.muxihuayi.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://dr.huixinmuqiang.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fu.nszjky.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ab.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://en.yuntaijiaju.cn

[D26] 数组转字符串
来源：http://bq.szxytkj.cn

Py:   ", ".join(map(str, arr))
来源：http://fg.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://re.jctech888.com.cn

JS:   arr.join(", ")
来源：http://rv.lnxyls.cn

TS:   arr.join(", ")
来源：http://ph.shxzukj.cn

Java: String.join(", ", list)
来源：http://ca.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://tw.bookmarksfly.cn

Ruby: arr.join(", ")
来源：http://gm.nicolike.cn

C#:   string.Join(", ", list)
来源：http://pq.szsharing.cn

================================================================================
来源：http://vd.521024.cn

E. 字符串处理
来源：http://ac.colortex.cn

================================================================================
来源：http://kk.panjiajie.cn

[E01] 拼接字符串
来源：http://th.haigaiapp.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://om.szsharing.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wx.9csxet.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ts.hahajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://zf.hahajie.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ay.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sr.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ed.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ya.yuntaijiaju.cn

[E02] 重复字符串
来源：http://ku.bookmarksfly.cn

Py:   "ab" * 3
来源：http://tk.huanxung.cn

PHP:  str_repeat("ab", 3);
来源：http://vq.hahajie.cn

JS:   "ab".repeat(3)
来源：http://hc.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://kc.jianghongdianzi.cn

Java: "ab".repeat(3)
来源：http://sg.colortex.cn

Go:   strings.Repeat("ab", 3)
来源：http://tw.haigaiapp.cn

Ruby: "ab" * 3
来源：http://wb.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sj.huanxung.cn

[E03] 截取子串
来源：http://gm.bjjhwx.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ic.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ti.hnjuh.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://gw.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://fk.colortex.cn

Java: s.substring(1, 4)
来源：http://ca.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://gw.huixiangedu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://mm.hahajie.cn

C#:   s.Substring(1, 3)
来源：http://pk.muxihuayi.cn

[E04] 查找子串位置
来源：http://ev.huanxung.cn

Py:   s.find("x");  s.index("x")
来源：http://bz.huixinmuqiang.cn

PHP:  strpos($s, "x");
来源：http://mr.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ao.asd995.cn

TS:   s.indexOf("x")
来源：http://ka.bookmarksfly.cn

Java: s.indexOf("x")
来源：http://gx.hnjuh.cn

Go:   strings.Index(s, "x")
来源：http://hj.hnjuh.cn

Ruby: s.index("x")
来源：http://rw.nszjky.cn

C#:   s.IndexOf("x")
来源：http://la.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://hn.szxytkj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hx.asd995.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://nn.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://iw.yuntaijiaju.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pd.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kf.bookmarksfly.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://jj.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://co.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://qb.lnxyls.cn

[E06] 替换子串
来源：http://qo.shxzskj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pn.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://hp.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gk.chemitech.net.cn

TS:   s.replaceAll("a", "b")
来源：http://bg.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://gb.asd995.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://qh.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hi.lnxyls.cn

C#:   s.Replace("a", "b")
来源：http://bq.shxzukj.cn

[E07] 按分隔符拆分
来源：http://jb.huixinmuqiang.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://se.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wx.yuntaijiaju.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://wx.haigaiapp.cn

TS:   s.split(",")
来源：http://na.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qy.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bj.shtwfgs.cn

Ruby: s.split(",");  s.split
来源：http://nw.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pp.yuntaijiaju.cn

[E08] 数组按分隔符合并
来源：http://rl.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://ny.colortex.cn

PHP:  implode(",", $items);
来源：http://cm.jianghongdianzi.cn

JS:   items.join(",")
来源：http://js.nszjky.cn

TS:   items.join(",")
来源：http://tt.panjiajie.cn

Java: String.join(",", items)
来源：http://ax.gzmigu.cn

Go:   strings.Join(items, ",")
来源：http://xi.huanxung.cn

Ruby: items.join(",")
来源：http://vu.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://ju.lnxyls.cn

[E09] 去除所有空白字符
来源：http://ky.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fa.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://nf.bjjhwx.cn

JS:   s.replace(/\s+/g, "")
来源：http://od.muxihuayi.cn

TS:   s.replace(/\s+/g, "")
来源：http://xr.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://va.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sl.hahajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mn.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fo.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://vb.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://nt.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://th.szsharing.cn

JS:   "7".padStart(3, "0")
来源：http://nx.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://et.nicolike.cn

Java: String.format("%03d", 7)
来源：http://qx.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rp.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ea.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ut.panjiajie.cn

[E11] 反转字符串
来源：http://bl.newstarts.cn

Py:   s[::-1]
来源：http://vr.nszjky.cn

PHP:  strrev($s);
来源：http://tu.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://so.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://kb.jianghongdianzi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dk.jctech888.com.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://cj.hnjuh.cn

Ruby: s.reverse
来源：http://go.521024.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gi.9csxet.cn

[E12] 统计某字符出现次数
来源：http://vh.colortex.cn

Py:   s.count("a")
来源：http://dv.chemitech.net.cn

PHP:  substr_count($s, "a");
来源：http://ex.newstarts.cn

JS:   s.split("a").length - 1
来源：http://df.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://jl.gzmigu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ik.asd995.cn

Go:   strings.Count(s, "a")
来源：http://qf.lnxyls.cn

Ruby: s.count("a")
来源：http://ko.huanxung.cn

C#:   s.Count(c => c == 'a')
来源：http://bu.hahajie.cn

[E13] 逐字符遍历
来源：http://lp.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://qh.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rl.hahajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hm.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://pk.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rj.lnxyls.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://he.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pe.jctech888.com.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://pb.newstarts.cn

[E14] URL 编码与 Base64
来源：http://er.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://dr.colortex.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qi.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://sd.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://dm.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hh.newstarts.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://sn.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ya.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wi.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://vp.shtwfgs.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qw.shtwfgs.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ss.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qr.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sp.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ex.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yu.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://vd.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://lj.lnxyls.cn

[E16] 数字千分位
来源：http://wx.szsharing.cn

Py:   f"{1234567:,}"
来源：http://qp.szsharing.cn

PHP:  number_format(1234567);
来源：http://my.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://py.huixinmuqiang.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rv.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://of.muxihuayi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xh.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ln.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://ks.asd995.cn

[E17] 首字母大写
来源：http://gg.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vy.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://wj.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sa.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zt.521024.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wy.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oo.asd995.cn

Ruby: s.capitalize
来源：http://xz.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wr.9csxet.cn

[E18] 模板占位符替换
来源：http://sz.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yk.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kn.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ok.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://di.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rm.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ds.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://au.9csxet.cn


<!-- 参考信息 -->