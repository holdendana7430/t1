代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://ie.wgjwhj.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zi.bookmarksfly.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wp.huixinmuqiang.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://yg.yuexingan06.cn

[E02] 重复字符串
来源：http://pg.shxzskj.cn

Py:   "ab" * 3
来源：http://ln.521024.cn

PHP:  str_repeat("ab", 3);
来源：http://no.shtwfgs.cn

JS:   "ab".repeat(3)
来源：http://dn.nicolike.cn

TS:   "ab".repeat(3)
来源：http://iy.muxihuayi.cn

Java: "ab".repeat(3)
来源：http://ep.shxzskj.cn

Go:   strings.Repeat("ab", 3)
来源：http://nu.huanxung.cn

Ruby: "ab" * 3
来源：http://yb.haigaiapp.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://po.9csxet.cn

[E03] 截取子串
来源：http://oi.yuexingan06.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://vs.jianghongdianzi.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ac.newstarts.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ha.521024.cn

TS:   s.slice(1, 4)
来源：http://ay.lnxyls.cn

Java: s.substring(1, 4)
来源：http://eb.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://pt.szsharing.cn

Ruby: s[1, 3];  s[1..3]
来源：http://fj.nszjky.cn

C#:   s.Substring(1, 3)
来源：http://gu.lnxyls.cn

[E04] 查找子串位置
来源：http://rp.shxzskj.cn

Py:   s.find("x");  s.index("x")
来源：http://uc.hnjuh.cn

PHP:  strpos($s, "x");
来源：http://wt.chemitech.net.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://fz.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ix.hnjuh.cn

Java: s.indexOf("x")
来源：http://mz.asd995.cn

Go:   strings.Index(s, "x")
来源：http://hn.jctech888.com.cn

Ruby: s.index("x")
来源：http://kg.haigaiapp.cn

C#:   s.IndexOf("x")
来源：http://zr.huixinmuqiang.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://rd.nszjky.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://xm.jianghongdianzi.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://zf.haigaiapp.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://fc.haigaiapp.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bu.chemitech.net.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bf.panjiajie.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ne.hnjuh.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ie.shxzukj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://fg.haigaiapp.cn

[E06] 替换子串
来源：http://fz.huixiangedu.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://rn.nszjky.cn

PHP:  str_replace("a", "b", $s);
来源：http://ms.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ij.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://gc.wgjwhj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://na.szxytkj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ww.nicolike.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://bw.shtwfgs.cn

C#:   s.Replace("a", "b")
来源：http://zu.521024.cn

[E07] 按分隔符拆分
来源：http://lb.szxytkj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gi.shxzskj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sn.bjjhwx.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yi.nszjky.cn

TS:   s.split(",")
来源：http://nf.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dn.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://qf.521024.cn

Ruby: s.split(",");  s.split
来源：http://au.nicolike.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://qk.hnjuh.cn

[E08] 数组按分隔符合并
来源：http://se.bjjhwx.cn

Py:   ",".join(items)
来源：http://xc.muxihuayi.cn

PHP:  implode(",", $items);
来源：http://kk.wgjwhj.cn

JS:   items.join(",")
来源：http://up.9csxet.cn

TS:   items.join(",")
来源：http://rr.lnxyls.cn

Java: String.join(",", items)
来源：http://yu.521024.cn

Go:   strings.Join(items, ",")
来源：http://xa.colortex.cn

Ruby: items.join(",")
来源：http://js.szsharing.cn

C#:   string.Join(",", items)
来源：http://xy.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://qo.521024.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://aq.gzmigu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://zu.nszjky.cn

JS:   s.replace(/\s+/g, "")
来源：http://au.bookmarksfly.cn

TS:   s.replace(/\s+/g, "")
来源：http://ur.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://of.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://qw.bookmarksfly.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rp.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://kf.huanxung.cn

[E10] 左侧补零 / 定长填充
来源：http://ab.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://la.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ko.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://qn.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://yv.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://bj.lnxyls.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ch.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ru.haigaiapp.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://sj.bjjhwx.cn

[E11] 反转字符串
来源：http://wd.muxihuayi.cn

Py:   s[::-1]
来源：http://ay.bjjhwx.cn

PHP:  strrev($s);
来源：http://jh.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://nv.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://qe.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pl.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ii.yuexingan06.cn

Ruby: s.reverse
来源：http://rh.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ir.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://kp.muxihuayi.cn

Py:   s.count("a")
来源：http://ce.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://yb.lnxyls.cn

JS:   s.split("a").length - 1
来源：http://nz.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://up.yuexingan06.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xd.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://oc.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://pf.lnxyls.cn

C#:   s.Count(c => c == 'a')
来源：http://de.panjiajie.cn

[E13] 逐字符遍历
来源：http://ko.nszjky.cn

