代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wa.colortex.cn

[E03] 截取子串
来源：http://mc.szxytkj.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://jk.jctech888.com.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://qj.huanxung.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://is.szxytkj.cn

TS:   s.slice(1, 4)
来源：http://iz.jianghongdianzi.cn

Java: s.substring(1, 4)
来源：http://ht.szxytkj.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://nw.huanxung.cn

Ruby: s[1, 3];  s[1..3]
来源：http://na.shtwfgs.cn

C#:   s.Substring(1, 3)
来源：http://jx.shxzskj.cn

[E04] 查找子串位置
来源：http://dc.jianghongdianzi.cn

Py:   s.find("x");  s.index("x")
来源：http://qa.chemitech.net.cn

PHP:  strpos($s, "x");
来源：http://kg.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://cq.nicolike.cn

TS:   s.indexOf("x")
来源：http://yd.muxihuayi.cn

Java: s.indexOf("x")
来源：http://ru.nszjky.cn

Go:   strings.Index(s, "x")
来源：http://ac.chemitech.net.cn

Ruby: s.index("x")
来源：http://vs.panjiajie.cn

C#:   s.IndexOf("x")
来源：http://ci.chemitech.net.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://te.huixinmuqiang.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://lo.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://jh.szxytkj.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wk.nszjky.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://je.hahajie.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://un.9csxet.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wp.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://vd.huixinmuqiang.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://os.jianghongdianzi.cn

[E06] 替换子串
来源：http://lm.huanxung.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://vh.shtwfgs.cn

PHP:  str_replace("a", "b", $s);
来源：http://rt.colortex.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://yt.9csxet.cn

TS:   s.replaceAll("a", "b")
来源：http://ru.haigaiapp.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://cz.huixiangedu.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://ds.hnjuh.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://nf.haigaiapp.cn

C#:   s.Replace("a", "b")
来源：http://ri.chemitech.net.cn

[E07] 按分隔符拆分
来源：http://yv.colortex.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://an.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ey.nicolike.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://ab.9csxet.cn

TS:   s.split(",")
来源：http://kw.hnjuh.cn

Java: s.split(",");  s.split("\\s+")
来源：http://ej.521024.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wx.szxytkj.cn

Ruby: s.split(",");  s.split
来源：http://un.521024.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://js.9csxet.cn

[E08] 数组按分隔符合并
来源：http://we.shtwfgs.cn

Py:   ",".join(items)
来源：http://ea.colortex.cn

PHP:  implode(",", $items);
来源：http://rs.muxihuayi.cn

JS:   items.join(",")
来源：http://yh.asd995.cn

TS:   items.join(",")
来源：http://jc.jianghongdianzi.cn

Java: String.join(",", items)
来源：http://xu.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://qo.szsharing.cn

Ruby: items.join(",")
来源：http://sc.szxytkj.cn

C#:   string.Join(",", items)
来源：http://sf.gzmigu.cn

[E09] 去除所有空白字符
来源：http://dx.muxihuayi.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zg.yuexingan06.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ey.jianghongdianzi.cn

JS:   s.replace(/\s+/g, "")
来源：http://ti.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://ku.haigaiapp.cn

Java: s.replaceAll("\\s+", "")
来源：http://oo.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gr.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://jb.nicolike.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://cv.yuexingan06.cn

[E10] 左侧补零 / 定长填充
来源：http://rl.gzmigu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://dh.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://xv.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://ek.hnjuh.cn

TS:   "7".padStart(3, "0")
来源：http://bb.huanxung.cn

Java: String.format("%03d", 7)
来源：http://ma.huanxung.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ha.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://yq.huanxung.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://da.panjiajie.cn

[E11] 反转字符串
来源：http://uz.521024.cn

Py:   s[::-1]
来源：http://bo.bookmarksfly.cn

PHP:  strrev($s);
来源：http://co.asd995.cn

JS:   [...s].reverse().join("")
来源：http://qp.bookmarksfly.cn

TS:   [...s].reverse().join("")
来源：http://px.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jq.colortex.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://by.shxzukj.cn

Ruby: s.reverse
来源：http://hw.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://it.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://bp.asd995.cn

Py:   s.count("a")
来源：http://gh.haigaiapp.cn

PHP:  substr_count($s, "a");
来源：http://pz.nszjky.cn

JS:   s.split("a").length - 1
来源：http://uu.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://tg.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ne.szxytkj.cn

Go:   strings.Count(s, "a")
来源：http://cw.wgjwhj.cn

Ruby: s.count("a")
来源：http://gj.szsharing.cn

C#:   s.Count(c => c == 'a')
来源：http://on.jctech888.com.cn

[E13] 逐字符遍历
来源：http://wr.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://de.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ff.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hc.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ih.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://fg.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ed.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://pk.jianghongdianzi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://jv.haigaiapp.cn

[E14] URL 编码与 Base64
来源：http://ca.9csxet.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xs.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://rp.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://yk.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hj.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://dy.shxzskj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tp.panjiajie.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fc.yuexingan06.cn

[E15] HTML 转义 / 反转义
来源：http://vo.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://kz.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://iy.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lv.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ux.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://bx.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://tj.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ma.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pe.huixiangedu.cn

[E16] 数字千分位
来源：http://fl.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://cr.bjjhwx.cn

