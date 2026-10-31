代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://al.haigaiapp.cn

[E03] 截取子串
来源：http://wg.huanxung.cn

Py:   s[1:4];  s[:3];  s[3:]
来源：http://ho.9csxet.cn

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://dz.panjiajie.cn

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://np.bjjhwx.cn

TS:   s.slice(1, 4)
来源：http://dn.bookmarksfly.cn

Java: s.substring(1, 4)
来源：http://nn.yuntaijiaju.cn

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://fp.shxzskj.cn

Ruby: s[1, 3];  s[1..3]
来源：http://xr.gzmigu.cn

C#:   s.Substring(1, 3)
来源：http://ll.jianghongdianzi.cn

[E04] 查找子串位置
来源：http://ma.wgjwhj.cn

Py:   s.find("x");  s.index("x")
来源：http://ba.shxzukj.cn

PHP:  strpos($s, "x");
来源：http://ts.9csxet.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://xq.9csxet.cn

TS:   s.indexOf("x")
来源：http://am.huixiangedu.cn

Java: s.indexOf("x")
来源：http://ku.shtwfgs.cn

Go:   strings.Index(s, "x")
来源：http://se.szsharing.cn

Ruby: s.index("x")
来源：http://ad.yuexingan06.cn

C#:   s.IndexOf("x")
来源：http://zg.gzmigu.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qh.asd995.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://ar.huixiangedu.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://kn.hahajie.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://cs.bookmarksfly.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kj.huanxung.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://bm.yuexingan06.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ps.szxytkj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://aj.yuexingan06.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://gp.shxzukj.cn

[E06] 替换子串
来源：http://ul.newstarts.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://zo.szsharing.cn

PHP:  str_replace("a", "b", $s);
来源：http://xr.asd995.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ia.hahajie.cn

TS:   s.replaceAll("a", "b")
来源：http://wt.shtwfgs.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ae.chemitech.net.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://yq.lnxyls.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://fu.huanxung.cn

C#:   s.Replace("a", "b")
来源：http://cn.hnjuh.cn

[E07] 按分隔符拆分
来源：http://ps.bookmarksfly.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mn.asd995.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://if.nszjky.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://pw.bookmarksfly.cn

TS:   s.split(",")
来源：http://qt.521024.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hc.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://ym.huixinmuqiang.cn

Ruby: s.split(",");  s.split
来源：http://ul.chemitech.net.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://cz.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://vw.lnxyls.cn

Py:   ",".join(items)
来源：http://yb.jctech888.com.cn

PHP:  implode(",", $items);
来源：http://fp.nszjky.cn

JS:   items.join(",")
来源：http://yh.wgjwhj.cn

TS:   items.join(",")
来源：http://dv.9csxet.cn

Java: String.join(",", items)
来源：http://hg.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://nr.newstarts.cn

Ruby: items.join(",")
来源：http://rq.huanxung.cn

C#:   string.Join(",", items)
来源：http://wy.shxzskj.cn

[E09] 去除所有空白字符
来源：http://kc.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://if.hnjuh.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://jn.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://su.wgjwhj.cn

TS:   s.replace(/\s+/g, "")
来源：http://al.huixinmuqiang.cn

Java: s.replaceAll("\\s+", "")
来源：http://tr.panjiajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://fq.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://mb.asd995.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://yw.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://ip.shxzskj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sq.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://md.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://ar.bookmarksfly.cn

TS:   "7".padStart(3, "0")
来源：http://up.shxzskj.cn

Java: String.format("%03d", 7)
来源：http://da.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tm.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uq.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://pn.lnxyls.cn

[E11] 反转字符串
来源：http://kd.bookmarksfly.cn

Py:   s[::-1]
来源：http://qj.hahajie.cn

PHP:  strrev($s);
来源：http://ui.colortex.cn

JS:   [...s].reverse().join("")
来源：http://pg.asd995.cn

TS:   [...s].reverse().join("")
来源：http://qe.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://jv.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oy.jctech888.com.cn

Ruby: s.reverse
来源：http://tx.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ya.bookmarksfly.cn

[E12] 统计某字符出现次数
来源：http://cm.521024.cn

Py:   s.count("a")
来源：http://qz.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://he.hnjuh.cn

JS:   s.split("a").length - 1
来源：http://dz.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://dl.shxzukj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://im.muxihuayi.cn

Go:   strings.Count(s, "a")
来源：http://bv.nszjky.cn

Ruby: s.count("a")
来源：http://jg.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://cy.bjjhwx.cn

[E13] 逐字符遍历
来源：http://ks.9csxet.cn

Py:   for ch in s: print(ch)
来源：http://rt.bjjhwx.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://as.huixiangedu.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://qz.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://rh.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://bf.bjjhwx.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tr.9csxet.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ac.chemitech.net.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://lf.hnjuh.cn

[E14] URL 编码与 Base64
来源：http://iv.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ku.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ti.shxzukj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://bu.hahajie.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fi.huixinmuqiang.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://yn.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ce.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://sk.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cz.hahajie.cn

[E15] HTML 转义 / 反转义
来源：http://aq.huixinmuqiang.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rz.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ep.hahajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://cb.nszjky.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://sy.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ds.muxihuayi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://cf.huixinmuqiang.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://fu.gzmigu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://bs.9csxet.cn

[E16] 数字千分位
来源：http://dt.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://ik.hnjuh.cn

