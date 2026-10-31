代发 wailian999

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://ho.gzmigu.cn

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wq.shxzskj.cn

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://qe.nicolike.cn

[D26] 数组转字符串
来源：http://jl.haigaiapp.cn

Py:   ", ".join(map(str, arr))
来源：http://zc.shxzukj.cn

PHP:  implode(", ", $arr);
来源：http://uf.huanxung.cn

JS:   arr.join(", ")
来源：http://hm.hnjuh.cn

TS:   arr.join(", ")
来源：http://fg.muxihuayi.cn

Java: String.join(", ", list)
来源：http://an.gzmigu.cn

Go:   strings.Join(strs, ", ")
来源：http://cy.newstarts.cn

Ruby: arr.join(", ")
来源：http://qu.asd995.cn

C#:   string.Join(", ", list)
来源：http://qa.huixinmuqiang.cn

================================================================================
来源：http://br.gzmigu.cn

E. 字符串处理
来源：http://op.9csxet.cn

================================================================================
来源：http://ko.chemitech.net.cn

[E01] 拼接字符串
来源：http://tm.jctech888.com.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://xj.chemitech.net.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://po.haigaiapp.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://im.wgjwhj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://le.chemitech.net.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://cl.huixinmuqiang.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://uv.muxihuayi.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://ej.shxzukj.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ef.huanxung.cn

[E02] 重复字符串
来源：http://oa.shxzskj.cn

Py:   "ab" * 3
来源：http://fu.9csxet.cn

PHP:  str_repeat("ab", 3);
来源：http://fv.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://ue.nicolike.cn

TS:   "ab".repeat(3)
来源：http://oy.huixinmuqiang.cn

Java: "ab".repeat(3)
来源：http://zu.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://em.asd995.cn

Ruby: "ab" * 3
来源：http://tm.nszjky.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mp.yuntaijiaju.cn

[E03] 截取子串
来源：http://ft.jianghongdianzi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://lv.huixiangedu.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hf.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://vi.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://jw.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://ih.newstarts.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hs.gzmigu.cn

Ruby: s[1, 3];  s[1..3]
来源：http://pn.bjjhwx.cn

C#:   s.Substring(1, 3)
来源：http://zt.hahajie.cn

[E04] 查找子串位置
来源：http://ji.huixinmuqiang.cn

Py:   s.find("x");  s.index("x")
来源：http://vj.jianghongdianzi.cn

PHP:  strpos($s, "x");
来源：http://uw.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://ce.newstarts.cn

TS:   s.indexOf("x")
来源：http://et.521024.cn

Java: s.indexOf("x")
来源：http://mt.jctech888.com.cn

Go:   strings.Index(s, "x")
来源：http://ln.huixiangedu.cn

Ruby: s.index("x")
来源：http://qi.newstarts.cn

C#:   s.IndexOf("x")
来源：http://su.panjiajie.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://aq.shxzukj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fp.bjjhwx.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://fs.9csxet.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ka.shxzukj.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://es.jianghongdianzi.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://kl.huixinmuqiang.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://vg.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hn.chemitech.net.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://og.yuntaijiaju.cn

[E06] 替换子串
来源：http://lu.chemitech.net.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mu.gzmigu.cn

PHP:  str_replace("a", "b", $s);
来源：http://fu.huanxung.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uo.bjjhwx.cn

TS:   s.replaceAll("a", "b")
来源：http://pr.nszjky.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zg.9csxet.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ep.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://yy.shxzukj.cn

C#:   s.Replace("a", "b")
来源：http://ap.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://rr.shtwfgs.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ry.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://du.jctech888.com.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tp.yuexingan06.cn

TS:   s.split(",")
来源：http://bp.shxzukj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hy.huixinmuqiang.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://px.szsharing.cn

Ruby: s.split(",");  s.split
来源：http://uu.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://tj.huanxung.cn

[E08] 数组按分隔符合并
来源：http://ly.colortex.cn

Py:   ",".join(items)
来源：http://bl.shxzukj.cn

PHP:  implode(",", $items);
来源：http://oo.bookmarksfly.cn

JS:   items.join(",")
来源：http://cp.lnxyls.cn

TS:   items.join(",")
来源：http://ds.yuexingan06.cn

Java: String.join(",", items)
来源：http://xa.huanxung.cn

Go:   strings.Join(items, ",")
来源：http://oi.jctech888.com.cn

Ruby: items.join(",")
来源：http://zb.szsharing.cn

C#:   string.Join(",", items)
来源：http://do.muxihuayi.cn

[E09] 去除所有空白字符
来源：http://ng.gzmigu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://dx.colortex.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xi.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://ya.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://qh.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://zt.chemitech.net.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qu.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://sm.jctech888.com.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://lt.jianghongdianzi.cn

[E10] 左侧补零 / 定长填充
来源：http://ze.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fc.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://oj.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://yr.colortex.cn

TS:   "7".padStart(3, "0")
来源：http://rz.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://kp.nicolike.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ph.wgjwhj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ec.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wx.shxzukj.cn

[E11] 反转字符串
来源：http://cs.huanxung.cn

