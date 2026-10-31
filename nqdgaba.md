代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://xb.lnxyls.cn

Ruby: arr.select { |x| x > 3 }
来源：http://nz.chemitech.net.cn

C#:   list.Where(x => x > 3).ToList()
来源：http://xi.szxytkj.cn

[D14] 映射转换（每个元素变形）
来源：http://yl.bookmarksfly.cn

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://na.9csxet.cn

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://dm.newstarts.cn

JS:   arr.map(x => x * 2)
来源：http://ed.newstarts.cn

TS:   arr.map(x => x * 2)
来源：http://il.huixiangedu.cn

Java: list.stream().map(x -> x * 2).toList()
来源：http://pi.bookmarksfly.cn

Go:   // 手写循环
来源：http://qc.gzmigu.cn

Ruby: arr.map { |x| x * 2 }
来源：http://tn.nicolike.cn

C#:   list.Select(x => x * 2).ToList()
来源：http://no.wgjwhj.cn

[D15] 去重
来源：http://sy.chemitech.net.cn

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://kb.newstarts.cn

PHP:  array_unique($arr);
来源：http://zv.huixinmuqiang.cn

JS:   [...new Set(arr)]
来源：http://hj.bjjhwx.cn

TS:   [...new Set(arr)]
来源：http://wf.nszjky.cn

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://in.asd995.cn

Go:   // 用 map[T]struct{} 手写
来源：http://iw.9csxet.cn

Ruby: arr.uniq
来源：http://yq.jctech888.com.cn

C#:   list.Distinct().ToList()
来源：http://uc.shxzskj.cn

[D16] 求和与平均值
来源：http://ab.huixiangedu.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://bq.chemitech.net.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://ho.jianghongdianzi.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://km.wgjwhj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://if.shxzskj.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://ke.shxzskj.cn

Go:   // 手写循环累加
来源：http://mo.shtwfgs.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://tj.shxzskj.cn

C#:   list.Sum();  list.Average()
来源：http://wq.jctech888.com.cn

[D17] 最大值与最小值
来源：http://su.nicolike.cn

Py:   max(arr);  min(arr)
来源：http://hv.hnjuh.cn

PHP:  max($arr);  min($arr);
来源：http://ig.szxytkj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mu.shxzskj.cn

TS:   Math.max(...arr);
来源：http://lf.shxzukj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://yg.shtwfgs.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://gu.jianghongdianzi.cn

Ruby: arr.max;  arr.min
来源：http://je.shxzukj.cn

C#:   list.Max();  list.Min()
来源：http://re.shtwfgs.cn

[D18] 扁平化嵌套数组
来源：http://ij.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://li.haigaiapp.cn

PHP:  array_merge(...$nested);
来源：http://un.huanxung.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://ti.521024.cn

TS:   nested.flat();
来源：http://tu.huanxung.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://oe.hnjuh.cn

Go:   // 手写双层循环
来源：http://sh.nszjky.cn

Ruby: nested.flatten
来源：http://mo.nszjky.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://mj.bjjhwx.cn

[D19] 按字段分组
来源：http://xs.muxihuayi.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://sq.hnjuh.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://cl.jctech888.com.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://xi.asd995.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://uu.huanxung.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://rr.huixiangedu.cn

Go:   // 手写 map[string][]T
来源：http://ma.nszjky.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://dg.huanxung.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://qi.szxytkj.cn

[D20] 统计每个元素出现次数
来源：http://lc.colortex.cn

Py:   Counter(arr)
来源：http://xj.shtwfgs.cn

PHP:  array_count_values($arr);
来源：http://po.chemitech.net.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://uj.hnjuh.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://rp.jctech888.com.cn

Go:   // 手写 map[T]int
来源：http://gz.bjjhwx.cn

Ruby: arr.tally
来源：http://re.szsharing.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wn.nicolike.cn

[D21] 判断是否包含某元素
来源：http://ox.panjiajie.cn

Py:   x in arr
来源：http://pz.lnxyls.cn

PHP:  in_array($x, $arr, true);
来源：http://ox.hahajie.cn

JS:   arr.includes(x)
来源：http://gf.gzmigu.cn

TS:   arr.includes(x)
来源：http://is.yuntaijiaju.cn

Java: list.contains(x)
来源：http://kc.bjjhwx.cn

Go:   slices.Contains(arr, x)
来源：http://bz.huixinmuqiang.cn

