代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://ky.nszjky.cn

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://rp.9csxet.cn

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://yv.hahajie.cn

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://iu.lnxyls.cn

Java: list.sort(Comparator.comparing(Person::age));
来源：http://pk.9csxet.cn

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://qs.lnxyls.cn

Ruby: arr.sort_by { |x| x[:age] }
来源：http://zd.nszjky.cn

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://dp.szsharing.cn

[D11] 反转数组
来源：http://xv.szsharing.cn

Py:   arr[::-1];  arr.reverse()
来源：http://ag.shxzukj.cn

PHP:  array_reverse($arr);
来源：http://eq.wgjwhj.cn

JS:   [...arr].reverse();  arr.toReversed()
来源：http://kb.yuntaijiaju.cn

TS:   [...arr].reverse();
来源：http://ol.yuexingan06.cn

Java: Collections.reverse(list);
来源：http://fz.asd995.cn

Go:   slices.Reverse(arr)
来源：http://qn.muxihuayi.cn

Ruby: arr.reverse
来源：http://xj.hahajie.cn

C#:   list.Reverse();
来源：http://kw.shxzskj.cn

[D12] 查找元素下标
来源：http://he.muxihuayi.cn

Py:   arr.index(x);  x in arr
来源：http://zf.szsharing.cn

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://mi.gzmigu.cn

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://rj.muxihuayi.cn

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://bn.gzmigu.cn

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://kb.huixinmuqiang.cn

Go:   slices.Index(arr, x)
来源：http://sv.asd995.cn

Ruby: arr.index(x)
来源：http://cw.chemitech.net.cn

C#:   list.IndexOf(x);
来源：http://np.lnxyls.cn

[D13] 过滤（保留满足条件的）
来源：http://fm.9csxet.cn

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://ak.521024.cn

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://le.gzmigu.cn

JS:   arr.filter(x => x > 3)
来源：http://hw.nicolike.cn

TS:   arr.filter(x => x > 3)
来源：http://iq.shtwfgs.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hw.shxzskj.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://go.hahajie.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nv.bookmarksfly.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://ft.hnjuh.cn

[D14] 映射转换（每个元素变形）
来源：http://or.hahajie.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://fr.panjiajie.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://ew.gzmigu.cn

JS:   arr.map(x => x * 2)
来源：http://lg.huanxung.cn

TS:   arr.map(x => x * 2)
来源：http://fz.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://za.nicolike.cn

Go:   // 手写循环
来源：http://pv.jctech888.com.cn

Ruby: arr.map { |x| x * 2 }
来源：http://bn.szsharing.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dl.lnxyls.cn

[D15] 去重
来源：http://ak.nicolike.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://oh.hnjuh.cn

PHP:  array_unique($arr);
来源：http://kn.9csxet.cn

JS:   [...new Set(arr)]
来源：http://zf.jianghongdianzi.cn

TS:   [...new Set(arr)]
来源：http://zi.jianghongdianzi.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://qy.newstarts.cn

Go:   // 用 map[T]struct{} 手写
来源：http://oi.huixinmuqiang.cn

Ruby: arr.uniq
来源：http://dq.521024.cn

C#:   list.Distinct().ToList()
来源：http://ip.szsharing.cn

[D16] 求和与平均值
来源：http://qi.lnxyls.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://ek.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://oa.gzmigu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://dv.shxzskj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wp.nicolike.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ak.shxzukj.cn

Go:   // 手写循环累加
来源：http://vy.panjiajie.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://nt.shtwfgs.cn

C#:   list.Sum();  list.Average()
来源：http://xa.huixiangedu.cn

[D17] 最大值与最小值
来源：http://hz.wgjwhj.cn

Py:   max(arr);  min(arr)
来源：http://xo.huixiangedu.cn

PHP:  max($arr);  min($arr);
来源：http://hn.521024.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ha.lnxyls.cn

TS:   Math.max(...arr);
来源：http://wi.521024.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://ug.haigaiapp.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://oh.asd995.cn

Ruby: arr.max;  arr.min
来源：http://kw.huixiangedu.cn

C#:   list.Max();  list.Min()
来源：http://on.szsharing.cn

[D18] 扁平化嵌套数组
来源：http://bh.huanxung.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ia.newstarts.cn

PHP:  array_merge(...$nested);
来源：http://ym.521024.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ty.huixinmuqiang.cn

TS:   nested.flat();
来源：http://ti.panjiajie.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yq.haigaiapp.cn

Go:   // 手写双层循环
来源：http://cr.lnxyls.cn

