代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://ab.jianghongdianzi.cn

JS:   arr.filter(x => x > 3)
来源：http://ef.muxihuayi.cn

TS:   arr.filter(x => x > 3)
来源：http://zs.shxzukj.cn

Java: list.stream().filter(x -> x > 3).toList()
来源：http://zc.bjjhwx.cn

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wn.yuexingan06.cn

Ruby: arr.select { |x| x > 3 }
来源：http://ie.huixiangedu.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://wa.hahajie.cn

[D14] 映射转换（每个元素变形）
来源：http://gz.asd995.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://dn.lnxyls.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://bv.asd995.cn

JS:   arr.map(x => x * 2)
来源：http://yc.szsharing.cn

TS:   arr.map(x => x * 2)
来源：http://kd.lnxyls.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://ks.muxihuayi.cn

Go:   // 手写循环
来源：http://ep.huanxung.cn

Ruby: arr.map { |x| x * 2 }
来源：http://no.haigaiapp.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://dl.shxzukj.cn

[D15] 去重
来源：http://us.hahajie.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://iy.jianghongdianzi.cn

PHP:  array_unique($arr);
来源：http://ly.9csxet.cn

JS:   [...new Set(arr)]
来源：http://dq.muxihuayi.cn

TS:   [...new Set(arr)]
来源：http://ki.yuexingan06.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://sp.wgjwhj.cn

Go:   // 用 map[T]struct{} 手写
来源：http://eq.newstarts.cn

Ruby: arr.uniq
来源：http://ln.newstarts.cn

C#:   list.Distinct().ToList()
来源：http://ov.panjiajie.cn

[D16] 求和与平均值
来源：http://px.bjjhwx.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://jw.yuexingan06.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ok.szxytkj.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://ch.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://ss.huixinmuqiang.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://lf.shxzukj.cn

Go:   // 手写循环累加
来源：http://rb.asd995.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://ki.wgjwhj.cn

C#:   list.Sum();  list.Average()
来源：http://ee.lnxyls.cn

[D17] 最大值与最小值
来源：http://gt.panjiajie.cn

Py:   max(arr);  min(arr)
来源：http://zp.chemitech.net.cn

PHP:  max($arr);  min($arr);
来源：http://wn.huixinmuqiang.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://df.9csxet.cn

TS:   Math.max(...arr);
来源：http://ik.hahajie.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://gx.szsharing.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://re.lnxyls.cn

Ruby: arr.max;  arr.min
来源：http://ld.muxihuayi.cn

C#:   list.Max();  list.Min()
来源：http://cf.nszjky.cn

[D18] 扁平化嵌套数组
来源：http://ec.shxzukj.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://kj.9csxet.cn

PHP:  array_merge(...$nested);
来源：http://oz.szsharing.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ad.yuexingan06.cn

TS:   nested.flat();
来源：http://ym.9csxet.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://lm.szsharing.cn

Go:   // 手写双层循环
来源：http://gh.szxytkj.cn

Ruby: nested.flatten
来源：http://ac.gzmigu.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://du.panjiajie.cn

[D19] 按字段分组
来源：http://ne.shxzskj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hw.jianghongdianzi.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://da.shtwfgs.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wt.jianghongdianzi.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://ap.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://kz.gzmigu.cn

Go:   // 手写 map[string][]T
来源：http://am.haigaiapp.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://uq.lnxyls.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yb.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://zy.newstarts.cn

Py:   Counter(arr)
来源：http://zp.hahajie.cn

PHP:  array_count_values($arr);
来源：http://yo.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://or.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://dr.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://dw.colortex.cn

Go:   // 手写 map[T]int
来源：http://kk.jianghongdianzi.cn

Ruby: arr.tally
来源：http://mu.colortex.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mj.shxzukj.cn

[D21] 判断是否包含某元素
来源：http://jk.9csxet.cn

Py:   x in arr
来源：http://cu.szxytkj.cn

PHP:  in_array($x, $arr, true);
来源：http://ci.wgjwhj.cn

JS:   arr.includes(x)
来源：http://om.jianghongdianzi.cn

TS:   arr.includes(x)
来源：http://hn.nszjky.cn

Java: list.contains(x)
来源：http://uk.panjiajie.cn

Go:   slices.Contains(arr, x)
来源：http://rh.newstarts.cn

