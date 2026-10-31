代发 wailian999

[D23] reduce 累积计算
来源：http://ei.shxzskj.cn

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://gi.panjiajie.cn

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://nb.chemitech.net.cn

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://vj.9csxet.cn

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wb.lnxyls.cn

Java: list.stream().reduce(0, Integer::sum)
来源：http://tv.gzmigu.cn

Go:   // 手写循环
来源：http://py.yuntaijiaju.cn

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://vq.muxihuayi.cn

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://fm.colortex.cn

[D24] 字典 / Map 基本操作
来源：http://tc.jianghongdianzi.cn

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://ay.huixiangedu.cn

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mb.jctech888.com.cn

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://nf.chemitech.net.cn

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://ai.shtwfgs.cn

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://st.wgjwhj.cn

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://zv.bookmarksfly.cn

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://qd.bjjhwx.cn

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://ck.shxzskj.cn

[D25] Set 集合去重与交并差
来源：http://ty.521024.cn

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://ed.jianghongdianzi.cn

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://db.jctech888.com.cn

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://zi.asd995.cn

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://ok.panjiajie.cn

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://pn.szsharing.cn

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://fr.newstarts.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://fn.hahajie.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://tu.huixinmuqiang.cn

[D26] 数组转字符串
来源：http://ku.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://jy.haigaiapp.cn

PHP:  implode(", ", $arr);
来源：http://ol.shxzskj.cn

JS:   arr.join(", ")
来源：http://he.gzmigu.cn

TS:   arr.join(", ")
来源：http://sr.huixiangedu.cn

Java: String.join(", ", list)
来源：http://pb.shxzukj.cn

Go:   strings.Join(strs, ", ")
来源：http://fb.shxzskj.cn

Ruby: arr.join(", ")
来源：http://lv.shxzukj.cn

C#:   string.Join(", ", list)
来源：http://vx.muxihuayi.cn

================================================================================
来源：http://to.huixinmuqiang.cn

E. 字符串处理
来源：http://zc.hnjuh.cn

================================================================================
来源：http://sm.shxzskj.cn

[E01] 拼接字符串
来源：http://hj.asd995.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://be.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://yu.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://kb.newstarts.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://lc.huixinmuqiang.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://du.muxihuayi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://nf.szxytkj.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://yi.newstarts.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://av.szsharing.cn

[E02] 重复字符串
来源：http://en.shxzukj.cn

Py:   "ab" * 3
来源：http://wb.szsharing.cn

PHP:  str_repeat("ab", 3);
来源：http://qs.bjjhwx.cn

JS:   "ab".repeat(3)
来源：http://pb.huixiangedu.cn

TS:   "ab".repeat(3)
来源：http://fb.521024.cn

Java: "ab".repeat(3)
来源：http://zn.gzmigu.cn

Go:   strings.Repeat("ab", 3)
来源：http://we.colortex.cn

Ruby: "ab" * 3
来源：http://nt.521024.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dj.szsharing.cn

[E03] 截取子串
来源：http://et.nicolike.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://gs.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://fg.yuexingan06.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ak.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://hu.haigaiapp.cn

Java: s.substring(1, 4)
来源：http://au.hnjuh.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ue.chemitech.net.cn

Ruby: s[1, 3];  s[1..3]
来源：http://hc.yuntaijiaju.cn

C#:   s.Substring(1, 3)
来源：http://bt.muxihuayi.cn

[E04] 查找子串位置
来源：http://im.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://vr.shtwfgs.cn

PHP:  strpos($s, "x");
来源：http://zm.newstarts.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ai.gzmigu.cn

TS:   s.indexOf("x")
来源：http://ng.shtwfgs.cn

Java: s.indexOf("x")
来源：http://mz.9csxet.cn

Go:   strings.Index(s, "x")
来源：http://di.521024.cn

Ruby: s.index("x")
来源：http://bi.szxytkj.cn

C#:   s.IndexOf("x")
来源：http://kb.szxytkj.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ax.shtwfgs.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://bx.nszjky.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wb.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rt.lnxyls.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://xz.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zo.asd995.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://pw.huixiangedu.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rc.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://va.asd995.cn

[E06] 替换子串
来源：http://du.szxytkj.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://sz.haigaiapp.cn

PHP:  str_replace("a", "b", $s);
来源：http://cd.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ov.bookmarksfly.cn

TS:   s.replaceAll("a", "b")
来源：http://ke.jianghongdianzi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uq.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yx.bjjhwx.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ps.521024.cn

C#:   s.Replace("a", "b")
来源：http://py.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://bi.bjjhwx.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://sy.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://nw.9csxet.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://im.lnxyls.cn

TS:   s.split(",")
来源：http://ot.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cr.jctech888.com.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://bh.yuntaijiaju.cn

Ruby: s.split(",");  s.split
来源：http://kt.newstarts.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tw.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://ay.bookmarksfly.cn

Py:   ",".join(items)
来源：http://qz.huixiangedu.cn

PHP:  implode(",", $items);
来源：http://yn.bjjhwx.cn

JS:   items.join(",")
来源：http://hz.huixinmuqiang.cn

TS:   items.join(",")
来源：http://tn.521024.cn

Java: String.join(",", items)
来源：http://as.nszjky.cn

Go:   strings.Join(items, ",")
来源：http://zw.shtwfgs.cn

Ruby: items.join(",")
来源：http://es.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://ao.nszjky.cn

