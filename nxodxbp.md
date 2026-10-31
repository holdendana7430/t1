代发 wailian999

================================================================================
来源：http://nq.bookmarksfly.cn

E. 字符串处理
来源：http://rs.9csxet.cn

================================================================================
来源：http://ck.huanxung.cn

[E01] 拼接字符串
来源：http://gi.bookmarksfly.cn

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://yd.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://un.521024.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mz.gzmigu.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://pe.huixiangedu.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://oc.jianghongdianzi.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://zn.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://vp.bookmarksfly.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://ix.huixiangedu.cn

[E02] 重复字符串
来源：http://tn.bookmarksfly.cn

Py:   "ab" * 3
来源：http://mm.shtwfgs.cn

PHP:  str_repeat("ab", 3);
来源：http://aq.bookmarksfly.cn

JS:   "ab".repeat(3)
来源：http://af.jctech888.com.cn

TS:   "ab".repeat(3)
来源：http://ns.shxzskj.cn

Java: "ab".repeat(3)
来源：http://ta.haigaiapp.cn

Go:   strings.Repeat("ab", 3)
来源：http://ql.wgjwhj.cn

Ruby: "ab" * 3
来源：http://xa.wgjwhj.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://dj.chemitech.net.cn

[E03] 截取子串
来源：http://nh.shxzukj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zk.nicolike.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://ga.chemitech.net.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ci.huixiangedu.cn

TS:   s.slice(1, 4)
来源：http://sd.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://ee.shtwfgs.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://yo.hnjuh.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uu.panjiajie.cn

C#:   s.Substring(1, 3)
来源：http://ub.newstarts.cn

[E04] 查找子串位置
来源：http://xa.szsharing.cn

Py:   s.find("x");  s.index("x")
来源：http://ur.wgjwhj.cn

PHP:  strpos($s, "x");
来源：http://ta.huixinmuqiang.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://lv.huixiangedu.cn

TS:   s.indexOf("x")
来源：http://hr.shtwfgs.cn

Java: s.indexOf("x")
来源：http://ut.lnxyls.cn

Go:   strings.Index(s, "x")
来源：http://co.asd995.cn

Ruby: s.index("x")
来源：http://fc.521024.cn

C#:   s.IndexOf("x")
来源：http://wd.jctech888.com.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://te.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://pf.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://dc.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rs.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://hw.newstarts.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vs.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://gv.asd995.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ub.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://or.newstarts.cn

[E06] 替换子串
来源：http://tj.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://pj.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://ry.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fh.huixiangedu.cn

TS:   s.replaceAll("a", "b")
来源：http://hu.bjjhwx.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ke.shtwfgs.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://gw.bookmarksfly.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://qr.521024.cn

C#:   s.Replace("a", "b")
来源：http://uz.nicolike.cn

[E07] 按分隔符拆分
来源：http://pz.gzmigu.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://gd.newstarts.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ec.szxytkj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://kb.huixiangedu.cn

TS:   s.split(",")
来源：http://me.huanxung.cn

Java: s.split(",");  s.split("\\s+")
来源：http://jr.shtwfgs.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ir.jctech888.com.cn

Ruby: s.split(",");  s.split
来源：http://tb.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wq.jctech888.com.cn

[E08] 数组按分隔符合并
来源：http://xw.shxzskj.cn

Py:   ",".join(items)
来源：http://bi.521024.cn

PHP:  implode(",", $items);
来源：http://ty.chemitech.net.cn

JS:   items.join(",")
来源：http://ew.asd995.cn

TS:   items.join(",")
来源：http://pe.lnxyls.cn

Java: String.join(",", items)
来源：http://ml.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://cv.huixinmuqiang.cn

Ruby: items.join(",")
来源：http://zq.szsharing.cn

C#:   string.Join(",", items)
来源：http://cl.521024.cn

[E09] 去除所有空白字符
来源：http://ja.nicolike.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://jh.chemitech.net.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jd.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://vt.nszjky.cn

TS:   s.replace(/\s+/g, "")
来源：http://fk.nszjky.cn

Java: s.replaceAll("\\s+", "")
来源：http://id.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dr.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ot.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ni.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://ka.9csxet.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wy.shxzukj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://rm.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://kb.hahajie.cn

TS:   "7".padStart(3, "0")
来源：http://jy.yuntaijiaju.cn

Java: String.format("%03d", 7)
来源：http://ee.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ww.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://dv.jianghongdianzi.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wr.newstarts.cn

[E11] 反转字符串
来源：http://ub.nszjky.cn

Py:   s[::-1]
来源：http://hw.gzmigu.cn

PHP:  strrev($s);
来源：http://ic.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://yu.521024.cn

TS:   [...s].reverse().join("")
来源：http://wq.nszjky.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://dh.newstarts.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ba.lnxyls.cn

Ruby: s.reverse
来源：http://aw.nicolike.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hn.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://ye.wgjwhj.cn

Py:   s.count("a")
来源：http://lr.9csxet.cn

PHP:  substr_count($s, "a");
来源：http://ba.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://vz.yuexingan06.cn

TS:   s.split("a").length - 1
来源：http://mq.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://kv.colortex.cn

Go:   strings.Count(s, "a")
来源：http://cg.nicolike.cn

