代发 wailian999

[D11] 反转数组
来源：http://gh.huixiangedu.cn

Py:   arr[::-1];  arr.reverse()
来源：http://qm.newstarts.cn

PHP:  array_reverse($arr);
来源：http://zt.bjjhwx.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://af.panjiajie.cn

TS:   [...arr].reverse();
来源：http://pl.bjjhwx.cn

Java: Collections.reverse(list);
来源：http://ym.shxzskj.cn

Go:   slices.Reverse(arr)
来源：http://vu.szxytkj.cn

Ruby: arr.reverse
来源：http://kc.lnxyls.cn

C#:   list.Reverse();
来源：http://mv.shxzukj.cn

[D12] 查找元素下标
来源：http://uo.asd995.cn

Py:   arr.index(x);  x in arr
来源：http://oi.lnxyls.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://xs.9csxet.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://zx.yuntaijiaju.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://ne.521024.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hv.jctech888.com.cn

Go:   slices.Index(arr, x)
来源：http://kn.colortex.cn

Ruby: arr.index(x)
来源：http://zl.szxytkj.cn

C#:   list.IndexOf(x);
来源：http://gy.shxzskj.cn

[D13] 过滤（保留满足条件的）
来源：http://yx.521024.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://av.huixinmuqiang.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mn.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://vh.chemitech.net.cn

TS:   arr.filter(x => x > 3)
来源：http://wj.hnjuh.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wj.szxytkj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://qs.muxihuayi.cn

Ruby: arr.select { |x| x > 3 }
来源：http://fw.bjjhwx.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://oq.haigaiapp.cn

[D14] 映射转换（每个元素变形）
来源：http://uj.huixiangedu.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://zg.newstarts.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://uf.panjiajie.cn

JS:   arr.map(x => x * 2)
来源：http://ec.bookmarksfly.cn

TS:   arr.map(x => x * 2)
来源：http://nn.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://xz.newstarts.cn

Go:   // 手写循环
来源：http://qe.chemitech.net.cn

Ruby: arr.map { |x| x * 2 }
来源：http://yn.szxytkj.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://qz.huixinmuqiang.cn

[D15] 去重
来源：http://bv.shtwfgs.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://vf.jctech888.com.cn

PHP:  array_unique($arr);
来源：http://jo.521024.cn

JS:   [...new Set(arr)]
来源：http://fx.colortex.cn

TS:   [...new Set(arr)]
来源：http://qt.shxzukj.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hr.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://nx.huixiangedu.cn

Ruby: arr.uniq
来源：http://cs.huixiangedu.cn

C#:   list.Distinct().ToList()
来源：http://jq.yuexingan06.cn

[D16] 求和与平均值
来源：http://cz.huixinmuqiang.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jc.521024.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://df.jctech888.com.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://pc.chemitech.net.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://co.muxihuayi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ot.muxihuayi.cn

Go:   // 手写循环累加
来源：http://mq.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://km.9csxet.cn

C#:   list.Sum();  list.Average()
来源：http://ow.jctech888.com.cn

[D17] 最大值与最小值
来源：http://ra.newstarts.cn

Py:   max(arr);  min(arr)
来源：http://ln.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://ru.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://gr.yuntaijiaju.cn

TS:   Math.max(...arr);
来源：http://vk.huanxung.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://nz.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ms.asd995.cn

Ruby: arr.max;  arr.min
来源：http://gw.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://gs.hnjuh.cn

[D18] 扁平化嵌套数组
来源：http://ub.jianghongdianzi.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://uu.panjiajie.cn

PHP:  array_merge(...$nested);
来源：http://br.chemitech.net.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://uz.lnxyls.cn

TS:   nested.flat();
来源：http://kj.chemitech.net.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://gt.muxihuayi.cn

Go:   // 手写双层循环
来源：http://fv.9csxet.cn

Ruby: nested.flatten
来源：http://ac.shxzukj.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://lr.muxihuayi.cn

[D19] 按字段分组
来源：http://fi.huixinmuqiang.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://qm.nicolike.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://nc.jianghongdianzi.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hw.nszjky.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://vq.nicolike.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ir.huanxung.cn

Go:   // 手写 map[string][]T
来源：http://hq.muxihuayi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://md.haigaiapp.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qs.panjiajie.cn

[D20] 统计每个元素出现次数
来源：http://nv.chemitech.net.cn

