代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://td.shxzukj.cn

[D20] 统计每个元素出现次数
来源：http://py.hahajie.cn

Py:   Counter(arr)
来源：http://ow.9csxet.cn

PHP:  array_count_values($arr);
来源：http://an.lnxyls.cn

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://fl.shxzukj.cn

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://sf.jianghongdianzi.cn

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mj.hnjuh.cn

Go:   // 手写 map[T]int
来源：http://fu.muxihuayi.cn

Ruby: arr.tally
来源：http://cu.huixiangedu.cn

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://ec.asd995.cn

[D21] 判断是否包含某元素
来源：http://ap.gzmigu.cn

Py:   x in arr
来源：http://yr.szsharing.cn

PHP:  in_array($x, $arr, true);
来源：http://mv.huixinmuqiang.cn

JS:   arr.includes(x)
来源：http://ot.szsharing.cn

TS:   arr.includes(x)
来源：http://uh.521024.cn

Java: list.contains(x)
来源：http://ua.nicolike.cn

Go:   slices.Contains(arr, x)
来源：http://hn.colortex.cn

Ruby: arr.include?(x)
来源：http://th.bookmarksfly.cn

C#:   list.Contains(x)
来源：http://bl.lnxyls.cn

[D22] 复制数组（避免共享引用）
来源：http://xm.chemitech.net.cn

Py:   arr.copy();  arr[:];  list(arr)
来源：http://ur.nicolike.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hc.yuntaijiaju.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://lk.huanxung.cn

TS:   [...arr];
来源：http://rv.muxihuayi.cn

Java: new ArrayList<>(list);
来源：http://zw.colortex.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lb.shxzukj.cn

Ruby: arr.dup;  arr.clone
来源：http://gi.bjjhwx.cn

C#:   new List<int>(list);
来源：http://ej.huixiangedu.cn

[D23] reduce 累积计算
来源：http://sh.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://eu.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://ba.shtwfgs.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://qx.newstarts.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://dz.shtwfgs.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://uy.yuntaijiaju.cn

Go:   // 手写循环
来源：http://ps.bookmarksfly.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://jz.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ci.hnjuh.cn

[D24] 字典 / Map 基本操作
来源：http://ih.shxzukj.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ib.szsharing.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://ue.nszjky.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wg.huixinmuqiang.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://vg.szsharing.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://yg.jianghongdianzi.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zg.haigaiapp.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://an.newstarts.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ym.bookmarksfly.cn

[D25] Set 集合去重与交并差
来源：http://ws.yuntaijiaju.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://fk.shxzukj.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://ou.huixinmuqiang.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://pr.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://vw.huanxung.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://jn.yuntaijiaju.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://tb.colortex.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://sn.panjiajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://cp.newstarts.cn

[D26] 数组转字符串
来源：http://zt.szsharing.cn

Py:   ", ".join(map(str, arr))
来源：http://hz.shxzskj.cn

PHP:  implode(", ", $arr);
来源：http://nc.jianghongdianzi.cn

JS:   arr.join(", ")
来源：http://wp.shxzukj.cn

TS:   arr.join(", ")
来源：http://vk.huixiangedu.cn

Java: String.join(", ", list)
来源：http://gd.huixinmuqiang.cn

Go:   strings.Join(strs, ", ")
来源：http://nw.9csxet.cn

Ruby: arr.join(", ")
来源：http://gm.bookmarksfly.cn

C#:   string.Join(", ", list)
来源：http://se.szsharing.cn

================================================================================
来源：http://mr.shxzskj.cn

E. 字符串处理
来源：http://vl.9csxet.cn

================================================================================
来源：http://hg.huanxung.cn

[E01] 拼接字符串
来源：http://uy.szsharing.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ea.shxzskj.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://en.yuexingan06.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ih.colortex.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://sd.wgjwhj.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://lz.hahajie.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://bq.gzmigu.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hq.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://pe.521024.cn

[E02] 重复字符串
来源：http://oi.hahajie.cn

Py:   "ab" * 3
来源：http://nl.hnjuh.cn

PHP:  str_repeat("ab", 3);
来源：http://dh.newstarts.cn

JS:   "ab".repeat(3)
来源：http://vd.szxytkj.cn

TS:   "ab".repeat(3)
来源：http://hv.szsharing.cn

Java: "ab".repeat(3)
来源：http://th.9csxet.cn

Go:   strings.Repeat("ab", 3)
来源：http://zr.huanxung.cn

Ruby: "ab" * 3
来源：http://wy.shxzskj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wd.muxihuayi.cn

[E03] 截取子串
来源：http://nq.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://rs.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://an.bjjhwx.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pl.shtwfgs.cn

TS:   s.slice(1, 4)
来源：http://oh.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://vn.panjiajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://bx.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://ll.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://ry.nicolike.cn

[E04] 查找子串位置
来源：http://uu.huixiangedu.cn

Py:   s.find("x");  s.index("x")
来源：http://cv.hahajie.cn

PHP:  strpos($s, "x");
来源：http://eu.haigaiapp.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rq.shxzukj.cn

TS:   s.indexOf("x")
来源：http://sr.shxzskj.cn

Java: s.indexOf("x")
来源：http://gr.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://ri.chemitech.net.cn

Ruby: s.index("x")
来源：http://hf.hahajie.cn

C#:   s.IndexOf("x")
来源：http://yc.muxihuayi.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://kx.yuexingan06.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wr.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://vd.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://pu.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://er.shxzukj.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ev.521024.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://of.bookmarksfly.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bt.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mp.panjiajie.cn

[E06] 替换子串
来源：http://tb.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://gb.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://sq.huixiangedu.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://dt.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://aj.huixinmuqiang.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rg.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mw.panjiajie.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yc.szxytkj.cn