Ruby: arr.include?(x)
来源：http://zx.9csxet.cn

C#:   list.Contains(x)
来源：http://ks.jianghongdianzi.cn

[D22] 复制数组（避免共享引用）
来源：http://zf.szxytkj.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://yo.shxzukj.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://ne.huixiangedu.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://er.chemitech.net.cn

TS:   [...arr];
来源：http://th.colortex.cn

Java: new ArrayList<>(list);
来源：http://as.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://zh.huanxung.cn

Ruby: arr.dup;  arr.clone
来源：http://tt.lnxyls.cn

C#:   new List<int>(list);
来源：http://rs.szxytkj.cn

[D23] reduce 累积计算
来源：http://op.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://px.bookmarksfly.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ii.nicolike.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ly.huixinmuqiang.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gt.shxzukj.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://up.newstarts.cn

Go:   // 手写循环
来源：http://lz.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ot.jctech888.com.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ey.panjiajie.cn

[D24] 字典 / Map 基本操作
来源：http://in.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mk.bookmarksfly.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://xu.9csxet.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://qx.jctech888.com.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://fa.bjjhwx.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://ka.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mz.jctech888.com.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://tk.shtwfgs.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://se.lnxyls.cn

[D25] Set 集合去重与交并差
来源：http://xs.nicolike.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://dt.bjjhwx.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qc.521024.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hq.521024.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://sd.jctech888.com.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://ix.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ln.chemitech.net.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.szsharing.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://zk.chemitech.net.cn

[D26] 数组转字符串
来源：http://ce.nicolike.cn

Py:   ", ".join(map(str, arr))
来源：http://rw.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://bo.521024.cn

JS:   arr.join(", ")
来源：http://dp.panjiajie.cn

TS:   arr.join(", ")
来源：http://zw.panjiajie.cn

Java: String.join(", ", list)
来源：http://wf.bjjhwx.cn

Go:   strings.Join(strs, ", ")
来源：http://ar.panjiajie.cn

Ruby: arr.join(", ")
来源：http://xw.haigaiapp.cn

C#:   string.Join(", ", list)
来源：http://ff.shxzukj.cn

================================================================================
来源：http://ox.9csxet.cn

E. 字符串处理
来源：http://kw.shxzskj.cn

================================================================================
来源：http://zj.yuntaijiaju.cn

[E01] 拼接字符串
来源：http://gy.newstarts.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hv.huanxung.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ee.chemitech.net.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://tf.huanxung.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bp.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ay.szxytkj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://cd.panjiajie.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://qs.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ci.wgjwhj.cn

[E02] 重复字符串
来源：http://ml.wgjwhj.cn

Py:   "ab" * 3
来源：http://uw.shxzukj.cn

PHP:  str_repeat("ab", 3);
来源：http://zj.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://ry.yuexingan06.cn

TS:   "ab".repeat(3)
来源：http://ey.szsharing.cn

Java: "ab".repeat(3)
来源：http://is.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://fo.hahajie.cn

Ruby: "ab" * 3
来源：http://st.hahajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wh.521024.cn

[E03] 截取子串
来源：http://xb.hnjuh.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ob.yuexingan06.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://je.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fc.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://nb.wgjwhj.cn

Java: s.substring(1, 4)
来源：http://ty.lnxyls.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://vz.bjjhwx.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zl.asd995.cn

C#:   s.Substring(1, 3)
来源：http://sh.nicolike.cn

[E04] 查找子串位置
来源：http://fw.shtwfgs.cn

Py:   s.find("x");  s.index("x")
来源：http://zc.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://iy.gzmigu.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mk.huixinmuqiang.cn

TS:   s.indexOf("x")
来源：http://jq.nicolike.cn

Java: s.indexOf("x")
来源：http://gj.szxytkj.cn

Go:   strings.Index(s, "x")
来源：http://zw.colortex.cn

Ruby: s.index("x")
来源：http://ol.shxzukj.cn

C#:   s.IndexOf("x")
来源：http://sw.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://gy.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ee.huanxung.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://pn.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ls.chemitech.net.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://tv.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://eg.szxytkj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://dn.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mi.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ww.panjiajie.cn

[E06] 替换子串
来源：http://lf.gzmigu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://yx.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://zs.newstarts.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wx.yuntaijiaju.cn

TS:   s.replaceAll("a", "b")
来源：http://la.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ip.gzmigu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mg.huixinmuqiang.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://cj.asd995.cn

