代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://di.huixinmuqiang.cn

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://pt.haigaiapp.cn

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://gf.huixiangedu.cn

TS:   [...arr];
来源：http://sq.jianghongdianzi.cn

Java: new ArrayList<>(list);
来源：http://yy.haigaiapp.cn

Go:   copied := append([]int(nil), arr...)
来源：http://lw.yuntaijiaju.cn

Ruby: arr.dup;  arr.clone
来源：http://ph.jianghongdianzi.cn

C#:   new List<int>(list);
来源：http://zo.huanxung.cn

[D23] reduce 累积计算
来源：http://ir.szxytkj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wy.gzmigu.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://yh.521024.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://gw.huixiangedu.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://kk.jianghongdianzi.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://be.huixiangedu.cn

Go:   // 手写循环
来源：http://le.szsharing.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://ef.9csxet.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://ve.yuexingan06.cn

[D24] 字典 / Map 基本操作
来源：http://uh.bjjhwx.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://rw.nszjky.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://fc.nicolike.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://gr.shxzskj.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://md.jctech888.com.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://aa.colortex.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://sp.szsharing.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://xp.nszjky.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://gz.yuexingan06.cn

[D25] Set 集合去重与交并差
来源：http://fn.jctech888.com.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://kc.hnjuh.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://lm.hnjuh.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hk.jctech888.com.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://by.nicolike.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://kg.nszjky.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ud.haigaiapp.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hd.nicolike.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://dk.panjiajie.cn

[D26] 数组转字符串
来源：http://ux.colortex.cn

Py:   ", ".join(map(str, arr))
来源：http://rr.jianghongdianzi.cn

PHP:  implode(", ", $arr);
来源：http://cx.panjiajie.cn

JS:   arr.join(", ")
来源：http://io.shxzukj.cn

TS:   arr.join(", ")
来源：http://oi.panjiajie.cn

Java: String.join(", ", list)
来源：http://zg.huixiangedu.cn

Go:   strings.Join(strs, ", ")
来源：http://kb.huanxung.cn

Ruby: arr.join(", ")
来源：http://ds.bjjhwx.cn

C#:   string.Join(", ", list)
来源：http://hp.nicolike.cn

================================================================================
来源：http://cv.panjiajie.cn

E. 字符串处理
来源：http://it.yuexingan06.cn

================================================================================
来源：http://fj.yuexingan06.cn

[E01] 拼接字符串
来源：http://zw.lnxyls.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://ab.yuexingan06.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://lk.panjiajie.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://ix.panjiajie.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://of.jctech888.com.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://np.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://sw.bjjhwx.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yo.szsharing.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ij.shxzskj.cn

[E02] 重复字符串
来源：http://wx.lnxyls.cn

Py:   "ab" * 3
来源：http://py.nszjky.cn

PHP:  str_repeat("ab", 3);
来源：http://hi.shxzskj.cn

JS:   "ab".repeat(3)
来源：http://ok.huixinmuqiang.cn

TS:   "ab".repeat(3)
来源：http://qb.szsharing.cn

Java: "ab".repeat(3)
来源：http://ft.bjjhwx.cn

Go:   strings.Repeat("ab", 3)
来源：http://kf.hahajie.cn

Ruby: "ab" * 3
来源：http://qb.lnxyls.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://qj.hnjuh.cn

[E03] 截取子串
来源：http://ej.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zq.haigaiapp.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ef.nicolike.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ss.yuexingan06.cn

TS:   s.slice(1, 4)
来源：http://gl.szxytkj.cn

Java: s.substring(1, 4)
来源：http://qr.shxzskj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ml.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hg.hnjuh.cn

C#:   s.Substring(1, 3)
来源：http://ak.huixiangedu.cn

[E04] 查找子串位置
来源：http://tl.muxihuayi.cn

Py:   s.find("x");  s.index("x")
来源：http://he.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://mr.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://rw.shxzukj.cn

TS:   s.indexOf("x")
来源：http://bp.huixiangedu.cn

Java: s.indexOf("x")
来源：http://sp.hahajie.cn

Go:   strings.Index(s, "x")
来源：http://eq.hahajie.cn

Ruby: s.index("x")
来源：http://od.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://ef.521024.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://in.lnxyls.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ez.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://cf.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://yp.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://pf.huixinmuqiang.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ef.bjjhwx.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://cq.chemitech.net.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ie.9csxet.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wj.huixiangedu.cn

[E06] 替换子串
来源：http://yb.hahajie.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://se.521024.cn

PHP:  str_replace("a", "b", $s);
来源：http://jk.bjjhwx.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://lc.asd995.cn

TS:   s.replaceAll("a", "b")
来源：http://ki.lnxyls.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tm.haigaiapp.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://uo.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://gz.bjjhwx.cn

C#:   s.Replace("a", "b")
来源：http://eo.521024.cn

[E07] 按分隔符拆分
来源：http://mj.hahajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gs.panjiajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gt.huixinmuqiang.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pq.hnjuh.cn

TS:   s.split(",")
来源：http://sj.muxihuayi.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jl.haigaiapp.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bu.asd995.cn

Ruby: s.split(",");  s.split
来源：http://aj.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://dy.panjiajie.cn

[E08] 数组按分隔符合并
来源：http://en.muxihuayi.cn

Py:   ",".join(items)
来源：http://mr.szsharing.cn

PHP:  implode(",", $items);
来源：http://td.hnjuh.cn

JS:   items.join(",")
来源：http://fp.bjjhwx.cn

TS:   items.join(",")
来源：http://qe.colortex.cn