PHP:  number_format(1234567);
来源：http://dv.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ff.gzmigu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://te.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://de.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dp.szxytkj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://va.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://jc.shxzskj.cn

[E17] 首字母大写
来源：http://eo.huixiangedu.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://cr.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ms.nszjky.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kb.hahajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ib.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://cg.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://tu.nicolike.cn

Ruby: s.capitalize
来源：http://zg.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ao.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://fc.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://aw.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dr.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vd.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://am.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ue.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hg.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://eg.colortex.cn

[E19] 多行文本按行拆分
来源：http://xh.muxihuayi.cn

Py:   s.splitlines()
来源：http://dl.wgjwhj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ox.colortex.cn

JS:   s.split(/\r?\n/)
来源：http://rl.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://dm.nszjky.cn

Java: s.lines().toList()
来源：http://gm.newstarts.cn

Go:   strings.Split(s, "\n")
来源：http://ua.hahajie.cn

Ruby: s.lines
来源：http://dg.shxzukj.cn

C#:   s.Split('\n')
来源：http://lu.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://xu.wgjwhj.cn

Py:   if not s:
来源：http://do.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yz.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://it.yuntaijiaju.cn

TS:   if (s === "") {}
来源：http://vp.gzmigu.cn

Java: if (s.isEmpty()) {}
来源：http://kn.shxzukj.cn

Go:   if s == "" {}
来源：http://zi.hahajie.cn

Ruby: if s.empty?
来源：http://nx.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wp.panjiajie.cn

[E21] 超长截断加省略号
来源：http://px.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sf.asd995.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hc.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lh.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gh.shxzukj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://yv.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://jv.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://zx.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rr.muxihuayi.cn

[E22] 字节长度与字符长度
来源：http://ld.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mz.shxzukj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ep.nszjky.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ok.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nj.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ar.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ra.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://ci.yuexingan06.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://se.bookmarksfly.cn

================================================================================
来源：http://tk.bookmarksfly.cn

F. 文件与目录
来源：http://bp.hnjuh.cn

================================================================================
来源：http://qv.hnjuh.cn

[F01] 读取整个文件
来源：http://bp.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kw.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://fg.asd995.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://et.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://oi.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pm.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dp.szsharing.cn

Ruby: File.read("a.txt")
来源：http://rs.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://wi.nszjky.cn

[F02] 逐行读取文件
来源：http://vx.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qs.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wh.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qi.nszjky.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xy.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://pm.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pe.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sp.shxzukj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pf.bookmarksfly.cn

[F03] 写入文件（覆盖）
来源：http://hu.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://im.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cw.shxzskj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hp.colortex.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lq.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mw.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rh.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://zr.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://dy.szsharing.cn

[F04] 追加写入文件
来源：http://av.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ye.asd995.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ii.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://it.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ca.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://tb.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://vx.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://me.bjjhwx.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://vh.jianghongdianzi.cn

[F05] 判断文件或目录是否存在
来源：http://ip.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lx.shxzskj.cn

PHP:  file_exists("a.txt");
来源：http://ah.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://il.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://ns.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ro.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ws.jianghongdianzi.cn

Ruby: File.exist?("a.txt")
来源：http://ho.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://hh.shtwfgs.cn

[F06] 删除文件
来源：http://bn.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ow.huixiangedu.cn

PHP:  unlink("a.txt");
来源：http://va.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://mi.9csxet.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ml.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ja.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://oj.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://aj.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://xg.colortex.cn

[F07] 创建目录（含多级）
来源：http://zd.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wp.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://du.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tv.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wr.huanxung.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://zi.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://md.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://th.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://rl.shtwfgs.cn

[F08] 遍历目录
来源：http://an.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vl.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qm.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://dx.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://pm.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sk.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xc.shtwfgs.cn

Ruby: Dir.children("dir")
来源：http://cq.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://vr.wgjwhj.cn

[F09] 获取文件大小
来源：http://pt.huixiangedu.cn

Py:   os.path.getsize("a.txt")
来源：http://ak.colortex.cn

PHP:  filesize("a.txt");
来源：http://wr.bookmarksfly.cn

JS:   fs.statSync("a.txt").size
来源：http://xm.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://qa.huixiangedu.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bu.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kx.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://cr.szxytkj.cn

C#:   new FileInfo("a.txt").Length
来源：http://xl.huixiangedu.cn

[F10] 取文件扩展名 / 文件名
来源：http://sj.yuntaijiaju.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jf.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://is.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qn.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://qw.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://rj.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yr.hnjuh.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gc.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tw.hahajie.cn

[F11] 复制与移动文件
来源：http://sf.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xu.bookmarksfly.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://kn.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vy.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oq.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pd.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://sp.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://sz.colortex.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ti.shtwfgs.cn

[F12] CSV 读写
来源：http://yh.hnjuh.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kb.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nv.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kr.shxzukj.cn

TS:   // 同上
来源：http://az.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://dn.bjjhwx.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kn.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://oy.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://np.yuntaijiaju.cn

================================================================================
来源：http://qe.szsharing.cn

G. 面向对象
来源：http://uv.nszjky.cn

================================================================================
来源：http://wf.wgjwhj.cn

[G01] 定义类
来源：http://nu.hnjuh.cn

Py:   class User: pass
来源：http://cb.nicolike.cn

PHP:  class User {}
来源：http://cp.newstarts.cn

JS:   class User {}
来源：http://tq.shxzukj.cn

TS:   class User { name: string = ""; }
来源：http://ys.hahajie.cn


<!-- 参考信息 -->