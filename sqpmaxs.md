代发 wailian999

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://vs.yuexingan06.cn

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://gn.nszjky.cn

Ruby: "a" + "b";  ["a", "b"].join
来源：http://bv.panjiajie.cn

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://sp.yuexingan06.cn

[E02] 重复字符串
来源：http://cl.szxytkj.cn

Py:   "ab" * 3
来源：http://wl.yuexingan06.cn

PHP:  str_repeat("ab", 3);
来源：http://tm.szsharing.cn

JS:   "ab".repeat(3)
来源：http://ce.9csxet.cn

TS:   "ab".repeat(3)
来源：http://ql.lnxyls.cn

Java: "ab".repeat(3)
来源：http://wg.jctech888.com.cn

Go:   strings.Repeat("ab", 3)
来源：http://gu.bookmarksfly.cn

Ruby: "ab" * 3
来源：http://nc.yuexingan06.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://ya.bjjhwx.cn

[E03] 截取子串
来源：http://yi.panjiajie.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ep.yuntaijiaju.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qu.shxzukj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fe.huanxung.cn

TS:   s.slice(1, 4)
来源：http://lx.huanxung.cn

Java: s.substring(1, 4)
来源：http://fl.521024.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://eq.haigaiapp.cn

Ruby: s[1, 3];  s[1..3]
来源：http://zb.szxytkj.cn

C#:   s.Substring(1, 3)
来源：http://da.521024.cn

[E04] 查找子串位置
来源：http://cy.haigaiapp.cn

Py:   s.find("x");  s.index("x")
来源：http://jb.yuntaijiaju.cn

PHP:  strpos($s, "x");
来源：http://oh.bookmarksfly.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://vv.yuexingan06.cn

TS:   s.indexOf("x")
来源：http://am.shxzukj.cn

Java: s.indexOf("x")
来源：http://hp.shxzukj.cn

Go:   strings.Index(s, "x")
来源：http://uz.shtwfgs.cn

Ruby: s.index("x")
来源：http://va.muxihuayi.cn

C#:   s.IndexOf("x")
来源：http://eh.szsharing.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://bw.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://oa.yuexingan06.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jf.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rx.huixiangedu.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://ep.szsharing.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://vr.hnjuh.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wg.jianghongdianzi.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://gu.panjiajie.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wg.yuntaijiaju.cn

[E06] 替换子串
来源：http://iy.bjjhwx.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://so.huixinmuqiang.cn

PHP:  str_replace("a", "b", $s);
来源：http://ge.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yn.shtwfgs.cn

TS:   s.replaceAll("a", "b")
来源：http://ed.panjiajie.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://zu.hnjuh.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sg.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ic.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://xe.hahajie.cn

[E07] 按分隔符拆分
来源：http://ht.chemitech.net.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://kb.jianghongdianzi.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://yp.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://hh.huanxung.cn

TS:   s.split(",")
来源：http://ro.bjjhwx.cn

Java: s.split(",");  s.split("\\s+")
来源：http://dk.nszjky.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wr.huanxung.cn

Ruby: s.split(",");  s.split
来源：http://lc.bookmarksfly.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://zn.muxihuayi.cn

[E08] 数组按分隔符合并
来源：http://rz.haigaiapp.cn

Py:   ",".join(items)
来源：http://qa.yuntaijiaju.cn

PHP:  implode(",", $items);
来源：http://eb.szxytkj.cn

JS:   items.join(",")
来源：http://hh.hahajie.cn

TS:   items.join(",")
来源：http://pw.hahajie.cn

Java: String.join(",", items)
来源：http://fq.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://cw.panjiajie.cn

Ruby: items.join(",")
来源：http://po.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://ur.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://lt.asd995.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ji.shxzskj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bb.yuntaijiaju.cn

JS:   s.replace(/\s+/g, "")
来源：http://la.hnjuh.cn

TS:   s.replace(/\s+/g, "")
来源：http://is.muxihuayi.cn

Java: s.replaceAll("\\s+", "")
来源：http://mz.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://kl.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rj.shxzskj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.jctech888.com.cn

[E10] 左侧补零 / 定长填充
来源：http://dp.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ev.shtwfgs.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://yx.jctech888.com.cn

JS:   "7".padStart(3, "0")
来源：http://vv.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://bp.shtwfgs.cn

Java: String.format("%03d", 7)
来源：http://fw.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hv.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lk.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yk.9csxet.cn

[E11] 反转字符串
来源：http://gm.bookmarksfly.cn

Py:   s[::-1]
来源：http://uq.521024.cn

PHP:  strrev($s);
来源：http://ko.521024.cn

JS:   [...s].reverse().join("")
来源：http://oi.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://oy.wgjwhj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://fg.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ox.jctech888.com.cn

Ruby: s.reverse
来源：http://ac.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xd.yuntaijiaju.cn

[E12] 统计某字符出现次数
来源：http://jn.lnxyls.cn

Py:   s.count("a")
来源：http://nu.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://jt.panjiajie.cn

JS:   s.split("a").length - 1
来源：http://vz.hnjuh.cn

