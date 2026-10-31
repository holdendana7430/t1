代发 wailian999

[E02] 重复字符串
来源：http://lh.huixinmuqiang.cn

Py:   "ab" * 3
来源：http://nc.huixinmuqiang.cn

PHP:  str_repeat("ab", 3);
来源：http://xz.9csxet.cn

JS:   "ab".repeat(3)
来源：http://da.gzmigu.cn

TS:   "ab".repeat(3)
来源：http://ws.jctech888.com.cn

Java: "ab".repeat(3)
来源：http://iw.huanxung.cn

Go:   strings.Repeat("ab", 3)
来源：http://oh.shxzukj.cn

Ruby: "ab" * 3
来源：http://ur.shtwfgs.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://rf.yuntaijiaju.cn

[E03] 截取子串
来源：http://tf.521024.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://zr.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dc.jianghongdianzi.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://ba.lnxyls.cn

TS:   s.slice(1, 4)
来源：http://lr.yuexingan06.cn

Java: s.substring(1, 4)
来源：http://ta.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://ru.lnxyls.cn

Ruby: s[1, 3];  s[1..3]
来源：http://yx.szsharing.cn

C#:   s.Substring(1, 3)
来源：http://cr.hnjuh.cn

[E04] 查找子串位置
来源：http://xa.panjiajie.cn

Py:   s.find("x");  s.index("x")
来源：http://lu.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://sb.muxihuayi.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://as.shxzskj.cn

TS:   s.indexOf("x")
来源：http://ek.huanxung.cn

Java: s.indexOf("x")
来源：http://lo.wgjwhj.cn

Go:   strings.Index(s, "x")
来源：http://tz.szxytkj.cn

Ruby: s.index("x")
来源：http://ta.szsharing.cn

C#:   s.IndexOf("x")
来源：http://ya.newstarts.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://sb.521024.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ad.nicolike.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mt.shtwfgs.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://io.shtwfgs.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://fh.bookmarksfly.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://rm.shxzukj.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://op.wgjwhj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://rz.huanxung.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wx.shxzskj.cn

[E06] 替换子串
来源：http://kw.lnxyls.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://za.panjiajie.cn

PHP:  str_replace("a", "b", $s);
来源：http://zp.521024.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://in.jianghongdianzi.cn

TS:   s.replaceAll("a", "b")
来源：http://rz.huanxung.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://xj.jianghongdianzi.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://sb.huixiangedu.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://tt.wgjwhj.cn

C#:   s.Replace("a", "b")
来源：http://ai.gzmigu.cn

[E07] 按分隔符拆分
来源：http://of.shxzukj.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://ew.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hw.shxzskj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://iy.newstarts.cn

TS:   s.split(",")
来源：http://dc.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://bh.yuexingan06.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yw.nszjky.cn

Ruby: s.split(",");  s.split
来源：http://hw.nszjky.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lx.9csxet.cn

[E08] 数组按分隔符合并
来源：http://sr.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://lq.nicolike.cn

PHP:  implode(",", $items);
来源：http://vx.huixinmuqiang.cn

JS:   items.join(",")
来源：http://yd.jctech888.com.cn

TS:   items.join(",")
来源：http://xd.chemitech.net.cn

Java: String.join(",", items)
来源：http://wk.haigaiapp.cn

Go:   strings.Join(items, ",")
来源：http://kp.huanxung.cn

Ruby: items.join(",")
来源：http://jy.wgjwhj.cn

C#:   string.Join(",", items)
来源：http://tw.9csxet.cn

[E09] 去除所有空白字符
来源：http://xp.lnxyls.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hj.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://up.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://kw.9csxet.cn

TS:   s.replace(/\s+/g, "")
来源：http://ys.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://ob.shxzukj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://xi.hnjuh.cn

Ruby: s.gsub(/\s+/, "")
来源：http://zm.521024.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hr.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://rb.shtwfgs.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gm.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ru.wgjwhj.cn

JS:   "7".padStart(3, "0")
来源：http://ev.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://te.szxytkj.cn

Java: String.format("%03d", 7)
来源：http://ul.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://hj.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ju.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ds.521024.cn

[E11] 反转字符串
来源：http://lc.shtwfgs.cn

Py:   s[::-1]
来源：http://pg.9csxet.cn

PHP:  strrev($s);
来源：http://mb.muxihuayi.cn

JS:   [...s].reverse().join("")
来源：http://am.chemitech.net.cn

TS:   [...s].reverse().join("")
来源：http://nx.yuexingan06.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://qw.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ix.yuntaijiaju.cn

Ruby: s.reverse
来源：http://sa.colortex.cn

C#:   new string(s.Reverse().ToArray())
来源：http://de.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://cv.gzmigu.cn

Py:   s.count("a")
来源：http://dx.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://qa.nicolike.cn

JS:   s.split("a").length - 1
来源：http://yp.asd995.cn

TS:   s.split("a").length - 1
来源：http://jn.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://xp.szsharing.cn

Go:   strings.Count(s, "a")
来源：http://vb.lnxyls.cn

Ruby: s.count("a")
来源：http://sx.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://tn.bjjhwx.cn

[E13] 逐字符遍历
来源：http://zj.nicolike.cn

Py:   for ch in s: print(ch)
来源：http://ax.newstarts.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zx.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://sw.shxzskj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://va.yuexingan06.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wy.huixiangedu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://na.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pa.panjiajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://bu.panjiajie.cn

