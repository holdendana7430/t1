代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://fb.gzmigu.cn

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://ph.hnjuh.cn

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://jl.shxzskj.cn

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://bo.9csxet.cn

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://io.521024.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://aw.lnxyls.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://rn.nicolike.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://si.asd995.cn

[E02] 重复字符串
来源：http://ty.521024.cn

Py:   "ab" * 3
来源：http://at.bookmarksfly.cn

PHP:  str_repeat("ab", 3);
来源：http://cp.szxytkj.cn

JS:   "ab".repeat(3)
来源：http://yh.asd995.cn

TS:   "ab".repeat(3)
来源：http://yo.newstarts.cn

Java: "ab".repeat(3)
来源：http://zo.newstarts.cn

Go:   strings.Repeat("ab", 3)
来源：http://rz.wgjwhj.cn

Ruby: "ab" * 3
来源：http://et.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://kg.colortex.cn

[E03] 截取子串
来源：http://jb.muxihuayi.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://nf.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hg.9csxet.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://pr.muxihuayi.cn

TS:   s.slice(1, 4)
来源：http://xd.szxytkj.cn

Java: s.substring(1, 4)
来源：http://yo.asd995.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://uu.jianghongdianzi.cn

Ruby: s[1, 3];  s[1..3]
来源：http://kp.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://oj.jctech888.com.cn

[E04] 查找子串位置
来源：http://ir.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://pc.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://uf.521024.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yj.chemitech.net.cn

TS:   s.indexOf("x")
来源：http://ig.shxzskj.cn

Java: s.indexOf("x")
来源：http://sk.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://sp.szsharing.cn

Ruby: s.index("x")
来源：http://se.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://yp.nszjky.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://ei.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dn.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hc.jianghongdianzi.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zs.jctech888.com.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://bb.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://sz.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wl.newstarts.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hb.newstarts.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://le.wgjwhj.cn

[E06] 替换子串
来源：http://nd.muxihuayi.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vg.wgjwhj.cn

PHP:  str_replace("a", "b", $s);
来源：http://mb.muxihuayi.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://px.shxzskj.cn

TS:   s.replaceAll("a", "b")
来源：http://ka.jctech888.com.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://rf.panjiajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zs.521024.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nd.huixinmuqiang.cn

C#:   s.Replace("a", "b")
来源：http://bo.wgjwhj.cn

[E07] 按分隔符拆分
来源：http://li.shxzskj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pa.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://sa.huixiangedu.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://bf.yuntaijiaju.cn

TS:   s.split(",")
来源：http://jh.huixiangedu.cn

Java: s.split(",");  s.split("\\s+")
来源：http://oy.panjiajie.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gd.chemitech.net.cn

Ruby: s.split(",");  s.split
来源：http://vq.huixiangedu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wd.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://hz.shxzskj.cn

Py:   ",".join(items)
来源：http://qb.colortex.cn

PHP:  implode(",", $items);
来源：http://nq.yuexingan06.cn

JS:   items.join(",")
来源：http://fb.shxzukj.cn

TS:   items.join(",")
来源：http://mg.panjiajie.cn

Java: String.join(",", items)
来源：http://oo.nicolike.cn

Go:   strings.Join(items, ",")
来源：http://sc.gzmigu.cn

Ruby: items.join(",")
来源：http://cx.lnxyls.cn

C#:   string.Join(",", items)
来源：http://zz.gzmigu.cn

[E09] 去除所有空白字符
来源：http://ow.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ww.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://dh.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ne.lnxyls.cn

TS:   s.replace(/\s+/g, "")
来源：http://lz.nicolike.cn

Java: s.replaceAll("\\s+", "")
来源：http://lu.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gq.gzmigu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://uf.yuexingan06.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mi.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://vh.yuntaijiaju.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://fi.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bf.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://dp.haigaiapp.cn

TS:   "7".padStart(3, "0")
来源：http://iy.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://ln.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://po.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wd.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zh.huixiangedu.cn

[E11] 反转字符串
来源：http://il.szsharing.cn

Py:   s[::-1]
来源：http://lz.newstarts.cn

PHP:  strrev($s);
来源：http://em.asd995.cn

JS:   [...s].reverse().join("")
来源：http://lz.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://ay.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ss.huixiangedu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://tr.9csxet.cn

Ruby: s.reverse
来源：http://sy.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://an.nicolike.cn

[E12] 统计某字符出现次数
来源：http://uj.hnjuh.cn

Py:   s.count("a")
来源：http://qg.yuexingan06.cn

PHP:  substr_count($s, "a");
来源：http://qi.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://vv.wgjwhj.cn

TS:   s.split("a").length - 1
来源：http://qt.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://al.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://rb.shxzskj.cn

Ruby: s.count("a")
来源：http://aq.gzmigu.cn

C#:   s.Count(c => c == 'a')
来源：http://cv.shxzskj.cn

[E13] 逐字符遍历
来源：http://at.haigaiapp.cn

Py:   for ch in s: print(ch)
来源：http://bc.szxytkj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://fj.asd995.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ah.huixiangedu.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://xq.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://rg.colortex.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wt.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yr.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hu.huanxung.cn