Java: String.join(",", items)
来源：http://qp.521024.cn

Go:   strings.Join(items, ",")
来源：http://nr.colortex.cn

Ruby: items.join(",")
来源：http://aj.yuexingan06.cn

C#:   string.Join(",", items)
来源：http://jz.wgjwhj.cn

[E09] 去除所有空白字符
来源：http://hb.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://fi.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://qx.lnxyls.cn

JS:   s.replace(/\s+/g, "")
来源：http://qu.jianghongdianzi.cn

TS:   s.replace(/\s+/g, "")
来源：http://fz.jianghongdianzi.cn

Java: s.replaceAll("\\s+", "")
来源：http://ko.szsharing.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://cw.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kg.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ip.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://we.hnjuh.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://qx.asd995.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qt.nszjky.cn

JS:   "7".padStart(3, "0")
来源：http://he.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://pd.colortex.cn

Java: String.format("%03d", 7)
来源：http://qr.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kn.huixinmuqiang.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lw.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rd.huixinmuqiang.cn

[E11] 反转字符串
来源：http://wr.shxzukj.cn

Py:   s[::-1]
来源：http://ld.szxytkj.cn

PHP:  strrev($s);
来源：http://re.hnjuh.cn

JS:   [...s].reverse().join("")
来源：http://pb.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://hp.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bh.szsharing.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://en.shxzukj.cn

Ruby: s.reverse
来源：http://io.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://il.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://oe.shxzskj.cn

Py:   s.count("a")
来源：http://ad.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://vv.huixinmuqiang.cn

JS:   s.split("a").length - 1
来源：http://tc.lnxyls.cn

TS:   s.split("a").length - 1
来源：http://xi.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ls.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://ne.lnxyls.cn

Ruby: s.count("a")
来源：http://uu.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://wd.asd995.cn

[E13] 逐字符遍历
来源：http://ej.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://wf.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://yc.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sx.newstarts.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ak.521024.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rk.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://rb.lnxyls.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yc.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://im.jianghongdianzi.cn

[E14] URL 编码与 Base64
来源：http://et.nszjky.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tm.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://vl.huixinmuqiang.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fr.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://xy.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xv.hahajie.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ph.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kj.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wl.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://tg.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://mi.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bn.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wb.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sg.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://eu.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://pw.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ot.9csxet.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vs.szxytkj.cn

[E16] 数字千分位
来源：http://lj.panjiajie.cn

Py:   f"{1234567:,}"
来源：http://bo.szxytkj.cn

PHP:  number_format(1234567);
来源：http://hm.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://mw.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ff.jctech888.com.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tk.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qe.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ne.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://yn.wgjwhj.cn

[E17] 首字母大写
来源：http://uh.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dx.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://na.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ir.521024.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ne.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://if.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mi.bjjhwx.cn

Ruby: s.capitalize
来源：http://yt.haigaiapp.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ev.jctech888.com.cn

[E18] 模板占位符替换
来源：http://tj.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://yv.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xg.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zr.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://td.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zw.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://pa.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uz.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mx.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://op.newstarts.cn

Py:   s.splitlines()
来源：http://mi.chemitech.net.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://po.szsharing.cn

JS:   s.split(/\r?\n/)
来源：http://ko.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://pb.newstarts.cn

Java: s.lines().toList()
来源：http://mm.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://ta.shxzukj.cn

Ruby: s.lines
来源：http://op.shxzskj.cn

C#:   s.Split('\n')
来源：http://xy.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://hl.hahajie.cn

Py:   if not s:
来源：http://zs.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://pn.gzmigu.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://tc.shxzskj.cn

TS:   if (s === "") {}
来源：http://gl.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://xz.shxzukj.cn

Go:   if s == "" {}
来源：http://li.gzmigu.cn

Ruby: if s.empty?
来源：http://mp.asd995.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qo.panjiajie.cn

[E21] 超长截断加省略号
来源：http://sf.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fu.colortex.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gj.gzmigu.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yp.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jy.haigaiapp.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hg.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ny.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ad.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ca.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://ai.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rq.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://fq.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qj.newstarts.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cy.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vf.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ia.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://yb.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mt.shxzukj.cn

================================================================================
来源：http://yd.gzmigu.cn

F. 文件与目录
来源：http://eq.panjiajie.cn

================================================================================
来源：http://nx.jctech888.com.cn

[F01] 读取整个文件
来源：http://sb.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nd.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://ls.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gp.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qo.shtwfgs.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yl.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://qc.colortex.cn

Ruby: File.read("a.txt")
来源：http://kl.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://fq.yuexingan06.cn

[F02] 逐行读取文件
来源：http://it.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://an.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ty.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xp.szsharing.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bc.nicolike.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ka.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://rv.muxihuayi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://oc.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xj.521024.cn

[F03] 写入文件（覆盖）
来源：http://ft.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ba.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ic.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sh.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iy.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sq.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://oh.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://py.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rm.gzmigu.cn

[F04] 追加写入文件
来源：http://uz.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hv.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rf.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ze.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ww.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vd.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ud.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pk.haigaiapp.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://bs.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://qa.jctech888.com.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qf.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://lz.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://xx.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://hr.bjjhwx.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nz.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zo.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://lq.521024.cn

C#:   File.Exists("a.txt")
来源：http://lm.hnjuh.cn

[F06] 删除文件
来源：http://xy.chemitech.net.cn

Py:   os.remove("a.txt")
来源：http://cm.szsharing.cn

PHP:  unlink("a.txt");
来源：http://an.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yq.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://iq.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bg.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://pm.szsharing.cn


<!-- 参考信息 -->