Ruby: arr.include?(x)
来源：http://xz.yuexingan06.cn

C#:   list.Contains(x)
来源：http://lc.huanxung.cn

[D22] 复制数组（避免共享引用）
来源：http://ac.haigaiapp.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://qz.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://cp.9csxet.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://ac.lnxyls.cn

TS:   [...arr];
来源：http://ss.shxzskj.cn

Java: new ArrayList<>(list);
来源：http://ud.jctech888.com.cn

Go:   copied := append([]int(nil), arr...)
来源：http://ot.jianghongdianzi.cn

Ruby: arr.dup;  arr.clone
来源：http://vs.shtwfgs.cn

C#:   new List<int>(list);
来源：http://vz.huixiangedu.cn

[D23] reduce 累积计算
来源：http://jl.chemitech.net.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://no.huanxung.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://pj.nszjky.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://oo.hnjuh.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wi.szxytkj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://al.bookmarksfly.cn

Go:   // 手写循环
来源：http://qa.wgjwhj.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://js.bookmarksfly.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ib.szxytkj.cn

[D24] 字典 / Map 基本操作
来源：http://sl.hnjuh.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ah.colortex.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ei.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://zc.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ka.yuexingan06.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://om.521024.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://ly.wgjwhj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://el.nicolike.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ip.hnjuh.cn

[D25] Set 集合去重与交并差
来源：http://ug.colortex.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://py.szxytkj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ma.szxytkj.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://qm.hahajie.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://dl.bookmarksfly.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ou.shtwfgs.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://bo.huanxung.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://np.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://pf.szsharing.cn

[D26] 数组转字符串
来源：http://ec.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://um.huixinmuqiang.cn

PHP:  implode(", ", $arr);
来源：http://eb.shtwfgs.cn

JS:   arr.join(", ")
来源：http://fv.nicolike.cn

TS:   arr.join(", ")
来源：http://di.shxzukj.cn

Java: String.join(", ", list)
来源：http://zk.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://mk.newstarts.cn

Ruby: arr.join(", ")
来源：http://hk.nicolike.cn

C#:   string.Join(", ", list)
来源：http://py.huanxung.cn

================================================================================
来源：http://iw.muxihuayi.cn

E. 字符串处理
来源：http://au.521024.cn

================================================================================
来源：http://uo.shtwfgs.cn

[E01] 拼接字符串
来源：http://ph.yuntaijiaju.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://kn.9csxet.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.lnxyls.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://pp.yuntaijiaju.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://ir.521024.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://pe.lnxyls.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bg.hnjuh.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://lf.wgjwhj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mf.yuexingan06.cn

[E02] 重复字符串
来源：http://rv.jctech888.com.cn

Py:   "ab" * 3
来源：http://ns.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://xl.newstarts.cn

JS:   "ab".repeat(3)
来源：http://xa.haigaiapp.cn

TS:   "ab".repeat(3)
来源：http://er.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://lc.szxytkj.cn

Go:   strings.Repeat("ab", 3)
来源：http://za.panjiajie.cn

Ruby: "ab" * 3
来源：http://mx.muxihuayi.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://xm.chemitech.net.cn

[E03] 截取子串
来源：http://ul.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nf.shxzskj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ir.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jn.huixinmuqiang.cn

TS:   s.slice(1, 4)
来源：http://ct.newstarts.cn

Java: s.substring(1, 4)
来源：http://vd.huixiangedu.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nt.jctech888.com.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ub.lnxyls.cn

C#:   s.Substring(1, 3)
来源：http://mf.huanxung.cn

[E04] 查找子串位置
来源：http://hj.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://zc.szxytkj.cn

PHP:  strpos($s, "x");
来源：http://cx.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://tn.shtwfgs.cn

TS:   s.indexOf("x")
来源：http://mr.gzmigu.cn

Java: s.indexOf("x")
来源：http://qf.chemitech.net.cn

Go:   strings.Index(s, "x")
来源：http://yi.hahajie.cn

Ruby: s.index("x")
来源：http://dr.nszjky.cn

C#:   s.IndexOf("x")
来源：http://hm.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://er.hahajie.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://no.chemitech.net.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ki.szsharing.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kf.nicolike.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pf.huixiangedu.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bj.haigaiapp.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://zg.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://lf.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fo.nicolike.cn

[E06] 替换子串
来源：http://xv.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://jx.shxzskj.cn