Ruby: nested.flatten
来源：http://uk.jianghongdianzi.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://yo.wgjwhj.cn

[D19] 按字段分组
来源：http://lv.lnxyls.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mw.panjiajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://pm.chemitech.net.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://rn.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ms.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://pg.chemitech.net.cn

Go:   // 手写 map[string][]T
来源：http://rd.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://ul.nicolike.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://xp.szsharing.cn

[D20] 统计每个元素出现次数
来源：http://ct.yuexingan06.cn

Py:   Counter(arr)
来源：http://qp.nicolike.cn

PHP:  array_count_values($arr);
来源：http://bx.huanxung.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wz.huixiangedu.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://tr.chemitech.net.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://vo.haigaiapp.cn

Go:   // 手写 map[T]int
来源：http://iy.haigaiapp.cn

Ruby: arr.tally
来源：http://qc.wgjwhj.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ua.huixinmuqiang.cn

[D21] 判断是否包含某元素
来源：http://qh.panjiajie.cn

Py:   x in arr
来源：http://qb.wgjwhj.cn

PHP:  in_array($x, $arr, true);
来源：http://df.gzmigu.cn

JS:   arr.includes(x)
来源：http://mp.hnjuh.cn

TS:   arr.includes(x)
来源：http://eq.newstarts.cn

Java: list.contains(x)
来源：http://xf.chemitech.net.cn

Go:   slices.Contains(arr, x)
来源：http://sj.wgjwhj.cn

Ruby: arr.include?(x)
来源：http://tm.panjiajie.cn

C#:   list.Contains(x)
来源：http://tt.szsharing.cn

[D22] 复制数组（避免共享引用）
来源：http://fp.huixiangedu.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://th.jianghongdianzi.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ns.nicolike.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://zb.asd995.cn

TS:   [...arr];
来源：http://ls.9csxet.cn

Java: new ArrayList<>(list);
来源：http://oq.newstarts.cn

Go:   copied := append([]int(nil), arr...)
来源：http://wx.hahajie.cn

Ruby: arr.dup;  arr.clone
来源：http://kl.shtwfgs.cn

C#:   new List<int>(list);
来源：http://by.gzmigu.cn

[D23] reduce 累积计算
来源：http://vr.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gn.colortex.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://cw.colortex.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ow.colortex.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://fy.szsharing.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://om.nszjky.cn

Go:   // 手写循环
来源：http://zt.newstarts.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://eu.nszjky.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://rf.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://ya.chemitech.net.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ex.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://pe.muxihuayi.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://xb.huixiangedu.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://gx.wgjwhj.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://av.haigaiapp.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://we.yuexingan06.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://nm.muxihuayi.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://vs.gzmigu.cn

[D25] Set 集合去重与交并差
来源：http://mj.muxihuayi.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://re.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://tl.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://dd.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://du.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://gb.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ql.hnjuh.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://zf.9csxet.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://ja.lnxyls.cn

[D26] 数组转字符串
来源：http://tc.panjiajie.cn

Py:   ", ".join(map(str, arr))
来源：http://iw.nszjky.cn

PHP:  implode(", ", $arr);
来源：http://oz.szxytkj.cn

JS:   arr.join(", ")
来源：http://hi.szsharing.cn

TS:   arr.join(", ")
来源：http://kd.muxihuayi.cn

Java: String.join(", ", list)
来源：http://jl.asd995.cn

Go:   strings.Join(strs, ", ")
来源：http://ud.hahajie.cn

Ruby: arr.join(", ")
来源：http://nj.muxihuayi.cn

C#:   string.Join(", ", list)
来源：http://bd.yuexingan06.cn

================================================================================
来源：http://vq.haigaiapp.cn

E. 字符串处理
来源：http://yz.huixiangedu.cn

================================================================================
来源：http://as.nicolike.cn

[E01] 拼接字符串
来源：http://nt.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://cm.shtwfgs.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://tj.jctech888.com.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://fj.yuexingan06.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://rm.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hb.huanxung.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ue.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dp.huanxung.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://rd.shxzskj.cn

[E02] 重复字符串
来源：http://uj.szxytkj.cn

Py:   "ab" * 3
来源：http://kd.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://tm.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://pn.colortex.cn

TS:   "ab".repeat(3)
来源：http://iq.lnxyls.cn

Java: "ab".repeat(3)
来源：http://ys.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://zf.chemitech.net.cn

Ruby: "ab" * 3
来源：http://fk.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://aq.lnxyls.cn

[E03] 截取子串
来源：http://la.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hd.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ld.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nv.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://wv.colortex.cn

