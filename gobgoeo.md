代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://fp.bjjhwx.cn

C#:   list.Sum();  list.Average()
来源：http://ki.wgjwhj.cn

[D17] 最大值与最小值
来源：http://gw.szxytkj.cn

Py:   max(arr);  min(arr)
来源：http://wf.521024.cn

PHP:  max($arr);  min($arr);
来源：http://ce.gzmigu.cn

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://dq.gzmigu.cn

TS:   Math.max(...arr);
来源：http://ul.huixiangedu.cn

Java: Collections.max(list);  Collections.min(list);
来源：http://to.szxytkj.cn

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://ys.jctech888.com.cn

Ruby: arr.max;  arr.min
来源：http://kt.huanxung.cn

C#:   list.Max();  list.Min()
来源：http://sx.bookmarksfly.cn

[D18] 扁平化嵌套数组
来源：http://kb.colortex.cn

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://fl.szxytkj.cn

PHP:  array_merge(...$nested);
来源：http://ju.haigaiapp.cn

JS:   nested.flat();  nested.flat(Infinity)
来源：http://il.gzmigu.cn

TS:   nested.flat();
来源：http://ry.nszjky.cn

Java: nested.stream().flatMap(List::stream).toList()
来源：http://re.gzmigu.cn

Go:   // 手写双层循环
来源：http://by.muxihuayi.cn

Ruby: nested.flatten
来源：http://ni.lnxyls.cn

C#:   nested.SelectMany(x => x).ToList()
来源：http://ns.jianghongdianzi.cn

[D19] 按字段分组
来源：http://sj.huixiangedu.cn

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://je.jctech888.com.cn

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://tc.huixinmuqiang.cn

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://jg.chemitech.net.cn

TS:   Object.groupBy(arr, x => x.type)
来源：http://yy.hnjuh.cn

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://ys.521024.cn

Go:   // 手写 map[string][]T
来源：http://ho.jianghongdianzi.cn

Ruby: arr.group_by { |x| x[:type] }
来源：http://fc.yuntaijiaju.cn

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://eh.yuntaijiaju.cn

[D20] 统计每个元素出现次数
来源：http://bo.haigaiapp.cn

Py:   Counter(arr)
来源：http://pl.hnjuh.cn

PHP:  array_count_values($arr);
来源：http://vc.gzmigu.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://kt.nszjky.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://lf.yuexingan06.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://ea.chemitech.net.cn

Go:   // 手写 map[T]int
来源：http://zi.hnjuh.cn

Ruby: arr.tally
来源：http://zp.asd995.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://np.jctech888.com.cn

[D21] 判断是否包含某元素
来源：http://rz.huixinmuqiang.cn

Py:   x in arr
来源：http://pz.asd995.cn

PHP:  in_array($x, $arr, true);
来源：http://aq.bookmarksfly.cn

JS:   arr.includes(x)
来源：http://mu.wgjwhj.cn

TS:   arr.includes(x)
来源：http://xp.bookmarksfly.cn

Java: list.contains(x)
来源：http://aa.szsharing.cn

Go:   slices.Contains(arr, x)
来源：http://te.9csxet.cn

Ruby: arr.include?(x)
来源：http://ag.bjjhwx.cn

C#:   list.Contains(x)
来源：http://mn.newstarts.cn

[D22] 复制数组（避免共享引用）
来源：http://cz.bjjhwx.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://gg.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://nj.bjjhwx.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gj.huanxung.cn

TS:   [...arr];
来源：http://el.9csxet.cn

Java: new ArrayList<>(list);
来源：http://bz.shxzukj.cn

Go:   copied := append([]int(nil), arr...)
来源：http://cq.nszjky.cn

Ruby: arr.dup;  arr.clone
来源：http://fo.huixinmuqiang.cn

C#:   new List<int>(list);
来源：http://jh.hnjuh.cn

[D23] reduce 累积计算
来源：http://ps.9csxet.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://xy.jianghongdianzi.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ei.szxytkj.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ft.yuexingan06.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://ed.bookmarksfly.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://ri.lnxyls.cn

Go:   // 手写循环
来源：http://pa.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://yp.haigaiapp.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://bi.shxzskj.cn