Py:   s[::-1]
来源：http://jz.panjiajie.cn

PHP:  strrev($s);
来源：http://hn.521024.cn

JS:   [...s].reverse().join("")
来源：http://xe.asd995.cn

TS:   [...s].reverse().join("")
来源：http://rv.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ag.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://bp.bjjhwx.cn

Ruby: s.reverse
来源：http://ki.chemitech.net.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mn.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://mf.szxytkj.cn

Py:   s.count("a")
来源：http://vw.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://um.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://jm.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://hn.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gr.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://go.asd995.cn

Ruby: s.count("a")
来源：http://ru.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://sn.huixiangedu.cn

[E13] 逐字符遍历
来源：http://rb.bjjhwx.cn

Py:   for ch in s: print(ch)
来源：http://qe.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://nl.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ua.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qa.jctech888.com.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ir.yuntaijiaju.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ic.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oo.asd995.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://zv.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://jw.panjiajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://pa.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://es.szsharing.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wa.asd995.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ii.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hr.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rt.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fu.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fs.gzmigu.cn

[E15] HTML 转义 / 反转义
来源：http://rz.colortex.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oy.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ue.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bg.shtwfgs.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jx.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wq.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cs.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tb.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://sn.shxzskj.cn

[E16] 数字千分位
来源：http://gl.lnxyls.cn

Py:   f"{1234567:,}"
来源：http://cl.hahajie.cn

PHP:  number_format(1234567);
来源：http://jr.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qj.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ty.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ny.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ht.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ub.jianghongdianzi.cn

C#:   1234567.ToString("N0")
来源：http://um.haigaiapp.cn

[E17] 首字母大写
来源：http://qm.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pd.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oc.muxihuayi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nz.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ta.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sd.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tz.shxzukj.cn

Ruby: s.capitalize
来源：http://bq.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://il.newstarts.cn

[E18] 模板占位符替换
来源：http://sl.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wv.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mb.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://sp.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://pw.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hl.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lj.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://pf.hahajie.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://uq.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://mb.gzmigu.cn

Py:   s.splitlines()
来源：http://ex.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://db.9csxet.cn

JS:   s.split(/\r?\n/)
来源：http://or.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://ff.huanxung.cn

Java: s.lines().toList()
来源：http://mv.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://to.hnjuh.cn

Ruby: s.lines
来源：http://lx.hnjuh.cn

C#:   s.Split('\n')
来源：http://hj.nszjky.cn

[E20] 判断字符串是否为空
来源：http://qt.huixinmuqiang.cn

Py:   if not s:
来源：http://bh.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ub.huanxung.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ur.panjiajie.cn

TS:   if (s === "") {}
来源：http://om.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://bp.nszjky.cn

Go:   if s == "" {}
来源：http://qf.colortex.cn

Ruby: if s.empty?
来源：http://ih.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://is.bookmarksfly.cn

[E21] 超长截断加省略号
来源：http://nl.521024.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://lu.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://os.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jg.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://yk.jctech888.com.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://uu.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://ys.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://po.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://qj.newstarts.cn

[E22] 字节长度与字符长度
来源：http://pd.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://td.shtwfgs.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gw.yuexingan06.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sl.bookmarksfly.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hd.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://gg.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ty.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://sa.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://nh.wgjwhj.cn

================================================================================
来源：http://hb.szsharing.cn

F. 文件与目录
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://gk.chemitech.net.cn

[F01] 读取整个文件
来源：http://mx.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tr.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://el.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vk.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://tk.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zi.jianghongdianzi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rs.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://qv.szxytkj.cn

C#:   File.ReadAllText("a.txt");
来源：http://qt.huixiangedu.cn

[F02] 逐行读取文件
来源：http://tm.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://by.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ln.nicolike.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xg.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oo.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://uy.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fi.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zw.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://it.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://lm.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sx.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mk.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ng.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vn.muxihuayi.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kx.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://qi.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ry.9csxet.cn

[F04] 追加写入文件
来源：http://hk.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gj.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vq.gzmigu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jw.haigaiapp.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zr.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ah.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vj.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://yh.nicolike.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ek.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://re.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ff.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://nb.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://im.gzmigu.cn

TS:   fs.existsSync("a.txt")
来源：http://gm.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sk.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ol.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://zz.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://pg.haigaiapp.cn

[F06] 删除文件
来源：http://tl.colortex.cn

Py:   os.remove("a.txt")
来源：http://xf.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://rp.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://is.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://lm.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cx.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://wa.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://tg.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://re.colortex.cn

[F07] 创建目录（含多级）
来源：http://zf.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ms.muxihuayi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xu.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tf.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jn.521024.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xu.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sd.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wx.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fc.newstarts.cn

[F08] 遍历目录
来源：http://yo.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://py.szsharing.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ql.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://ot.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://my.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ov.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sf.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://el.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://ey.bookmarksfly.cn

[F09] 获取文件大小
来源：http://uk.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://zz.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://gw.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://tf.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://na.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bl.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fo.9csxet.cn

Ruby: File.size("a.txt")
来源：http://wg.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ko.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://xw.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mj.shxzskj.cn


<!-- 参考信息 -->