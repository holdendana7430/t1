代发 wailian999

C#:   list.Distinct().ToList()
来源：http://fa.huixinmuqiang.cn

[D16] 求和与平均值
来源：http://ub.shtwfgs.cn

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://pm.nszjky.cn

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://le.huixiangedu.cn

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://yo.szxytkj.cn

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://jh.jianghongdianzi.cn

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://en.jctech888.com.cn

Go:   // 手写循环累加
来源：http://vt.yuntaijiaju.cn

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://gi.hahajie.cn

C#:   list.Sum();  list.Average()
来源：http://ks.jctech888.com.cn

[D17] 最大值与最小值
来源：http://kt.shxzskj.cn

Py:   max(arr);  min(arr)
来源：http://ji.hahajie.cn

PHP:  max($arr);  min($arr);
来源：http://gi.shxzukj.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://ey.wgjwhj.cn

TS:   Math.max(...arr);
来源：http://hv.wgjwhj.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://pj.nicolike.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://qo.panjiajie.cn

Ruby: arr.max;  arr.min
来源：http://js.yuntaijiaju.cn

C#:   list.Max();  list.Min()
来源：http://cf.yuexingan06.cn

[D18] 扁平化嵌套数组
来源：http://kf.newstarts.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://ks.gzmigu.cn

PHP:  array_merge(...$nested);
来源：http://fq.lnxyls.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wk.asd995.cn

TS:   nested.flat();
来源：http://in.jctech888.com.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://yt.yuntaijiaju.cn

Go:   // 手写双层循环
来源：http://yn.panjiajie.cn

Ruby: nested.flatten
来源：http://bn.newstarts.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://zp.colortex.cn

[D19] 按字段分组
来源：http://dl.szxytkj.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://vi.hahajie.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://er.shxzskj.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://zo.bookmarksfly.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://oq.9csxet.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://xb.hnjuh.cn

Go:   // 手写 map[string][]T
来源：http://sn.lnxyls.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://qy.panjiajie.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://yb.yuexingan06.cn

[D20] 统计每个元素出现次数
来源：http://xk.521024.cn

Py:   Counter(arr)
来源：http://su.chemitech.net.cn

PHP:  array_count_values($arr);
来源：http://ew.nicolike.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://jk.asd995.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://oo.newstarts.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://cb.huixiangedu.cn

Go:   // 手写 map[T]int
来源：http://fo.asd995.cn

Ruby: arr.tally
来源：http://xg.yuntaijiaju.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://gv.panjiajie.cn

[D21] 判断是否包含某元素
来源：http://bv.lnxyls.cn

Py:   x in arr
来源：http://wz.huixiangedu.cn

PHP:  in_array($x, $arr, true);
来源：http://uu.shxzukj.cn

JS:   arr.includes(x)
来源：http://ry.gzmigu.cn

TS:   arr.includes(x)
来源：http://vc.newstarts.cn

Java: list.contains(x)
来源：http://dr.521024.cn

Go:   slices.Contains(arr, x)
来源：http://sp.nszjky.cn

Ruby: arr.include?(x)
来源：http://aj.hahajie.cn

C#:   list.Contains(x)
来源：http://td.wgjwhj.cn

[D22] 复制数组（避免共享引用）
来源：http://vp.jianghongdianzi.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://oy.haigaiapp.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://xh.huixinmuqiang.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lu.yuexingan06.cn

TS:   [...arr];
来源：http://dy.huanxung.cn

Java: new ArrayList<>(list);
来源：http://wx.szsharing.cn

Go:   copied := append([]int(nil), arr...)
来源：http://us.yuexingan06.cn

Ruby: arr.dup;  arr.clone
来源：http://nq.szxytkj.cn

C#:   new List<int>(list);
来源：http://mz.jctech888.com.cn

[D23] reduce 累积计算
来源：http://my.hahajie.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gg.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://md.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://xu.haigaiapp.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://iv.panjiajie.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://xk.shtwfgs.cn

Go:   // 手写循环
来源：http://um.jianghongdianzi.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ox.panjiajie.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://eu.huixinmuqiang.cn

