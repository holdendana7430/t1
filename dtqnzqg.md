代发 wailian999

TS:   "ab".repeat(3)
来源：http://kz.asd995.cn

Java: "ab".repeat(3)
来源：http://rd.muxihuayi.cn

Go:   strings.Repeat("ab", 3)
来源：http://pz.lnxyls.cn

Ruby: "ab" * 3
来源：http://fu.panjiajie.cn

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://gl.hahajie.cn

[E03] 截取子串
来源：http://yl.huixiangedu.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ao.wgjwhj.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://vb.shxzskj.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://fn.shxzukj.cn

TS:   s.slice(1, 4)
来源：http://bl.huanxung.cn

Java: s.substring(1, 4)
来源：http://du.hahajie.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mj.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://uf.huixinmuqiang.cn

C#:   s.Substring(1, 3)
来源：http://he.huixiangedu.cn

[E04] 查找子串位置
来源：http://ft.yuexingan06.cn

Py:   s.find("x");  s.index("x")
来源：http://bn.gzmigu.cn

PHP:  strpos($s, "x");
来源：http://vp.huanxung.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xs.lnxyls.cn

TS:   s.indexOf("x")
来源：http://ru.nszjky.cn

Java: s.indexOf("x")
来源：http://cy.panjiajie.cn

Go:   strings.Index(s, "x")
来源：http://dd.huanxung.cn

Ruby: s.index("x")
来源：http://vv.9csxet.cn

C#:   s.IndexOf("x")
来源：http://dp.hnjuh.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://fj.jianghongdianzi.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://dy.hahajie.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://er.shxzukj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cu.colortex.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://da.yuexingan06.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://zb.yuntaijiaju.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://sf.huixinmuqiang.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ah.521024.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://vp.wgjwhj.cn

[E06] 替换子串
来源：http://bi.yuntaijiaju.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vf.yuntaijiaju.cn

PHP:  str_replace("a", "b", $s);
来源：http://te.hahajie.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ud.nicolike.cn

TS:   s.replaceAll("a", "b")
来源：http://fx.szxytkj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://fa.shxzskj.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ke.yuntaijiaju.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ky.szsharing.cn

C#:   s.Replace("a", "b")
来源：http://tt.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://qg.yuexingan06.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pw.521024.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ih.haigaiapp.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://li.wgjwhj.cn

TS:   s.split(",")
来源：http://ki.nszjky.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hq.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://yh.gzmigu.cn

Ruby: s.split(",");  s.split
来源：http://bx.asd995.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://pv.9csxet.cn

[E08] 数组按分隔符合并
来源：http://sl.haigaiapp.cn

Py:   ",".join(items)
来源：http://jo.hnjuh.cn

PHP:  implode(",", $items);
来源：http://mz.jianghongdianzi.cn

JS:   items.join(",")
来源：http://ym.lnxyls.cn

TS:   items.join(",")
来源：http://nt.gzmigu.cn

Java: String.join(",", items)
来源：http://rq.jianghongdianzi.cn

Go:   strings.Join(items, ",")
来源：http://su.bjjhwx.cn

Ruby: items.join(",")
来源：http://pk.shxzskj.cn

C#:   string.Join(",", items)
来源：http://pk.lnxyls.cn

[E09] 去除所有空白字符
来源：http://kr.huanxung.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wx.wgjwhj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ep.shtwfgs.cn

JS:   s.replace(/\s+/g, "")
来源：http://iv.nicolike.cn

TS:   s.replace(/\s+/g, "")
来源：http://pz.newstarts.cn

Java: s.replaceAll("\\s+", "")
来源：http://lc.huanxung.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sq.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ai.gzmigu.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yu.9csxet.cn

[E10] 左侧补零 / 定长填充
来源：http://uh.huixinmuqiang.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://xs.lnxyls.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bw.huixiangedu.cn

JS:   "7".padStart(3, "0")
来源：http://ll.szxytkj.cn

TS:   "7".padStart(3, "0")
来源：http://uu.nicolike.cn

Java: String.format("%03d", 7)
来源：http://ty.huixiangedu.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zm.panjiajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://ch.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://cw.9csxet.cn

[E11] 反转字符串
来源：http://xg.jctech888.com.cn

Py:   s[::-1]
来源：http://vc.lnxyls.cn

PHP:  strrev($s);
来源：http://kj.521024.cn

JS:   [...s].reverse().join("")
来源：http://kt.wgjwhj.cn

TS:   [...s].reverse().join("")
来源：http://cz.521024.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://aa.panjiajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://it.521024.cn

Ruby: s.reverse
来源：http://vz.hahajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://bf.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://ra.newstarts.cn

Py:   s.count("a")
来源：http://ya.nszjky.cn

PHP:  substr_count($s, "a");
来源：http://oi.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://fx.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://ce.wgjwhj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://jp.gzmigu.cn

Go:   strings.Count(s, "a")
来源：http://mi.huanxung.cn

Ruby: s.count("a")
来源：http://kp.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://ot.shxzskj.cn

[E13] 逐字符遍历
来源：http://ro.lnxyls.cn