Py:   Counter(arr)
来源：http://bi.shxzukj.cn

PHP:  array_count_values($arr);
来源：http://ao.bjjhwx.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://xg.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sd.nszjky.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://uw.newstarts.cn

Go:   // 手写 map[T]int
来源：http://ny.szsharing.cn

Ruby: arr.tally
来源：http://ld.nszjky.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://nz.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://vc.hnjuh.cn

Py:   x in arr
来源：http://ct.jianghongdianzi.cn

PHP:  in_array($x, $arr, true);
来源：http://qj.szxytkj.cn

JS:   arr.includes(x)
来源：http://bz.muxihuayi.cn

TS:   arr.includes(x)
来源：http://hx.9csxet.cn

Java: list.contains(x)
来源：http://qv.wgjwhj.cn

Go:   slices.Contains(arr, x)
来源：http://zg.gzmigu.cn

Ruby: arr.include?(x)
来源：http://sp.bjjhwx.cn

C#:   list.Contains(x)
来源：http://kb.hahajie.cn

[D22] 复制数组（避免共享引用）
来源：http://ya.9csxet.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://de.shtwfgs.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hm.521024.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://pt.yuntaijiaju.cn

TS:   [...arr];
来源：http://yo.shtwfgs.cn

Java: new ArrayList<>(list);
来源：http://bt.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://jx.szxytkj.cn

Ruby: arr.dup;  arr.clone
来源：http://tv.szsharing.cn

C#:   new List<int>(list);
来源：http://wq.nszjky.cn

[D23] reduce 累积计算
来源：http://vd.yuexingan06.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://tb.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wt.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cf.bookmarksfly.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://cj.yuexingan06.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://al.nicolike.cn

Go:   // 手写循环
来源：http://ad.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://uh.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://vn.nicolike.cn

[D24] 字典 / Map 基本操作
来源：http://gl.panjiajie.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wz.newstarts.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://db.wgjwhj.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xc.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://yi.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://xh.jctech888.com.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hy.muxihuayi.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qi.huixiangedu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mc.szxytkj.cn

[D25] Set 集合去重与交并差
来源：http://op.huixinmuqiang.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://jk.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ms.wgjwhj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://eq.shxzukj.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ea.9csxet.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://xb.bookmarksfly.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://dq.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ah.muxihuayi.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.bjjhwx.cn

[D26] 数组转字符串
来源：http://yu.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://hs.9csxet.cn

PHP:  implode(", ", $arr);
来源：http://ac.bjjhwx.cn

JS:   arr.join(", ")
来源：http://vp.szsharing.cn

TS:   arr.join(", ")
来源：http://jr.newstarts.cn

Java: String.join(", ", list)
来源：http://nh.521024.cn

Go:   strings.Join(strs, ", ")
来源：http://qr.shtwfgs.cn

Ruby: arr.join(", ")
来源：http://mb.colortex.cn

C#:   string.Join(", ", list)
来源：http://lr.chemitech.net.cn

================================================================================
来源：http://yc.hahajie.cn

E. 字符串处理
来源：http://ju.newstarts.cn

================================================================================
来源：http://uz.szxytkj.cn

[E01] 拼接字符串
来源：http://rx.yuexingan06.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mh.shxzukj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://up.huixiangedu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wv.shtwfgs.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://no.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://qd.colortex.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nv.yuexingan06.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://za.shxzskj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://em.jianghongdianzi.cn

[E02] 重复字符串
来源：http://ws.panjiajie.cn

Py:   "ab" * 3
来源：http://lw.bjjhwx.cn

PHP:  str_repeat("ab", 3);
来源：http://qn.hahajie.cn

JS:   "ab".repeat(3)
来源：http://sa.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://ue.521024.cn

Java: "ab".repeat(3)
来源：http://nu.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://ha.yuexingan06.cn

Ruby: "ab" * 3
来源：http://pi.gzmigu.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://sg.yuntaijiaju.cn

[E03] 截取子串
来源：http://sw.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ut.lnxyls.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vs.nszjky.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ur.nicolike.cn

TS:   s.slice(1, 4)
来源：http://xf.jctech888.com.cn

Java: s.substring(1, 4)
来源：http://xt.wgjwhj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hd.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://du.shxzukj.cn

C#:   s.Substring(1, 3)
来源：http://ne.chemitech.net.cn

[E04] 查找子串位置
来源：http://nw.chemitech.net.cn