[D24] 字典 / Map 基本操作
来源：http://vr.9csxet.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mu.jctech888.com.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ty.bjjhwx.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nl.hnjuh.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://tq.colortex.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wg.huanxung.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://xq.newstarts.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://vl.shxzukj.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://pu.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://he.bookmarksfly.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://tl.9csxet.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://aj.bookmarksfly.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://bh.newstarts.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ks.yuexingan06.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://uk.huixiangedu.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://er.asd995.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ci.chemitech.net.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://la.521024.cn

[D26] 数组转字符串
来源：http://vt.bjjhwx.cn

Py:   ", ".join(map(str, arr))
来源：http://ur.chemitech.net.cn

PHP:  implode(", ", $arr);
来源：http://zx.hahajie.cn

JS:   arr.join(", ")
来源：http://bl.huixiangedu.cn

TS:   arr.join(", ")
来源：http://lp.hnjuh.cn

Java: String.join(", ", list)
来源：http://mj.newstarts.cn

Go:   strings.Join(strs, ", ")
来源：http://wc.panjiajie.cn

Ruby: arr.join(", ")
来源：http://ir.lnxyls.cn

C#:   string.Join(", ", list)
来源：http://fp.hahajie.cn

================================================================================
来源：http://st.hahajie.cn

E. 字符串处理
来源：http://oo.hnjuh.cn

================================================================================
来源：http://md.nszjky.cn

[E01] 拼接字符串
来源：http://lh.hahajie.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://sv.hahajie.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://pt.asd995.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://el.muxihuayi.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://cb.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://gq.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://ak.szsharing.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://dq.521024.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yf.wgjwhj.cn

[E02] 重复字符串
来源：http://yo.huanxung.cn

Py:   "ab" * 3
来源：http://ro.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://dw.newstarts.cn

JS:   "ab".repeat(3)
来源：http://nz.muxihuayi.cn

TS:   "ab".repeat(3)
来源：http://us.huanxung.cn

Java: "ab".repeat(3)
来源：http://no.hnjuh.cn

Go:   strings.Repeat("ab", 3)
来源：http://sh.shxzukj.cn

Ruby: "ab" * 3
来源：http://lw.szxytkj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ll.bookmarksfly.cn

[E03] 截取子串
来源：http://ys.wgjwhj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://bn.colortex.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hq.shtwfgs.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://nq.szsharing.cn

TS:   s.slice(1, 4)
来源：http://by.chemitech.net.cn

Java: s.substring(1, 4)
来源：http://fg.szsharing.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pd.nicolike.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ws.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://xe.jctech888.com.cn

[E04] 查找子串位置
来源：http://ol.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://jb.haigaiapp.cn

PHP:  strpos($s, "x");
来源：http://gs.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ga.nszjky.cn

TS:   s.indexOf("x")
来源：http://ri.yuexingan06.cn

Java: s.indexOf("x")
来源：http://fg.colortex.cn

Go:   strings.Index(s, "x")
来源：http://mt.szxytkj.cn

Ruby: s.index("x")
来源：http://es.huixiangedu.cn

C#:   s.IndexOf("x")
来源：http://be.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://pb.colortex.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://tm.lnxyls.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wg.jctech888.com.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://km.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hn.muxihuayi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://nd.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://kg.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vc.huixiangedu.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://ns.huixinmuqiang.cn

[E06] 替换子串
来源：http://ho.shxzukj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kg.hahajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://an.lnxyls.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mj.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://wo.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://pq.521024.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zl.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://rd.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://zb.bookmarksfly.cn

[E07] 按分隔符拆分
来源：http://tn.521024.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://uy.bookmarksfly.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://tv.jianghongdianzi.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://eq.panjiajie.cn

TS:   s.split(",")
来源：http://si.haigaiapp.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jw.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://zj.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://lr.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zl.521024.cn

[E08] 数组按分隔符合并
来源：http://sq.panjiajie.cn

Py:   ",".join(items)
来源：http://fm.bookmarksfly.cn

PHP:  implode(",", $items);
来源：http://xs.nicolike.cn

JS:   items.join(",")
来源：http://rv.newstarts.cn