[D24] 字典 / Map 基本操作
来源：http://hz.jctech888.com.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://kr.9csxet.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://gq.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://vi.muxihuayi.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://jz.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hq.newstarts.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hb.szxytkj.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://ct.gzmigu.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://jx.huixiangedu.cn

[D25] Set 集合去重与交并差
来源：http://hz.gzmigu.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ck.nicolike.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://qm.panjiajie.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://lr.gzmigu.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://lo.wgjwhj.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jb.newstarts.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://qh.9csxet.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://ss.szxytkj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://di.chemitech.net.cn

[D26] 数组转字符串
来源：http://pf.huanxung.cn

Py:   ", ".join(map(str, arr))
来源：http://sc.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://oj.yuntaijiaju.cn

JS:   arr.join(", ")
来源：http://hc.521024.cn

TS:   arr.join(", ")
来源：http://qr.jianghongdianzi.cn

Java: String.join(", ", list)
来源：http://ky.colortex.cn

Go:   strings.Join(strs, ", ")
来源：http://lw.lnxyls.cn

Ruby: arr.join(", ")
来源：http://vn.panjiajie.cn

C#:   string.Join(", ", list)
来源：http://uq.hahajie.cn

================================================================================
来源：http://hc.nicolike.cn

E. 字符串处理
来源：http://su.gzmigu.cn

================================================================================
来源：http://nz.huixinmuqiang.cn

[E01] 拼接字符串
来源：http://qr.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://uf.colortex.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ns.gzmigu.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wi.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://qs.nicolike.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ef.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wd.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://oh.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ec.jianghongdianzi.cn

[E02] 重复字符串
来源：http://fh.szxytkj.cn

Py:   "ab" * 3
来源：http://io.yuntaijiaju.cn

PHP:  str_repeat("ab", 3);
来源：http://cb.hahajie.cn

JS:   "ab".repeat(3)
来源：http://fg.panjiajie.cn

TS:   "ab".repeat(3)
来源：http://my.colortex.cn

Java: "ab".repeat(3)
来源：http://sr.bookmarksfly.cn

Go:   strings.Repeat("ab", 3)
来源：http://zf.szsharing.cn

Ruby: "ab" * 3
来源：http://pr.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://lb.panjiajie.cn

[E03] 截取子串
来源：http://nw.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://pu.panjiajie.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ag.asd995.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://jz.yuntaijiaju.cn

TS:   s.slice(1, 4)
来源：http://xb.shxzskj.cn

Java: s.substring(1, 4)
来源：http://xq.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yn.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://iz.chemitech.net.cn

C#:   s.Substring(1, 3)
来源：http://pe.shtwfgs.cn

[E04] 查找子串位置
来源：http://im.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://jh.521024.cn

PHP:  strpos($s, "x");
来源：http://gs.nicolike.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://py.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://lw.lnxyls.cn

Java: s.indexOf("x")
来源：http://ti.gzmigu.cn

Go:   strings.Index(s, "x")
来源：http://ma.hnjuh.cn

Ruby: s.index("x")
来源：http://vx.asd995.cn

C#:   s.IndexOf("x")
来源：http://in.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://mp.hnjuh.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://uj.muxihuayi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://au.colortex.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://su.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ui.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://uz.nszjky.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://lb.szsharing.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://pd.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://kc.haigaiapp.cn

[E06] 替换子串
来源：http://hn.hnjuh.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://cn.shxzukj.cn

PHP:  str_replace("a", "b", $s);
来源：http://oo.shxzukj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yx.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ba.yuexingan06.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ji.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://aq.yuexingan06.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qk.chemitech.net.cn

C#:   s.Replace("a", "b")
来源：http://qx.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://fp.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://um.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sb.chemitech.net.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ac.9csxet.cn

TS:   s.split(",")
来源：http://nu.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://zv.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ao.hnjuh.cn

Ruby: s.split(",");  s.split
来源：http://fb.yuntaijiaju.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://is.lnxyls.cn

[E08] 数组按分隔符合并
来源：http://wk.gzmigu.cn

Py:   ",".join(items)
来源：http://ul.521024.cn

PHP:  implode(",", $items);
来源：http://bd.hnjuh.cn

JS:   items.join(",")
来源：http://ol.bjjhwx.cn

TS:   items.join(",")
来源：http://py.panjiajie.cn

Java: String.join(",", items)
来源：http://ml.bookmarksfly.cn