PHP:  str_replace("a", "b", $s);
来源：http://va.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ou.huixinmuqiang.cn

TS:   s.replaceAll("a", "b")
来源：http://qr.szsharing.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mj.yuntaijiaju.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tn.jianghongdianzi.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://te.colortex.cn

C#:   s.Replace("a", "b")
来源：http://hr.muxihuayi.cn

[E07] 按分隔符拆分
来源：http://ff.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ak.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://vy.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gt.9csxet.cn

TS:   s.split(",")
来源：http://fd.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ih.jianghongdianzi.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://cw.newstarts.cn

Ruby: s.split(",");  s.split
来源：http://nc.wgjwhj.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://bc.nszjky.cn

[E08] 数组按分隔符合并
来源：http://je.9csxet.cn

Py:   ",".join(items)
来源：http://xg.9csxet.cn

PHP:  implode(",", $items);
来源：http://bh.jctech888.com.cn

JS:   items.join(",")
来源：http://hr.gzmigu.cn

TS:   items.join(",")
来源：http://om.szsharing.cn

Java: String.join(",", items)
来源：http://af.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://rk.szxytkj.cn

Ruby: items.join(",")
来源：http://vr.colortex.cn

C#:   string.Join(",", items)
来源：http://bt.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://hm.shtwfgs.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fv.521024.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zp.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://xz.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://ga.shxzukj.cn

Java: s.replaceAll("\\s+", "")
来源：http://se.haigaiapp.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ks.shxzskj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://dp.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hj.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ty.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://st.colortex.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fz.yuexingan06.cn

JS:   "7".padStart(3, "0")
来源：http://am.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://se.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://xb.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://gk.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gm.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bw.muxihuayi.cn

[E11] 反转字符串
来源：http://dw.huixiangedu.cn

Py:   s[::-1]
来源：http://mv.521024.cn

PHP:  strrev($s);
来源：http://rj.szsharing.cn

JS:   [...s].reverse().join("")
来源：http://cr.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://cv.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yc.lnxyls.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vb.jianghongdianzi.cn

Ruby: s.reverse
来源：http://sf.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yn.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://gz.jianghongdianzi.cn

Py:   s.count("a")
来源：http://ct.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://tr.gzmigu.cn

JS:   s.split("a").length - 1
来源：http://tf.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://sb.lnxyls.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://fx.shxzukj.cn

Go:   strings.Count(s, "a")
来源：http://qm.hnjuh.cn

Ruby: s.count("a")
来源：http://kd.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://kf.huanxung.cn

[E13] 逐字符遍历
来源：http://mo.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://qf.hnjuh.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bw.gzmigu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vc.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://da.colortex.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://pu.chemitech.net.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://lt.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gk.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ep.asd995.cn

[E14] URL 编码与 Base64
来源：http://hw.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ei.chemitech.net.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bt.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bu.bookmarksfly.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://iv.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://kz.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jj.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bo.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cm.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://wy.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ws.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://cb.huixiangedu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wm.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cp.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xr.bookmarksfly.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://jn.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xm.yuexingan06.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vm.nicolike.cn

[E16] 数字千分位
来源：http://ug.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://tu.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://zh.szxytkj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rg.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zc.szsharing.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hb.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lt.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://lv.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://rd.nicolike.cn

[E17] 首字母大写
来源：http://pu.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cu.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fm.haigaiapp.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sm.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bn.nszjky.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qj.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ec.yuexingan06.cn

Ruby: s.capitalize
来源：http://pt.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rn.hnjuh.cn

[E18] 模板占位符替换
来源：http://ab.hahajie.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fo.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://js.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://oq.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mt.huixinmuqiang.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://er.jianghongdianzi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://jz.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://do.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://lx.huixiangedu.cn

[E19] 多行文本按行拆分
来源：http://aa.wgjwhj.cn

Py:   s.splitlines()
来源：http://ze.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mu.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://xe.521024.cn

TS:   s.split(/\r?\n/)
来源：http://xs.szxytkj.cn

Java: s.lines().toList()
来源：http://uf.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://wq.nszjky.cn

Ruby: s.lines
来源：http://vl.muxihuayi.cn

C#:   s.Split('\n')
来源：http://by.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://pm.colortex.cn

Py:   if not s:
来源：http://ao.asd995.cn


<!-- 参考信息 -->