Py:   for ch in s: print(ch)
来源：http://kn.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bp.szsharing.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nf.haigaiapp.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://fx.bookmarksfly.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qh.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://bj.521024.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://oe.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://as.huanxung.cn

[E14] URL 编码与 Base64
来源：http://tz.521024.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ev.gzmigu.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nn.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xm.yuntaijiaju.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bc.haigaiapp.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ju.chemitech.net.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://zi.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://yf.bookmarksfly.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://oz.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://tw.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yd.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ni.huanxung.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://zt.shxzukj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://su.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wa.szxytkj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wb.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://aa.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yg.jianghongdianzi.cn

[E16] 数字千分位
来源：http://pu.gzmigu.cn

Py:   f"{1234567:,}"
来源：http://ht.huixinmuqiang.cn

PHP:  number_format(1234567);
来源：http://uj.521024.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://gk.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qu.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gb.wgjwhj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ee.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gy.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://gn.huixiangedu.cn

[E17] 首字母大写
来源：http://td.gzmigu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qd.chemitech.net.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nb.panjiajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yx.newstarts.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kv.shtwfgs.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vf.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hd.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://zo.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ri.szxytkj.cn

[E18] 模板占位符替换
来源：http://tv.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wq.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hl.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xq.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rc.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qu.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dk.yuexingan06.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ii.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yq.panjiajie.cn

[E19] 多行文本按行拆分
来源：http://ik.szsharing.cn

Py:   s.splitlines()
来源：http://nq.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qd.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://kq.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://ea.szxytkj.cn

Java: s.lines().toList()
来源：http://ht.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://kz.huixiangedu.cn

Ruby: s.lines
来源：http://rq.shxzukj.cn

C#:   s.Split('\n')
来源：http://zz.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://fl.newstarts.cn

Py:   if not s:
来源：http://fn.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ko.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yl.wgjwhj.cn

TS:   if (s === "") {}
来源：http://jh.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://eu.szsharing.cn

Go:   if s == "" {}
来源：http://gk.lnxyls.cn

Ruby: if s.empty?
来源：http://oh.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://di.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://hq.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kf.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ci.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mz.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://du.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://cv.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://zf.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zs.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sr.newstarts.cn

[E22] 字节长度与字符长度
来源：http://pp.nszjky.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://yo.lnxyls.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://dq.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://we.bjjhwx.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://aj.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ns.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sg.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://zz.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xz.hnjuh.cn

================================================================================
来源：http://gv.panjiajie.cn

F. 文件与目录
来源：http://wx.lnxyls.cn

================================================================================
来源：http://sb.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://pv.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tf.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://xq.hnjuh.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zv.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ji.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ye.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kv.huanxung.cn

Ruby: File.read("a.txt")
来源：http://od.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://wx.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://qk.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rv.szsharing.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://gy.jianghongdianzi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ih.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://up.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tc.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pp.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://if.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wb.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://jo.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://rs.asd995.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://yu.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ns.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xn.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gs.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bz.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://ot.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rs.bjjhwx.cn

[F04] 追加写入文件
来源：http://jl.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qu.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://za.muxihuayi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gi.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pj.521024.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ov.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xi.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://id.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://cd.szsharing.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zk.newstarts.cn

PHP:  file_exists("a.txt");
来源：http://zg.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://cl.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://ie.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ph.asd995.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nc.nszjky.cn

Ruby: File.exist?("a.txt")
来源：http://oi.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ec.huixinmuqiang.cn

[F06] 删除文件
来源：http://jh.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://tf.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://om.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tt.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://mz.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mr.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://fk.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://aw.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://bb.asd995.cn

[F07] 创建目录（含多级）
来源：http://vt.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://up.nszjky.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pc.bookmarksfly.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hx.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ct.jctech888.com.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ya.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://cu.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wi.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://cw.yuntaijiaju.cn

[F08] 遍历目录
来源：http://vy.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ot.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://nj.yuexingan06.cn

JS:   fs.readdirSync("dir")
来源：http://ko.jctech888.com.cn

TS:   fs.readdirSync("dir")
来源：http://ts.haigaiapp.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mk.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pm.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://em.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://wi.panjiajie.cn

[F09] 获取文件大小
来源：http://vo.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://eg.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://zf.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://rn.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://rg.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://fd.shxzukj.cn

Ruby: File.size("a.txt")
来源：http://ge.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://ni.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://ow.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wh.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://cg.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wa.9csxet.cn

TS:   path.extname("a.txt")
来源：http://bm.gzmigu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vb.szxytkj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ln.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fb.chemitech.net.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xf.nszjky.cn

[F11] 复制与移动文件
来源：http://hu.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://va.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qj.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qc.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ua.bjjhwx.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bp.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qr.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://un.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qr.yuexingan06.cn

[F12] CSV 读写
来源：http://tf.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://te.lnxyls.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ab.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://yw.bjjhwx.cn

TS:   // 同上
来源：http://sz.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zm.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://uo.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zx.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dy.shtwfgs.cn

================================================================================
来源：http://xj.jctech888.com.cn

G. 面向对象
来源：http://qi.nszjky.cn

================================================================================
来源：http://nt.colortex.cn

[G01] 定义类
来源：http://hb.nszjky.cn


<!-- 参考信息 -->