[E09] 去除所有空白字符
来源：http://by.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ko.szsharing.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ua.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://mb.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://vr.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://ti.muxihuayi.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://he.9csxet.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ma.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://jx.shxzukj.cn

[E10] 左侧补零 / 定长填充
来源：http://cm.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bs.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://vv.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://om.wgjwhj.cn

TS:   "7".padStart(3, "0")
来源：http://ds.wgjwhj.cn

Java: String.format("%03d", 7)
来源：http://iz.gzmigu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vt.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://we.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://of.haigaiapp.cn

[E11] 反转字符串
来源：http://fs.bookmarksfly.cn

Py:   s[::-1]
来源：http://wt.newstarts.cn

PHP:  strrev($s);
来源：http://ro.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://dh.shxzskj.cn

TS:   [...s].reverse().join("")
来源：http://hy.yuntaijiaju.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sz.huixinmuqiang.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://vc.shtwfgs.cn

Ruby: s.reverse
来源：http://nw.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yu.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://rk.wgjwhj.cn

Py:   s.count("a")
来源：http://ha.gzmigu.cn

PHP:  substr_count($s, "a");
来源：http://lp.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://gq.521024.cn

TS:   s.split("a").length - 1
来源：http://xr.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wk.521024.cn

Go:   strings.Count(s, "a")
来源：http://wo.shxzukj.cn

Ruby: s.count("a")
来源：http://ed.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://sy.521024.cn

[E13] 逐字符遍历
来源：http://eq.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://dy.muxihuayi.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://lc.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fh.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ig.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ws.jianghongdianzi.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://jp.hnjuh.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fb.haigaiapp.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kn.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://zt.jianghongdianzi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pc.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://iv.haigaiapp.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://dg.szxytkj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sb.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://bq.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rj.shtwfgs.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://su.9csxet.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nb.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://il.bookmarksfly.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fh.hnjuh.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://sy.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fu.hahajie.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kv.muxihuayi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://br.gzmigu.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ky.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sx.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ca.haigaiapp.cn

[E16] 数字千分位
来源：http://oq.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://rh.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://pc.nszjky.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gp.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://su.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tt.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://tb.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://az.szsharing.cn

C#:   1234567.ToString("N0")
来源：http://cm.shxzukj.cn

[E17] 首字母大写
来源：http://yr.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://jq.shtwfgs.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yi.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lw.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tq.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ws.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://om.nicolike.cn

Ruby: s.capitalize
来源：http://ia.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sb.9csxet.cn

[E18] 模板占位符替换
来源：http://uw.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://sd.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cj.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://rs.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://on.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xp.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://nn.jianghongdianzi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://gp.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://im.yuexingan06.cn

[E19] 多行文本按行拆分
来源：http://et.shtwfgs.cn

Py:   s.splitlines()
来源：http://zt.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://oe.muxihuayi.cn

JS:   s.split(/\r?\n/)
来源：http://jf.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://dd.colortex.cn

Java: s.lines().toList()
来源：http://ii.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://jq.yuexingan06.cn

Ruby: s.lines
来源：http://qs.szsharing.cn

C#:   s.Split('\n')
来源：http://de.huixinmuqiang.cn

[E20] 判断字符串是否为空
来源：http://mx.gzmigu.cn

Py:   if not s:
来源：http://ic.shxzskj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kr.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://px.panjiajie.cn

TS:   if (s === "") {}
来源：http://ww.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://hn.panjiajie.cn

Go:   if s == "" {}
来源：http://hf.bookmarksfly.cn

Ruby: if s.empty?
来源：http://lm.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://sy.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://er.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://md.szsharing.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ou.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sw.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ww.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://iu.nszjky.cn

Go:   // 按 rune 判断长度后截断
来源：http://gl.panjiajie.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dd.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gx.shxzskj.cn

[E22] 字节长度与字符长度
来源：http://bc.gzmigu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pj.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ib.wgjwhj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wn.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://dw.jctech888.com.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ld.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xw.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://fe.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://dn.521024.cn

================================================================================
来源：http://mg.huanxung.cn

F. 文件与目录
来源：http://lo.asd995.cn

================================================================================
来源：http://gv.shxzskj.cn

[F01] 读取整个文件
来源：http://im.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tf.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://bm.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yv.bookmarksfly.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://zt.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fr.nszjky.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://su.huixinmuqiang.cn

Ruby: File.read("a.txt")
来源：http://eq.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://se.muxihuayi.cn

[F02] 逐行读取文件
来源：http://kp.panjiajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gi.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://oc.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dx.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ak.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zp.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xo.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xt.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vz.huanxung.cn

[F03] 写入文件（覆盖）
来源：http://iu.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://kt.wgjwhj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ud.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fr.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sk.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vv.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wi.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://zl.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vf.shtwfgs.cn

[F04] 追加写入文件
来源：http://un.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jr.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://tb.lnxyls.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pp.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tr.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pi.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://kc.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eq.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nv.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://sh.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://io.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://lf.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://uc.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://dq.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dj.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gy.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://ay.bjjhwx.cn

C#:   File.Exists("a.txt")
来源：http://wr.shtwfgs.cn

[F06] 删除文件
来源：http://sg.asd995.cn

Py:   os.remove("a.txt")
来源：http://gj.colortex.cn

PHP:  unlink("a.txt");
来源：http://yo.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qr.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zm.lnxyls.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cr.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://rs.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://xn.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://hc.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://rv.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://id.jctech888.com.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sx.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ld.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bu.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://aj.yuntaijiaju.cn


<!-- 参考信息 -->