[E14] URL 编码与 Base64
来源：http://od.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ee.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://af.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ki.huixiangedu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://yb.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://pj.shtwfgs.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jo.huixiangedu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sx.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fr.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://ng.yuntaijiaju.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://es.szsharing.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ml.colortex.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://yg.jianghongdianzi.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://fz.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://yp.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ft.shtwfgs.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://lm.nicolike.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ol.yuexingan06.cn

[E16] 数字千分位
来源：http://mz.muxihuayi.cn

Py:   f"{1234567:,}"
来源：http://yt.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://wq.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wh.asd995.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ey.colortex.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tl.9csxet.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://au.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pl.bookmarksfly.cn

C#:   1234567.ToString("N0")
来源：http://ni.shtwfgs.cn

[E17] 首字母大写
来源：http://jk.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://vr.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bw.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zm.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kp.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://um.9csxet.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://qj.chemitech.net.cn

Ruby: s.capitalize
来源：http://nn.bjjhwx.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://tv.shxzukj.cn

[E18] 模板占位符替换
来源：http://tk.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://xs.szsharing.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://zm.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wq.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ak.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dy.haigaiapp.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zt.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://am.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://fp.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://bu.9csxet.cn

Py:   s.splitlines()
来源：http://cp.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://os.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://ls.yuntaijiaju.cn

TS:   s.split(/\r?\n/)
来源：http://he.haigaiapp.cn

Java: s.lines().toList()
来源：http://lw.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://vb.jianghongdianzi.cn

Ruby: s.lines
来源：http://oo.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://ac.huanxung.cn

[E20] 判断字符串是否为空
来源：http://xw.szxytkj.cn

Py:   if not s:
来源：http://tn.muxihuayi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uc.hnjuh.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ib.chemitech.net.cn

TS:   if (s === "") {}
来源：http://qp.lnxyls.cn

Java: if (s.isEmpty()) {}
来源：http://xy.muxihuayi.cn

Go:   if s == "" {}
来源：http://ue.asd995.cn

Ruby: if s.empty?
来源：http://oz.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://kg.521024.cn

[E21] 超长截断加省略号
来源：http://yz.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ol.haigaiapp.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://we.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ku.asd995.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rp.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mh.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://mw.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://qg.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wc.hahajie.cn

[E22] 字节长度与字符长度
来源：http://mc.bjjhwx.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://re.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dp.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jb.panjiajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://rb.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://rv.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://st.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://sc.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jm.huixiangedu.cn

================================================================================
来源：http://mu.shxzukj.cn

F. 文件与目录
来源：http://sr.yuexingan06.cn

================================================================================
来源：http://tv.nszjky.cn

[F01] 读取整个文件
来源：http://bs.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://km.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://ce.panjiajie.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nc.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nj.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://in.wgjwhj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ae.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://oe.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://bu.hahajie.cn

[F02] 逐行读取文件
来源：http://oc.newstarts.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://xu.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://az.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ea.haigaiapp.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wg.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xv.shxzskj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yy.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hw.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ws.9csxet.cn

[F03] 写入文件（覆盖）
来源：http://ky.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xp.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vk.hahajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://dw.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wd.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yw.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ba.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://pq.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hw.gzmigu.cn

[F04] 追加写入文件
来源：http://ju.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qx.lnxyls.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hl.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dg.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ab.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ye.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://my.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wf.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lm.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://ps.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wu.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://tl.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://tf.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://vd.521024.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sf.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://th.yuntaijiaju.cn

Ruby: File.exist?("a.txt")
来源：http://uc.huixiangedu.cn

C#:   File.Exists("a.txt")
来源：http://qg.bjjhwx.cn

[F06] 删除文件
来源：http://es.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://kd.colortex.cn

PHP:  unlink("a.txt");
来源：http://kf.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://hy.shtwfgs.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ja.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nb.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://ns.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://ti.colortex.cn

C#:   File.Delete("a.txt");
来源：http://yy.nszjky.cn

[F07] 创建目录（含多级）
来源：http://an.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://rj.shxzukj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zj.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rk.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dh.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://pr.bjjhwx.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://oq.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://yz.yuntaijiaju.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://by.szsharing.cn

[F08] 遍历目录
来源：http://bp.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://yp.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ai.panjiajie.cn

JS:   fs.readdirSync("dir")
来源：http://uy.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://fr.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://yy.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vm.szsharing.cn

Ruby: Dir.children("dir")
来源：http://rh.jianghongdianzi.cn

C#:   Directory.GetFiles("dir")
来源：http://hz.jianghongdianzi.cn

[F09] 获取文件大小
来源：http://xf.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://lv.521024.cn

PHP:  filesize("a.txt");
来源：http://sg.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://hl.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://mj.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yj.muxihuayi.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bf.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://dw.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://ch.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ge.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://bh.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ey.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://vd.521024.cn

TS:   path.extname("a.txt")
来源：http://vf.yuntaijiaju.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xt.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qe.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://kz.jctech888.com.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://df.haigaiapp.cn

[F11] 复制与移动文件
来源：http://qt.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jk.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rs.yuntaijiaju.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jx.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zp.huixinmuqiang.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rn.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ry.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fn.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://uo.panjiajie.cn

[F12] CSV 读写
来源：http://sw.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nn.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ex.newstarts.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://oh.yuntaijiaju.cn

TS:   // 同上
来源：http://mk.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jb.huanxung.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://vx.gzmigu.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mj.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://em.9csxet.cn


<!-- 参考信息 -->