TS:   items.join(",")
来源：http://zy.wgjwhj.cn

Java: String.join(",", items)
来源：http://sj.szxytkj.cn

Go:   strings.Join(items, ",")
来源：http://xi.haigaiapp.cn

Ruby: items.join(",")
来源：http://zy.nszjky.cn

C#:   string.Join(",", items)
来源：http://mk.nszjky.cn

[E09] 去除所有空白字符
来源：http://jg.newstarts.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://to.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ht.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://bn.gzmigu.cn

TS:   s.replace(/\s+/g, "")
来源：http://wo.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://en.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yu.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bb.colortex.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://io.yuntaijiaju.cn

[E10] 左侧补零 / 定长填充
来源：http://wn.asd995.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ce.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ds.yuntaijiaju.cn

JS:   "7".padStart(3, "0")
来源：http://qg.9csxet.cn

TS:   "7".padStart(3, "0")
来源：http://cz.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://ly.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ef.huixiangedu.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://gl.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://no.bookmarksfly.cn

[E11] 反转字符串
来源：http://uf.chemitech.net.cn

Py:   s[::-1]
来源：http://uo.bookmarksfly.cn

PHP:  strrev($s);
来源：http://fh.9csxet.cn

JS:   [...s].reverse().join("")
来源：http://ex.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://is.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qr.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://zd.panjiajie.cn

Ruby: s.reverse
来源：http://rc.wgjwhj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sx.muxihuayi.cn

[E12] 统计某字符出现次数
来源：http://ib.huixinmuqiang.cn

Py:   s.count("a")
来源：http://cs.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://yj.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://ek.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://fz.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dx.bjjhwx.cn

Go:   strings.Count(s, "a")
来源：http://aq.asd995.cn

Ruby: s.count("a")
来源：http://fp.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://gm.jianghongdianzi.cn

[E13] 逐字符遍历
来源：http://qv.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://ga.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://xj.huixinmuqiang.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dl.wgjwhj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wu.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qi.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cj.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cj.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ua.muxihuayi.cn

[E14] URL 编码与 Base64
来源：http://ex.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ru.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dn.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hn.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ne.hnjuh.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yw.panjiajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wc.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://af.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://vq.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://hy.wgjwhj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://an.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sk.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wm.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jm.panjiajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://op.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://nz.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://az.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://un.wgjwhj.cn

[E16] 数字千分位
来源：http://lx.szsharing.cn

Py:   f"{1234567:,}"
来源：http://zw.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://io.muxihuayi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qz.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sm.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ki.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://up.jctech888.com.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://rz.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://gi.panjiajie.cn

[E17] 首字母大写
来源：http://wz.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uf.nicolike.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ij.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xf.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jh.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://yi.jianghongdianzi.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ev.lnxyls.cn

Ruby: s.capitalize
来源：http://mf.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bb.panjiajie.cn

[E18] 模板占位符替换
来源：http://kw.jianghongdianzi.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mi.gzmigu.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://rk.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xl.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://km.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kt.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lr.hnjuh.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mj.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://et.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://ej.huixiangedu.cn

Py:   s.splitlines()
来源：http://wo.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mb.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://ml.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://ds.chemitech.net.cn

Java: s.lines().toList()
来源：http://gf.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://ys.nicolike.cn

Ruby: s.lines
来源：http://zx.panjiajie.cn

C#:   s.Split('\n')
来源：http://pw.colortex.cn

[E20] 判断字符串是否为空
来源：http://bf.chemitech.net.cn

Py:   if not s:
来源：http://yo.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jm.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ei.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://xz.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://hz.hahajie.cn

Go:   if s == "" {}
来源：http://om.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://cf.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://zt.colortex.cn

[E21] 超长截断加省略号
来源：http://jz.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xe.newstarts.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://vj.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tb.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nv.hnjuh.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://kv.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://bm.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wa.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zm.newstarts.cn

[E22] 字节长度与字符长度
来源：http://qv.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mr.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ih.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ir.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ze.bookmarksfly.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ug.newstarts.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ao.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://rl.chemitech.net.cn


<!-- 参考信息 -->