Py:   for ch in s: print(ch)
来源：http://rt.lnxyls.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cb.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://yf.nicolike.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bx.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://un.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mx.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tn.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ei.nszjky.cn

[E14] URL 编码与 Base64
来源：http://er.bookmarksfly.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hg.bookmarksfly.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://wa.yuexingan06.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kg.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://qn.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://vn.colortex.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ri.huanxung.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ui.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://al.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://mo.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://ye.szxytkj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ha.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://nl.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://au.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tg.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ix.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://pa.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wg.521024.cn

[E16] 数字千分位
来源：http://le.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://ou.hahajie.cn

PHP:  number_format(1234567);
来源：http://em.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ep.jctech888.com.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ng.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qi.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://pr.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oe.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://na.chemitech.net.cn

[E17] 首字母大写
来源：http://pn.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sm.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lp.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wd.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ej.hahajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://il.gzmigu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bz.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://oy.szxytkj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ce.muxihuayi.cn

[E18] 模板占位符替换
来源：http://yo.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hr.nszjky.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cx.panjiajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://si.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://dt.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://md.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://kr.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yb.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://bd.szsharing.cn

[E19] 多行文本按行拆分
来源：http://wv.lnxyls.cn

Py:   s.splitlines()
来源：http://tw.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xp.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://si.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://xg.chemitech.net.cn

Java: s.lines().toList()
来源：http://yh.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://dz.colortex.cn

Ruby: s.lines
来源：http://ff.asd995.cn

C#:   s.Split('\n')
来源：http://rs.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://ai.szsharing.cn

Py:   if not s:
来源：http://gk.hahajie.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://bj.wgjwhj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://um.huanxung.cn

TS:   if (s === "") {}
来源：http://qb.hnjuh.cn

Java: if (s.isEmpty()) {}
来源：http://ey.huixinmuqiang.cn

Go:   if s == "" {}
来源：http://lz.hnjuh.cn

Ruby: if s.empty?
来源：http://kh.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cr.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://uj.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://um.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bn.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pd.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wd.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hd.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://jv.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://iz.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ei.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://sf.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zm.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gh.shtwfgs.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sp.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://cy.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ql.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://lz.yuntaijiaju.cn

Ruby: s.bytesize;  s.length
来源：http://co.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://us.szsharing.cn

================================================================================
来源：http://dv.hnjuh.cn

F. 文件与目录
来源：http://qu.nicolike.cn

================================================================================
来源：http://mg.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://td.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mv.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://at.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pu.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pg.shxzukj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qz.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pw.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://qt.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://qi.hahajie.cn

[F02] 逐行读取文件
来源：http://cw.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yp.yuexingan06.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mg.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bf.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://co.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xv.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://of.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fe.wgjwhj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://al.colortex.cn

[F03] 写入文件（覆盖）
来源：http://ru.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://gk.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zm.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://io.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lc.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dh.hnjuh.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://un.521024.cn

Ruby: File.write("a.txt", "hi")
来源：http://nq.huixinmuqiang.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ot.shxzskj.cn

[F04] 追加写入文件
来源：http://oj.shtwfgs.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yj.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qn.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gp.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xc.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://om.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fa.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zt.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://et.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://tb.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wz.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://ba.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://xp.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://ld.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://bx.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oj.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://cb.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://my.muxihuayi.cn

[F06] 删除文件
来源：http://ki.newstarts.cn

Py:   os.remove("a.txt")
来源：http://pq.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://qn.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zn.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qc.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://au.huixiangedu.cn

Go:   os.Remove("a.txt")
来源：http://dx.szsharing.cn

Ruby: File.delete("a.txt")
来源：http://nx.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://dh.colortex.cn

[F07] 创建目录（含多级）
来源：http://fz.huixiangedu.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bz.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://dv.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lw.szxytkj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mf.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ad.hnjuh.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bl.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://fg.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oc.haigaiapp.cn

[F08] 遍历目录
来源：http://tu.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gt.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jx.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://xz.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://wm.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hk.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wo.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://vb.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://bq.shtwfgs.cn

[F09] 获取文件大小
来源：http://wc.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://rr.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://fc.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://pn.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://in.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zu.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uu.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://dg.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://dr.huixinmuqiang.cn

[F10] 取文件扩展名 / 文件名
来源：http://zp.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jh.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ji.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://sp.szxytkj.cn

TS:   path.extname("a.txt")
来源：http://cr.muxihuayi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ki.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gr.szsharing.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kr.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kh.hnjuh.cn

[F11] 复制与移动文件
来源：http://lu.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://sc.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bb.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jl.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oh.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lv.colortex.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://av.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rv.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ww.chemitech.net.cn

[F12] CSV 读写
来源：http://ia.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zz.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ei.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xz.hnjuh.cn

TS:   // 同上
来源：http://id.panjiajie.cn


<!-- 参考信息 -->