C#:   s.Replace("a", "b")
来源：http://tt.newstarts.cn

[E07] 按分隔符拆分
来源：http://dn.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hr.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ad.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ke.hnjuh.cn

TS:   s.split(",")
来源：http://xf.yuexingan06.cn

Java: s.split(",");  s.split("\\s+")
来源：http://sp.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bg.haigaiapp.cn

Ruby: s.split(",");  s.split
来源：http://ln.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mo.wgjwhj.cn

[E08] 数组按分隔符合并
来源：http://jf.lnxyls.cn

Py:   ",".join(items)
来源：http://np.shtwfgs.cn

PHP:  implode(",", $items);
来源：http://xf.521024.cn

JS:   items.join(",")
来源：http://ed.lnxyls.cn

TS:   items.join(",")
来源：http://qp.newstarts.cn

Java: String.join(",", items)
来源：http://wn.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://kk.szsharing.cn

Ruby: items.join(",")
来源：http://ho.hnjuh.cn

C#:   string.Join(",", items)
来源：http://gx.gzmigu.cn

[E09] 去除所有空白字符
来源：http://mb.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ut.yuntaijiaju.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wn.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://zl.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://qs.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://sa.bjjhwx.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ga.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://my.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ua.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://qu.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fa.chemitech.net.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ny.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ke.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://nw.panjiajie.cn

Java: String.format("%03d", 7)
来源：http://fm.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://cd.shtwfgs.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zn.hahajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vt.haigaiapp.cn

[E11] 反转字符串
来源：http://ie.huanxung.cn

Py:   s[::-1]
来源：http://aj.chemitech.net.cn

PHP:  strrev($s);
来源：http://ui.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://nn.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://jh.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sh.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://sm.chemitech.net.cn

Ruby: s.reverse
来源：http://tf.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://td.9csxet.cn

[E12] 统计某字符出现次数
来源：http://zp.szsharing.cn

Py:   s.count("a")
来源：http://kz.huanxung.cn

PHP:  substr_count($s, "a");
来源：http://uc.chemitech.net.cn

JS:   s.split("a").length - 1
来源：http://rg.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://lg.nszjky.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jg.hnjuh.cn

Go:   strings.Count(s, "a")
来源：http://bl.yuntaijiaju.cn

Ruby: s.count("a")
来源：http://ug.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://mc.newstarts.cn

[E13] 逐字符遍历
来源：http://mt.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://nl.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dh.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ne.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://nw.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://de.asd995.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cl.jctech888.com.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uo.hnjuh.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qw.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://pt.hnjuh.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://bv.lnxyls.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wa.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dd.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://aj.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pq.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nt.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://uk.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wl.huanxung.cn

[E15] HTML 转义 / 反转义
来源：http://cy.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://uz.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ey.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://oz.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://xu.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://gl.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pj.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ja.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vw.jctech888.com.cn

[E16] 数字千分位
来源：http://qt.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://eq.huixiangedu.cn

PHP:  number_format(1234567);
来源：http://ep.szsharing.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ne.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://jk.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dv.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yc.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fo.hahajie.cn

C#:   1234567.ToString("N0")
来源：http://yg.huixinmuqiang.cn

[E17] 首字母大写
来源：http://uw.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yv.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://se.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ik.szsharing.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xs.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ae.yuexingan06.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ab.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://md.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://at.bjjhwx.cn

[E18] 模板占位符替换
来源：http://sn.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://uz.jctech888.com.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://au.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://iv.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gl.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ls.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sx.wgjwhj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gs.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://um.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://lm.huixinmuqiang.cn

Py:   s.splitlines()
来源：http://ag.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ep.newstarts.cn

JS:   s.split(/\r?\n/)
来源：http://ho.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://tv.asd995.cn

Java: s.lines().toList()
来源：http://nf.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://mo.yuexingan06.cn

Ruby: s.lines
来源：http://zc.muxihuayi.cn

C#:   s.Split('\n')
来源：http://xa.9csxet.cn

[E20] 判断字符串是否为空
来源：http://sz.newstarts.cn

Py:   if not s:
来源：http://hz.nicolike.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rc.muxihuayi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tw.szxytkj.cn

TS:   if (s === "") {}
来源：http://cs.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://uk.yuntaijiaju.cn

Go:   if s == "" {}
来源：http://vp.lnxyls.cn

Ruby: if s.empty?
来源：http://yh.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xd.gzmigu.cn

[E21] 超长截断加省略号
来源：http://zn.hahajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kr.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qk.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://bj.521024.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://cx.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://la.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://zy.colortex.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qn.521024.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ip.nicolike.cn

[E22] 字节长度与字符长度
来源：http://ft.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ja.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hc.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tf.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://gs.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gf.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hk.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://qu.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ee.nicolike.cn

================================================================================
来源：http://vm.panjiajie.cn

F. 文件与目录
来源：http://hr.panjiajie.cn

================================================================================
来源：http://nf.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://rd.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hh.colortex.cn

PHP:  file_get_contents("a.txt");
来源：http://sb.szsharing.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://bs.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cy.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pa.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ji.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://xv.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://bm.521024.cn

[F02] 逐行读取文件
来源：http://bh.asd995.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nl.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mt.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fk.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kj.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wc.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jc.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uc.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ql.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://rp.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://og.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sx.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dn.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cb.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ab.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xw.gzmigu.cn

Ruby: File.write("a.txt", "hi")
来源：http://dz.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jd.nszjky.cn

[F04] 追加写入文件
来源：http://al.jctech888.com.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sx.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ha.chemitech.net.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://um.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xw.gzmigu.cn


<!-- 参考信息 -->