TS:   s.split("a").length - 1
来源：http://xm.hahajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://vj.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://dv.colortex.cn

Ruby: s.count("a")
来源：http://qr.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://up.chemitech.net.cn

[E13] 逐字符遍历
来源：http://wx.hnjuh.cn

Py:   for ch in s: print(ch)
来源：http://oe.bookmarksfly.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://cy.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://li.yuexingan06.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://mh.hahajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://db.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ez.bjjhwx.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://yp.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://uv.wgjwhj.cn

[E14] URL 编码与 Base64
来源：http://hz.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://lb.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://lr.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://io.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fb.bookmarksfly.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ou.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ho.asd995.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://es.szxytkj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://zs.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://hi.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://li.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://bx.yuexingan06.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://dl.wgjwhj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://rs.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oy.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gz.hahajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://uq.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ce.muxihuayi.cn

[E16] 数字千分位
来源：http://mm.9csxet.cn

Py:   f"{1234567:,}"
来源：http://uk.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://bl.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://po.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://wg.jianghongdianzi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ar.shxzskj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fl.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ld.shxzukj.cn

C#:   1234567.ToString("N0")
来源：http://us.9csxet.cn

[E17] 首字母大写
来源：http://jw.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://se.wgjwhj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jv.bjjhwx.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://rr.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kf.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ok.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://af.bjjhwx.cn

Ruby: s.capitalize
来源：http://tg.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vg.newstarts.cn

[E18] 模板占位符替换
来源：http://wk.hnjuh.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oh.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qs.hahajie.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qy.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://be.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://li.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dz.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ym.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://if.nicolike.cn

[E19] 多行文本按行拆分
来源：http://gj.haigaiapp.cn

Py:   s.splitlines()
来源：http://zr.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zt.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://yp.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://eq.szsharing.cn

Java: s.lines().toList()
来源：http://ca.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://nn.jianghongdianzi.cn

Ruby: s.lines
来源：http://fx.chemitech.net.cn

C#:   s.Split('\n')
来源：http://om.newstarts.cn

[E20] 判断字符串是否为空
来源：http://xr.newstarts.cn

Py:   if not s:
来源：http://ca.asd995.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ju.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vx.hnjuh.cn

TS:   if (s === "") {}
来源：http://tz.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://ai.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://eq.newstarts.cn

Ruby: if s.empty?
来源：http://ak.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ps.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://nx.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wl.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pq.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zl.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xp.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fb.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://gj.hnjuh.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jj.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ro.szsharing.cn

[E22] 字节长度与字符长度
来源：http://cy.hnjuh.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sb.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sl.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xy.hnjuh.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://le.haigaiapp.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wd.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oc.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://qu.szxytkj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ys.muxihuayi.cn

================================================================================
来源：http://pp.9csxet.cn

F. 文件与目录
来源：http://wg.huixiangedu.cn

================================================================================
来源：http://nn.nszjky.cn

[F01] 读取整个文件
来源：http://og.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lk.jctech888.com.cn

PHP:  file_get_contents("a.txt");
来源：http://oc.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ln.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ac.nszjky.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ve.shtwfgs.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bf.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://gi.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://hw.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://ap.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sb.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ka.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oi.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fm.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cv.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mm.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rp.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://nx.hnjuh.cn

[F03] 写入文件（覆盖）
来源：http://xc.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hl.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tw.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wg.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xp.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yg.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://kw.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://np.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hf.nszjky.cn

[F04] 追加写入文件
来源：http://io.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://px.jctech888.com.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zv.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://or.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://na.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wa.shxzskj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ij.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://gg.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jw.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://yf.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nf.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://ll.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://vn.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://gj.hahajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hp.szsharing.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://pf.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://av.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://li.yuntaijiaju.cn

[F06] 删除文件
来源：http://rz.asd995.cn

Py:   os.remove("a.txt")
来源：http://wh.yuexingan06.cn

PHP:  unlink("a.txt");
来源：http://jk.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://el.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://te.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sj.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://qn.szxytkj.cn

Ruby: File.delete("a.txt")
来源：http://yl.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://nf.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://xk.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ut.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://za.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kr.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gk.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ax.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hu.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wp.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uw.huixinmuqiang.cn

[F08] 遍历目录
来源：http://ve.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://aj.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bx.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://zd.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://ux.521024.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://su.bjjhwx.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://kf.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://fw.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://zx.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://nd.bookmarksfly.cn

Py:   os.path.getsize("a.txt")
来源：http://eo.lnxyls.cn

PHP:  filesize("a.txt");
来源：http://bq.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://up.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://qa.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://mv.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ui.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://za.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://fj.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://ap.shtwfgs.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bk.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://eh.nszjky.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gl.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://kn.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://he.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sf.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yn.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rt.asd995.cn

[F11] 复制与移动文件
来源：http://jt.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://cs.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jh.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ub.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://uv.newstarts.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yb.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lt.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://db.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://oy.gzmigu.cn

[F12] CSV 读写
来源：http://ah.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kl.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mh.huixiangedu.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://eh.huixinmuqiang.cn

TS:   // 同上
来源：http://xb.jianghongdianzi.cn


<!-- 参考信息 -->