[E14] URL 编码与 Base64
来源：http://ie.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://an.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ee.521024.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xi.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bd.szxytkj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://tx.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ad.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gk.huanxung.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pe.yuntaijiaju.cn

[E15] HTML 转义 / 反转义
来源：http://lm.newstarts.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jp.jctech888.com.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wd.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://gu.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://up.szxytkj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ll.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cr.nicolike.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sv.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://am.hahajie.cn

[E16] 数字千分位
来源：http://vg.asd995.cn

Py:   f"{1234567:,}"
来源：http://cx.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://lq.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://md.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://dn.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://pw.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ly.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://jf.gzmigu.cn

C#:   1234567.ToString("N0")
来源：http://dc.szsharing.cn

[E17] 首字母大写
来源：http://gm.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mo.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xp.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yy.huanxung.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lj.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ev.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ld.nszjky.cn

Ruby: s.capitalize
来源：http://hy.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wh.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://zd.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tg.hahajie.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://xe.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dg.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://og.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ac.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://xv.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://fh.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://em.muxihuayi.cn

[E19] 多行文本按行拆分
来源：http://of.haigaiapp.cn

Py:   s.splitlines()
来源：http://bb.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qu.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://ag.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://ls.yuntaijiaju.cn

Java: s.lines().toList()
来源：http://kf.nicolike.cn

Go:   strings.Split(s, "\n")
来源：http://js.wgjwhj.cn

Ruby: s.lines
来源：http://oy.szxytkj.cn

C#:   s.Split('\n')
来源：http://gp.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://xe.haigaiapp.cn

Py:   if not s:
来源：http://ab.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://si.9csxet.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ht.shxzskj.cn

TS:   if (s === "") {}
来源：http://mh.chemitech.net.cn

Java: if (s.isEmpty()) {}
来源：http://tz.huixiangedu.cn

Go:   if s == "" {}
来源：http://lc.hnjuh.cn

Ruby: if s.empty?
来源：http://zp.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://pv.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://vn.nszjky.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ah.huixinmuqiang.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uc.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://um.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ox.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ib.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://ib.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qd.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sn.yuntaijiaju.cn

[E22] 字节长度与字符长度
来源：http://ez.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ay.521024.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://kw.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zr.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://jf.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://tt.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ni.bjjhwx.cn

Ruby: s.bytesize;  s.length
来源：http://lr.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fw.chemitech.net.cn

================================================================================
来源：http://hw.huixiangedu.cn

F. 文件与目录
来源：http://pt.chemitech.net.cn

================================================================================
来源：http://kj.bjjhwx.cn

[F01] 读取整个文件
来源：http://bv.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ed.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://qt.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://lz.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ws.jctech888.com.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://up.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://iq.hnjuh.cn

Ruby: File.read("a.txt")
来源：http://nj.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://vl.shxzskj.cn

[F02] 逐行读取文件
来源：http://th.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yb.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vy.bookmarksfly.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ig.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fd.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://un.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xf.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://tt.shtwfgs.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://iy.nicolike.cn

[F03] 写入文件（覆盖）
来源：http://ng.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ev.nszjky.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://mo.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yt.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xo.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dh.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fa.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://wg.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://bl.bjjhwx.cn

[F04] 追加写入文件
来源：http://kp.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fb.wgjwhj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://fu.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://fs.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ft.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nk.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sn.yuntaijiaju.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ps.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://es.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://sn.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yh.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://gf.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://ih.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://xe.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://or.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tw.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://nz.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://mn.bjjhwx.cn

[F06] 删除文件
来源：http://wl.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://dg.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://td.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ud.panjiajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://az.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://we.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://zd.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://hp.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://ey.521024.cn

[F07] 创建目录（含多级）
来源：http://ef.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jv.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nr.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bj.jctech888.com.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tj.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yi.chemitech.net.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ns.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://at.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://js.muxihuayi.cn

[F08] 遍历目录
来源：http://wg.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mn.yuexingan06.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bn.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://py.lnxyls.cn

TS:   fs.readdirSync("dir")
来源：http://ie.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://do.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://al.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://pc.yuntaijiaju.cn

C#:   Directory.GetFiles("dir")
来源：http://rn.jctech888.com.cn

[F09] 获取文件大小
来源：http://cp.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://dk.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://yc.huixinmuqiang.cn

JS:   fs.statSync("a.txt").size
来源：http://am.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://fq.shtwfgs.cn

Java: Files.size(Path.of("a.txt"))
来源：http://us.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hx.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://vc.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://xm.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://fb.haigaiapp.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gh.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://kf.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ag.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://oe.chemitech.net.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jo.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sj.nszjky.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cd.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://kx.szxytkj.cn

[F11] 复制与移动文件
来源：http://of.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xt.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gw.jianghongdianzi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bv.hahajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://he.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rs.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eg.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fm.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hu.bjjhwx.cn

[F12] CSV 读写
来源：http://me.colortex.cn


<!-- 参考信息 -->