Py:   s.find("x");  s.index("x")
来源：http://nh.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://nu.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://bc.colortex.cn

TS:   s.indexOf("x")
来源：http://kc.nszjky.cn

Java: s.indexOf("x")
来源：http://vg.newstarts.cn

Go:   strings.Index(s, "x")
来源：http://pl.gzmigu.cn

Ruby: s.index("x")
来源：http://jn.yuntaijiaju.cn

C#:   s.IndexOf("x")
来源：http://xq.haigaiapp.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ee.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tv.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://bw.panjiajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yg.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://mn.hnjuh.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://jk.shtwfgs.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://tj.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ky.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://yb.bookmarksfly.cn

[E06] 替换子串
来源：http://ta.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cl.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://ip.9csxet.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://jt.gzmigu.cn

TS:   s.replaceAll("a", "b")
来源：http://cm.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fd.bjjhwx.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://cp.shxzskj.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://up.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://ev.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://eu.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hx.colortex.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://xw.newstarts.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ie.hnjuh.cn

TS:   s.split(",")
来源：http://hj.shxzskj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://qc.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mh.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://si.bjjhwx.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pn.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://dh.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://it.huanxung.cn

PHP:  implode(",", $items);
来源：http://pu.lnxyls.cn

JS:   items.join(",")
来源：http://he.shtwfgs.cn

TS:   items.join(",")
来源：http://rt.muxihuayi.cn

Java: String.join(",", items)
来源：http://gg.wgjwhj.cn

Go:   strings.Join(items, ",")
来源：http://tj.bookmarksfly.cn

Ruby: items.join(",")
来源：http://fw.szsharing.cn

C#:   string.Join(",", items)
来源：http://dh.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://ei.shxzukj.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ql.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://gr.asd995.cn

JS:   s.replace(/\s+/g, "")
来源：http://on.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://pz.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://nx.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://wa.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vs.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://un.huixiangedu.cn

[E10] 左侧补零 / 定长填充
来源：http://oc.lnxyls.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://je.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://gc.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://tp.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://xs.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://kr.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://nj.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gq.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sv.lnxyls.cn

[E11] 反转字符串
来源：http://rp.yuexingan06.cn

Py:   s[::-1]
来源：http://es.nszjky.cn

PHP:  strrev($s);
来源：http://bw.bjjhwx.cn

JS:   [...s].reverse().join("")
来源：http://kt.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://sn.nicolike.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rg.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ip.haigaiapp.cn

Ruby: s.reverse
来源：http://xv.haigaiapp.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yx.szxytkj.cn

[E12] 统计某字符出现次数
来源：http://ia.hahajie.cn

Py:   s.count("a")
来源：http://vb.huixinmuqiang.cn

PHP:  substr_count($s, "a");
来源：http://du.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://io.huanxung.cn

TS:   s.split("a").length - 1
来源：http://wr.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://zr.hahajie.cn

Go:   strings.Count(s, "a")
来源：http://ox.hnjuh.cn

Ruby: s.count("a")
来源：http://wp.asd995.cn

C#:   s.Count(c => c == 'a')
来源：http://ii.shxzskj.cn

[E13] 逐字符遍历
来源：http://yp.asd995.cn

Py:   for ch in s: print(ch)
来源：http://ld.asd995.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ie.9csxet.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://tr.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ik.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://un.huanxung.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ku.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ne.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sp.gzmigu.cn

[E14] URL 编码与 Base64
来源：http://ot.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bu.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://es.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ko.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xz.yuntaijiaju.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kt.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zm.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://iq.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nh.muxihuayi.cn

[E15] HTML 转义 / 反转义
来源：http://vd.shxzskj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ep.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ow.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://rp.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mx.yuntaijiaju.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://nn.huixinmuqiang.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vh.yuexingan06.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ms.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://rd.huixinmuqiang.cn

[E16] 数字千分位
来源：http://ci.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://od.wgjwhj.cn

PHP:  number_format(1234567);
来源：http://ls.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gi.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dq.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ak.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ud.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zo.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://qn.gzmigu.cn

[E17] 首字母大写
来源：http://wu.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cc.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://hi.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wv.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://al.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ic.jctech888.com.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wq.szxytkj.cn

Ruby: s.capitalize
来源：http://eh.nszjky.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hf.chemitech.net.cn


<!-- 参考信息 -->