PHP:  number_format(1234567);
来源：http://mx.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bj.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fa.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vc.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vz.haigaiapp.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://bp.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://mr.lnxyls.cn

[E17] 首字母大写
来源：http://hy.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ow.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qx.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gf.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xf.haigaiapp.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vx.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://pa.9csxet.cn

Ruby: s.capitalize
来源：http://je.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ib.hahajie.cn

[E18] 模板占位符替换
来源：http://wx.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hi.bookmarksfly.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pl.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ct.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yt.lnxyls.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cz.huixiangedu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mt.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://kr.huixinmuqiang.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qw.521024.cn

[E19] 多行文本按行拆分
来源：http://vb.shtwfgs.cn

Py:   s.splitlines()
来源：http://gd.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://as.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://gr.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://gs.huixiangedu.cn

Java: s.lines().toList()
来源：http://uy.asd995.cn

Go:   strings.Split(s, "\n")
来源：http://gd.shxzukj.cn

Ruby: s.lines
来源：http://qy.bjjhwx.cn

C#:   s.Split('\n')
来源：http://do.newstarts.cn

[E20] 判断字符串是否为空
来源：http://rt.panjiajie.cn

Py:   if not s:
来源：http://nb.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://rg.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://yh.yuexingan06.cn

TS:   if (s === "") {}
来源：http://re.wgjwhj.cn

Java: if (s.isEmpty()) {}
来源：http://vo.huixiangedu.cn

Go:   if s == "" {}
来源：http://tf.panjiajie.cn

Ruby: if s.empty?
来源：http://qr.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qb.9csxet.cn

[E21] 超长截断加省略号
来源：http://gk.huanxung.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iz.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://us.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.shxzukj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rm.bjjhwx.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://zp.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ne.lnxyls.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://vp.nicolike.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://yg.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://qd.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://fo.chemitech.net.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hs.9csxet.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gv.yuntaijiaju.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wq.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hv.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sd.shxzskj.cn

Ruby: s.bytesize;  s.length
来源：http://bn.hahajie.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mh.nicolike.cn

================================================================================
来源：http://en.gzmigu.cn

F. 文件与目录
来源：http://gf.newstarts.cn

================================================================================
来源：http://pl.wgjwhj.cn

[F01] 读取整个文件
来源：http://vs.lnxyls.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lt.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://ho.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://rn.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://io.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fh.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tr.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://oo.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://zk.panjiajie.cn

[F02] 逐行读取文件
来源：http://jp.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cl.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qd.9csxet.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bk.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://nt.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qy.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tw.szxytkj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fl.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ze.nszjky.cn

[F03] 写入文件（覆盖）
来源：http://pq.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://za.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://jr.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gv.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jj.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gj.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://nt.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://bf.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ju.newstarts.cn

[F04] 追加写入文件
来源：http://qi.nszjky.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pz.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://lf.haigaiapp.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lt.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gz.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ao.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://km.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ws.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kl.hnjuh.cn

[F05] 判断文件或目录是否存在
来源：http://qa.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ot.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ew.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://jt.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://up.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dw.yuntaijiaju.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ay.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://zt.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://lf.jctech888.com.cn

[F06] 删除文件
来源：http://lv.huanxung.cn

Py:   os.remove("a.txt")
来源：http://hp.szsharing.cn

PHP:  unlink("a.txt");
来源：http://wn.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ze.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wq.jctech888.com.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ps.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://xl.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://nj.521024.cn

C#:   File.Delete("a.txt");
来源：http://pk.yuexingan06.cn

[F07] 创建目录（含多级）
来源：http://zr.bookmarksfly.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bn.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hf.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://he.yuntaijiaju.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yu.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xf.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ed.wgjwhj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://sx.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ex.shxzukj.cn

[F08] 遍历目录
来源：http://ch.nszjky.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ff.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kc.huanxung.cn

JS:   fs.readdirSync("dir")
来源：http://ls.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://le.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hc.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://nn.jianghongdianzi.cn

Ruby: Dir.children("dir")
来源：http://nr.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://js.hahajie.cn

[F09] 获取文件大小
来源：http://zw.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://ye.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://tj.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://hf.nicolike.cn

TS:   fs.statSync("a.txt").size
来源：http://ae.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ke.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ul.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://nw.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://cu.muxihuayi.cn

[F10] 取文件扩展名 / 文件名
来源：http://lc.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xm.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://aj.yuexingan06.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://er.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://xb.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jd.yuexingan06.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lx.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hb.bjjhwx.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://aa.newstarts.cn

[F11] 复制与移动文件
来源：http://zp.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hw.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oc.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rf.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tj.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ds.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ni.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pm.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yr.wgjwhj.cn

[F12] CSV 读写
来源：http://pm.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ke.szsharing.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qr.huixinmuqiang.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xe.bjjhwx.cn

TS:   // 同上
来源：http://uw.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wj.huixinmuqiang.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yt.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jt.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://gn.shtwfgs.cn

================================================================================
来源：http://fz.chemitech.net.cn

G. 面向对象
来源：http://sz.szsharing.cn

================================================================================
来源：http://fa.bookmarksfly.cn

[G01] 定义类
来源：http://ya.colortex.cn

Py:   class User: pass
来源：http://rx.haigaiapp.cn

PHP:  class User {}
来源：http://rb.lnxyls.cn

JS:   class User {}
来源：http://km.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://am.huanxung.cn


<!-- 参考信息 -->