Ruby: s.count("a")
来源：http://yy.jctech888.com.cn

C#:   s.Count(c => c == 'a')
来源：http://hg.jctech888.com.cn

[E13] 逐字符遍历
来源：http://wx.muxihuayi.cn

Py:   for ch in s: print(ch)
来源：http://nj.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zj.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://fx.chemitech.net.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://hj.szsharing.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://jh.jctech888.com.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zr.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cq.colortex.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wg.bookmarksfly.cn

[E14] URL 编码与 Base64
来源：http://ir.wgjwhj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qt.muxihuayi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://tz.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://fx.panjiajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mx.chemitech.net.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://be.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://om.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ov.bjjhwx.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gl.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://eq.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://xy.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ki.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ag.colortex.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yc.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bm.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ly.colortex.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://jj.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yv.colortex.cn

[E16] 数字千分位
来源：http://xc.asd995.cn

Py:   f"{1234567:,}"
来源：http://ny.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://ew.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zq.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gg.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hf.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sf.shxzskj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://aa.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://xp.colortex.cn

[E17] 首字母大写
来源：http://ue.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oj.huixiangedu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xp.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://iq.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pl.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sw.newstarts.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ya.colortex.cn

Ruby: s.capitalize
来源：http://tk.lnxyls.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sc.shxzskj.cn

[E18] 模板占位符替换
来源：http://vg.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hx.asd995.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pt.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://br.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://gn.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gs.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ga.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://uh.nicolike.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dn.szsharing.cn

[E19] 多行文本按行拆分
来源：http://dz.jianghongdianzi.cn

Py:   s.splitlines()
来源：http://qk.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ca.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://hg.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://li.szxytkj.cn

Java: s.lines().toList()
来源：http://za.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ze.shxzskj.cn

Ruby: s.lines
来源：http://th.newstarts.cn

C#:   s.Split('\n')
来源：http://gs.huixiangedu.cn

[E20] 判断字符串是否为空
来源：http://ym.muxihuayi.cn

Py:   if not s:
来源：http://ax.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ag.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mw.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://wq.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://oi.bjjhwx.cn

Go:   if s == "" {}
来源：http://kg.huixiangedu.cn

Ruby: if s.empty?
来源：http://kd.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tb.9csxet.cn

[E21] 超长截断加省略号
来源：http://kj.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qb.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://yd.hahajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tz.shxzskj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kw.szsharing.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bw.jctech888.com.cn

Go:   // 按 rune 判断长度后截断
来源：http://cy.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ja.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://oq.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://nb.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mh.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kd.newstarts.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nm.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://km.colortex.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jh.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cw.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://mo.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ln.521024.cn

================================================================================
来源：http://lu.yuntaijiaju.cn

F. 文件与目录
来源：http://lo.hnjuh.cn

================================================================================
来源：http://ro.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://an.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://jh.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://aq.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pe.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nh.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ig.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dc.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://qa.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://rm.shxzskj.cn

[F02] 逐行读取文件
来源：http://cv.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fg.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vu.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sk.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zy.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ba.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pa.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qd.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hk.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://il.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://px.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sd.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ii.newstarts.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://we.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xa.nszjky.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pu.chemitech.net.cn

Ruby: File.write("a.txt", "hi")
来源：http://oi.hnjuh.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xh.szxytkj.cn

[F04] 追加写入文件
来源：http://ks.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sw.shxzskj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wv.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://is.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://da.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wv.gzmigu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cp.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://vs.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pn.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://il.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lf.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://vx.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://xl.shxzskj.cn

TS:   fs.existsSync("a.txt")
来源：http://ca.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://db.chemitech.net.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cl.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://ir.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://ag.lnxyls.cn

[F06] 删除文件
来源：http://pf.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ej.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://kb.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ue.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ux.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://od.bjjhwx.cn

Go:   os.Remove("a.txt")
来源：http://yi.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://sr.jianghongdianzi.cn

C#:   File.Delete("a.txt");
来源：http://xt.9csxet.cn

[F07] 创建目录（含多级）
来源：http://zf.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://li.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vw.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kr.jianghongdianzi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tr.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zp.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gw.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jb.muxihuayi.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oc.gzmigu.cn

[F08] 遍历目录
来源：http://lz.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fl.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://gz.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://ye.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://qv.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rk.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://gn.nszjky.cn

Ruby: Dir.children("dir")
来源：http://jl.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://el.wgjwhj.cn

[F09] 获取文件大小
来源：http://az.hahajie.cn

Py:   os.path.getsize("a.txt")
来源：http://du.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://rs.chemitech.net.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.hnjuh.cn

TS:   fs.statSync("a.txt").size
来源：http://uy.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ew.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xe.nicolike.cn

Ruby: File.size("a.txt")
来源：http://ay.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://bh.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://fy.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://br.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cs.colortex.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://av.jianghongdianzi.cn

TS:   path.extname("a.txt")
来源：http://ax.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rb.panjiajie.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rl.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fa.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lr.jianghongdianzi.cn

[F11] 复制与移动文件
来源：http://ro.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://id.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bs.shtwfgs.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xl.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cu.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hv.hnjuh.cn


<!-- 参考信息 -->