C#:   s.Replace("a", "b")
来源：http://wr.colortex.cn

[E07] 按分隔符拆分
来源：http://zr.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://yl.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hg.gzmigu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://sx.shxzskj.cn

TS:   s.split(",")
来源：http://pk.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://kc.newstarts.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://co.yuexingan06.cn

Ruby: s.split(",");  s.split
来源：http://gt.jctech888.com.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zv.9csxet.cn

[E08] 数组按分隔符合并
来源：http://jv.jctech888.com.cn

Py:   ",".join(items)
来源：http://oy.newstarts.cn

PHP:  implode(",", $items);
来源：http://tm.colortex.cn

JS:   items.join(",")
来源：http://zh.wgjwhj.cn

TS:   items.join(",")
来源：http://bt.bookmarksfly.cn

Java: String.join(",", items)
来源：http://ht.chemitech.net.cn

Go:   strings.Join(items, ",")
来源：http://kn.gzmigu.cn

Ruby: items.join(",")
来源：http://ex.shxzukj.cn

C#:   string.Join(",", items)
来源：http://sd.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://yv.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ft.asd995.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://io.nicolike.cn

JS:   s.replace(/\s+/g, "")
来源：http://ge.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://az.wgjwhj.cn

Java: s.replaceAll("\\s+", "")
来源：http://ll.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ra.bjjhwx.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gi.muxihuayi.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://no.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ix.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dr.hahajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hw.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://lp.huixiangedu.cn

TS:   "7".padStart(3, "0")
来源：http://yy.colortex.cn

Java: String.format("%03d", 7)
来源：http://zq.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://oi.9csxet.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sv.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fv.hnjuh.cn

[E11] 反转字符串
来源：http://uj.nszjky.cn

Py:   s[::-1]
来源：http://lu.lnxyls.cn

PHP:  strrev($s);
来源：http://gh.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://xi.yuntaijiaju.cn

TS:   [...s].reverse().join("")
来源：http://nc.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://gd.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gm.chemitech.net.cn

Ruby: s.reverse
来源：http://yw.huanxung.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xi.huanxung.cn

[E12] 统计某字符出现次数
来源：http://iw.huixiangedu.cn

Py:   s.count("a")
来源：http://ts.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://mq.jctech888.com.cn

JS:   s.split("a").length - 1
来源：http://ec.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://kh.shxzskj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hw.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://ry.huanxung.cn

Ruby: s.count("a")
来源：http://ov.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://xd.colortex.cn

[E13] 逐字符遍历
来源：http://px.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://so.colortex.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wj.yuexingan06.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yz.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ja.wgjwhj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://aq.szsharing.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://pl.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://hm.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kh.huanxung.cn

[E14] URL 编码与 Base64
来源：http://fh.gzmigu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xh.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bp.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://of.huixinmuqiang.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://za.shxzukj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gq.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hj.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://lr.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://df.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://yx.nszjky.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ws.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ek.muxihuayi.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://pi.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bq.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vk.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://kc.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://gu.muxihuayi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://qg.asd995.cn

[E16] 数字千分位
来源：http://rt.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://zd.521024.cn

PHP:  number_format(1234567);
来源：http://ry.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://kb.shxzskj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jq.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ca.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ts.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dw.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://gb.wgjwhj.cn

[E17] 首字母大写
来源：http://os.shxzskj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gx.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ic.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kb.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hr.shxzukj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ru.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://oo.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://fs.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ng.asd995.cn

[E18] 模板占位符替换
来源：http://sf.nicolike.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bl.huixinmuqiang.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ne.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://es.shtwfgs.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yv.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wc.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pl.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hv.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xb.szsharing.cn

[E19] 多行文本按行拆分
来源：http://le.asd995.cn

Py:   s.splitlines()
来源：http://lv.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xb.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://ae.hnjuh.cn

TS:   s.split(/\r?\n/)
来源：http://jn.hahajie.cn

Java: s.lines().toList()
来源：http://vw.muxihuayi.cn

Go:   strings.Split(s, "\n")
来源：http://wv.shtwfgs.cn

Ruby: s.lines
来源：http://ao.shtwfgs.cn

C#:   s.Split('\n')
来源：http://lx.newstarts.cn

[E20] 判断字符串是否为空
来源：http://qw.nicolike.cn

Py:   if not s:
来源：http://ky.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pe.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yv.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://iy.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://nq.huanxung.cn


<!-- 参考信息 -->