Go:   strings.Join(items, ",")
来源：http://lp.asd995.cn

Ruby: items.join(",")
来源：http://iq.9csxet.cn

C#:   string.Join(",", items)
来源：http://df.nicolike.cn

[E09] 去除所有空白字符
来源：http://vh.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://li.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://uj.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://pe.shtwfgs.cn

TS:   s.replace(/\s+/g, "")
来源：http://nb.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://rc.yuntaijiaju.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://pw.szxytkj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://gx.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://uh.lnxyls.cn

[E10] 左侧补零 / 定长填充
来源：http://db.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rc.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ll.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://pj.szsharing.cn

TS:   "7".padStart(3, "0")
来源：http://ah.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://mp.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rm.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://pf.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yu.jianghongdianzi.cn

[E11] 反转字符串
来源：http://vd.jctech888.com.cn

Py:   s[::-1]
来源：http://fs.shtwfgs.cn

PHP:  strrev($s);
来源：http://fh.yuntaijiaju.cn

JS:   [...s].reverse().join("")
来源：http://uo.bjjhwx.cn

TS:   [...s].reverse().join("")
来源：http://gg.haigaiapp.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bd.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gj.yuntaijiaju.cn

Ruby: s.reverse
来源：http://rn.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sy.nicolike.cn

[E12] 统计某字符出现次数
来源：http://bx.muxihuayi.cn

Py:   s.count("a")
来源：http://hx.wgjwhj.cn

PHP:  substr_count($s, "a");
来源：http://xh.jianghongdianzi.cn

JS:   s.split("a").length - 1
来源：http://wx.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://ht.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gp.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://oc.yuexingan06.cn

Ruby: s.count("a")
来源：http://pa.haigaiapp.cn

C#:   s.Count(c => c == 'a')
来源：http://vf.hnjuh.cn

[E13] 逐字符遍历
来源：http://xd.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://se.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://sm.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://vt.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://dm.szxytkj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://do.nszjky.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ai.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://wl.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hg.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://ca.yuntaijiaju.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://td.newstarts.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ld.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://tn.nszjky.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ud.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vs.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rr.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://vi.nicolike.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fu.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://dc.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://eo.nicolike.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://tv.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://px.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mz.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cu.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xy.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vv.chemitech.net.cn

[E16] 数字千分位
来源：http://su.chemitech.net.cn

Py:   f"{1234567:,}"
来源：http://xr.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://yv.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://cz.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ai.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://rs.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nj.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://zg.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://kp.yuntaijiaju.cn

[E17] 首字母大写
来源：http://jl.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wg.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rw.szxytkj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ul.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kw.lnxyls.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://rj.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://uc.9csxet.cn

Ruby: s.capitalize
来源：http://py.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://gz.szsharing.cn

[E18] 模板占位符替换
来源：http://ks.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ip.haigaiapp.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://td.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jz.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ot.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ea.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hu.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sq.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yq.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://qm.nicolike.cn

Py:   s.splitlines()
来源：http://iw.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qs.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://oo.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://qx.szsharing.cn

Java: s.lines().toList()
来源：http://nf.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://jb.nicolike.cn

Ruby: s.lines
来源：http://nl.chemitech.net.cn

C#:   s.Split('\n')
来源：http://or.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://la.jianghongdianzi.cn

Py:   if not s:
来源：http://rr.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oh.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.shxzukj.cn

TS:   if (s === "") {}
来源：http://ga.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://kp.chemitech.net.cn

Go:   if s == "" {}
来源：http://mm.yuexingan06.cn

Ruby: if s.empty?
来源：http://wp.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ac.szxytkj.cn

[E21] 超长截断加省略号
来源：http://bs.newstarts.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://vj.huanxung.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qh.colortex.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ns.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mr.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://pk.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://xf.huixinmuqiang.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tm.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hs.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://dl.shxzskj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://tx.hahajie.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tv.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sm.colortex.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lv.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://lt.muxihuayi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dt.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://ey.huanxung.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://at.9csxet.cn

================================================================================
来源：http://ch.panjiajie.cn

F. 文件与目录
来源：http://fi.lnxyls.cn

================================================================================
来源：http://qz.wgjwhj.cn

[F01] 读取整个文件
来源：http://pa.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://di.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://kv.hahajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ht.huixinmuqiang.cn


<!-- 参考信息 -->