Java: s.substring(1, 4)
来源：http://mx.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://sn.nszjky.cn

Ruby: s[1, 3];  s[1..3]
来源：http://dq.jctech888.com.cn

C#:   s.Substring(1, 3)
来源：http://yo.szxytkj.cn

[E04] 查找子串位置
来源：http://fi.nicolike.cn

Py:   s.find("x");  s.index("x")
来源：http://bp.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://as.shxzukj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://gz.lnxyls.cn

TS:   s.indexOf("x")
来源：http://gr.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ax.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://xk.9csxet.cn

Ruby: s.index("x")
来源：http://aa.nicolike.cn

C#:   s.IndexOf("x")
来源：http://dg.shxzskj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://cj.huixiangedu.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hi.jctech888.com.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://xn.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vk.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://sf.shtwfgs.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ig.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://yg.colortex.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vb.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://bk.bookmarksfly.cn

[E06] 替换子串
来源：http://yf.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://xz.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://lm.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://or.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://kr.hnjuh.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://kn.szsharing.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wb.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://pv.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://xb.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://tx.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ec.huanxung.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://qz.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://in.panjiajie.cn

TS:   s.split(",")
来源：http://ns.asd995.cn

Java: s.split(",");  s.split("\\s+")
来源：http://te.asd995.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wc.asd995.cn

Ruby: s.split(",");  s.split
来源：http://ve.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://ax.huixiangedu.cn

[E08] 数组按分隔符合并
来源：http://ee.yuexingan06.cn

Py:   ",".join(items)
来源：http://fs.chemitech.net.cn

PHP:  implode(",", $items);
来源：http://ep.huanxung.cn

JS:   items.join(",")
来源：http://hy.lnxyls.cn

TS:   items.join(",")
来源：http://yg.lnxyls.cn

Java: String.join(",", items)
来源：http://mi.panjiajie.cn

Go:   strings.Join(items, ",")
来源：http://wi.colortex.cn

Ruby: items.join(",")
来源：http://wa.szxytkj.cn

C#:   string.Join(",", items)
来源：http://dk.nicolike.cn

[E09] 去除所有空白字符
来源：http://rg.yuexingan06.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://al.shtwfgs.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ul.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://eg.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://lb.hahajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://vd.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kn.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://nm.shxzukj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://pz.asd995.cn

[E10] 左侧补零 / 定长填充
来源：http://hj.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tz.bjjhwx.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rw.panjiajie.cn

JS:   "7".padStart(3, "0")
来源：http://yi.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://ns.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://lb.521024.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://am.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://at.colortex.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://gf.panjiajie.cn

[E11] 反转字符串
来源：http://ah.nicolike.cn

Py:   s[::-1]
来源：http://ph.chemitech.net.cn

PHP:  strrev($s);
来源：http://ba.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://qd.huixiangedu.cn

TS:   [...s].reverse().join("")
来源：http://hq.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dc.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zf.nszjky.cn

Ruby: s.reverse
来源：http://ao.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://os.shtwfgs.cn

[E12] 统计某字符出现次数
来源：http://gp.szxytkj.cn

Py:   s.count("a")
来源：http://vg.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ky.nszjky.cn

JS:   s.split("a").length - 1
来源：http://eo.colortex.cn

TS:   s.split("a").length - 1
来源：http://kv.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kl.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://il.wgjwhj.cn

Ruby: s.count("a")
来源：http://qy.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ab.colortex.cn

[E13] 逐字符遍历
来源：http://ge.newstarts.cn

Py:   for ch in s: print(ch)
来源：http://se.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://on.panjiajie.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://gt.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yh.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://iz.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://yz.huixiangedu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://dz.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hj.hahajie.cn

[E14] URL 编码与 Base64
来源：http://fx.shxzukj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://oh.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jj.huixiangedu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fq.yuexingan06.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mb.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nm.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pe.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://il.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cb.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://fn.hnjuh.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pe.huixinmuqiang.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bj.jctech888.com.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ha.muxihuayi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fe.hnjuh.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://km.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qb.szxytkj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ct.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ks.chemitech.net.cn

[E16] 数字千分位
来源：http://oa.nicolike.cn

Py:   f"{1234567:,}"
来源：http://rb.szsharing.cn

PHP:  number_format(1234567);
来源：http://ku.shxzskj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ey.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://rf.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vb.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hd.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ux.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://db.bookmarksfly.cn

[E17] 首字母大写
来源：http://lt.wgjwhj.cn


<!-- 参考信息 -->