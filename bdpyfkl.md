代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://fu.haigaiapp.cn

C#:   s.Substring(1, 3)
来源：http://me.asd995.cn

[E04] 查找子串位置
来源：http://lk.lnxyls.cn

Py:   s.find("x");  s.index("x")
来源：http://sm.shxzskj.cn

PHP:  strpos($s, "x");
来源：http://wm.wgjwhj.cn

JS:   s.indexOf("x");  s.search(/x/)
来源：http://yy.colortex.cn

TS:   s.indexOf("x")
来源：http://kr.jctech888.com.cn

Java: s.indexOf("x")
来源：http://zo.yuexingan06.cn

Go:   strings.Index(s, "x")
来源：http://aa.asd995.cn

Ruby: s.index("x")
来源：http://jj.bookmarksfly.cn

C#:   s.IndexOf("x")
来源：http://lw.shtwfgs.cn

[E05] 判断包含 / 前缀 / 后缀
来源：http://qs.wgjwhj.cn

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://fp.haigaiapp.cn

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://ud.yuexingan06.cn

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://en.muxihuayi.cn

TS:   s.includes("x");  s.startsWith("a")
来源：http://kt.lnxyls.cn

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://xa.muxihuayi.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ju.panjiajie.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://jg.wgjwhj.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://da.huixiangedu.cn

[E06] 替换子串
来源：http://hd.9csxet.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://kf.szxytkj.cn

PHP:  str_replace("a", "b", $s);
来源：http://fo.szxytkj.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://sm.wgjwhj.cn

TS:   s.replaceAll("a", "b")
来源：http://vn.gzmigu.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://oz.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://bz.jctech888.com.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ft.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://yh.hahajie.cn

[E07] 按分隔符拆分
来源：http://to.panjiajie.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://cg.hahajie.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://ik.panjiajie.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://tt.9csxet.cn

TS:   s.split(",")
来源：http://ac.hahajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://yt.nicolike.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://em.muxihuayi.cn

Ruby: s.split(",");  s.split
来源：http://po.hnjuh.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mz.bookmarksfly.cn

[E08] 数组按分隔符合并
来源：http://yt.yuntaijiaju.cn

Py:   ",".join(items)
来源：http://ar.asd995.cn

PHP:  implode(",", $items);
来源：http://qu.lnxyls.cn

JS:   items.join(",")
来源：http://wz.hnjuh.cn

TS:   items.join(",")
来源：http://ns.wgjwhj.cn

Java: String.join(",", items)
来源：http://ww.muxihuayi.cn

Go:   strings.Join(items, ",")
来源：http://vp.hahajie.cn

Ruby: items.join(",")
来源：http://gv.chemitech.net.cn

C#:   string.Join(",", items)
来源：http://cz.colortex.cn

[E09] 去除所有空白字符
来源：http://fv.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://vi.panjiajie.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ws.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ft.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://ro.bookmarksfly.cn

Java: s.replaceAll("\\s+", "")
来源：http://fw.jctech888.com.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hq.newstarts.cn

Ruby: s.gsub(/\s+/, "")
来源：http://vh.huixinmuqiang.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://oy.newstarts.cn

[E10] 左侧补零 / 定长填充
来源：http://qm.jctech888.com.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://bf.shxzskj.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://uj.haigaiapp.cn

JS:   "7".padStart(3, "0")
来源：http://rj.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://xj.asd995.cn

Java: String.format("%03d", 7)
来源：http://ty.asd995.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bn.521024.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lr.chemitech.net.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ug.521024.cn

[E11] 反转字符串
来源：http://xh.nicolike.cn

Py:   s[::-1]
来源：http://ih.chemitech.net.cn

PHP:  strrev($s);
来源：http://ni.huixinmuqiang.cn

JS:   [...s].reverse().join("")
来源：http://ve.shxzukj.cn

TS:   [...s].reverse().join("")
来源：http://zm.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://us.9csxet.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://fl.shxzskj.cn

Ruby: s.reverse
来源：http://ht.huixinmuqiang.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uy.gzmigu.cn

[E12] 统计某字符出现次数
来源：http://kp.bjjhwx.cn

Py:   s.count("a")
来源：http://it.bjjhwx.cn

PHP:  substr_count($s, "a");
来源：http://jc.yuntaijiaju.cn

JS:   s.split("a").length - 1
来源：http://tg.huixinmuqiang.cn

TS:   s.split("a").length - 1
来源：http://oy.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://bf.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://fo.hnjuh.cn

Ruby: s.count("a")
来源：http://kx.hnjuh.cn

C#:   s.Count(c => c == 'a')
来源：http://ut.wgjwhj.cn

[E13] 逐字符遍历
来源：http://mq.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://zl.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gr.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kb.muxihuayi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vn.hnjuh.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://qe.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wr.huanxung.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://fo.521024.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qm.nszjky.cn

[E14] URL 编码与 Base64
来源：http://uj.chemitech.net.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vz.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jk.muxihuayi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ot.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mv.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://jj.haigaiapp.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://dd.newstarts.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ly.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wd.newstarts.cn

[E15] HTML 转义 / 反转义
来源：http://pl.chemitech.net.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jg.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://uo.bookmarksfly.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://qb.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hg.huixiangedu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ro.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ha.newstarts.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wy.szxytkj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ei.nszjky.cn

[E16] 数字千分位
来源：http://eg.szsharing.cn

Py:   f"{1234567:,}"
来源：http://tw.nszjky.cn

PHP:  number_format(1234567);
来源：http://is.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ko.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://za.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ot.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://nz.wgjwhj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://dh.chemitech.net.cn

C#:   1234567.ToString("N0")
来源：http://bb.lnxyls.cn

[E17] 首字母大写
来源：http://wt.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://df.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yd.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dw.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bq.huanxung.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zl.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://su.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://eh.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ih.szsharing.cn

[E18] 模板占位符替换
来源：http://yk.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ms.521024.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wv.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://bg.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://de.asd995.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pa.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sg.panjiajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wo.colortex.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ly.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://io.huixiangedu.cn

Py:   s.splitlines()
来源：http://dp.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ce.bjjhwx.cn

JS:   s.split(/\r?\n/)
来源：http://ib.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://fc.lnxyls.cn

Java: s.lines().toList()
来源：http://lt.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ad.shxzskj.cn

Ruby: s.lines
来源：http://gl.huixiangedu.cn

C#:   s.Split('\n')
来源：http://vi.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://ek.wgjwhj.cn

Py:   if not s:
来源：http://tv.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://vc.jianghongdianzi.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://xg.colortex.cn

TS:   if (s === "") {}
来源：http://pt.nicolike.cn

Java: if (s.isEmpty()) {}
来源：http://mh.huanxung.cn

Go:   if s == "" {}
来源：http://fu.lnxyls.cn

Ruby: if s.empty?
来源：http://nk.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vq.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://kh.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xb.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://my.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ug.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ak.huixinmuqiang.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tr.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://nf.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ws.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ki.szsharing.cn

[E22] 字节长度与字符长度
来源：http://bp.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xe.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wc.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ja.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vx.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ts.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xw.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://ca.nicolike.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://px.huixiangedu.cn

================================================================================
来源：http://wb.shtwfgs.cn

F. 文件与目录
来源：http://bc.muxihuayi.cn

================================================================================
来源：http://ev.lnxyls.cn

[F01] 读取整个文件
来源：http://rb.szsharing.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ky.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://dj.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://gr.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vp.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://yz.bookmarksfly.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://zu.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://mi.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://ho.521024.cn

[F02] 逐行读取文件
来源：http://zf.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tu.newstarts.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://sl.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ep.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cr.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ie.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://eu.huixiangedu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yq.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://cb.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://pu.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vh.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bk.szxytkj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://az.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://lh.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://gl.colortex.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vz.jctech888.com.cn

Ruby: File.write("a.txt", "hi")
来源：http://ko.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://rw.asd995.cn

[F04] 追加写入文件
来源：http://gd.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://sn.szxytkj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ha.shxzukj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://km.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://yv.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ro.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jv.jianghongdianzi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nx.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mx.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://dk.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wy.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://rv.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://es.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://xs.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ci.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nc.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://yn.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://sf.szsharing.cn

[F06] 删除文件
来源：http://ks.9csxet.cn

Py:   os.remove("a.txt")
来源：http://vo.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://hi.gzmigu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wd.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://wq.panjiajie.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zv.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://hr.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://as.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://ok.szsharing.cn

[F07] 创建目录（含多级）
来源：http://hz.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ka.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ci.shxzskj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tn.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ic.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://de.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://no.huanxung.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qe.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xy.szxytkj.cn

[F08] 遍历目录
来源：http://vl.chemitech.net.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://oz.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jz.szsharing.cn

JS:   fs.readdirSync("dir")
来源：http://bk.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://ps.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://bb.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ov.asd995.cn

Ruby: Dir.children("dir")
来源：http://ac.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://jp.asd995.cn

[F09] 获取文件大小
来源：http://sy.jctech888.com.cn

Py:   os.path.getsize("a.txt")
来源：http://sw.9csxet.cn

PHP:  filesize("a.txt");
来源：http://ji.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://zm.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://ir.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ju.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://we.9csxet.cn

Ruby: File.size("a.txt")
来源：http://im.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ky.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ow.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://pi.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://jy.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gy.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ed.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vs.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://vi.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xr.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pe.huanxung.cn

[F11] 复制与移动文件
来源：http://vn.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vj.colortex.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gp.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dd.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bq.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://sb.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kn.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gi.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://dp.szsharing.cn

[F12] CSV 读写
来源：http://in.chemitech.net.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://oh.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ld.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://tu.wgjwhj.cn

TS:   // 同上
来源：http://oa.bjjhwx.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://op.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hx.huanxung.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://em.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sm.hnjuh.cn

================================================================================
来源：http://so.jctech888.com.cn

G. 面向对象
来源：http://mu.shxzskj.cn

================================================================================
来源：http://xe.shtwfgs.cn

[G01] 定义类
来源：http://qr.szsharing.cn

Py:   class User: pass
来源：http://se.yuntaijiaju.cn

PHP:  class User {}
来源：http://ck.colortex.cn

JS:   class User {}
来源：http://fq.huixiangedu.cn

TS:   class User { name: string = ""; }
来源：http://lk.hnjuh.cn

Java: class User {}
来源：http://sc.colortex.cn

Go:   type User struct { Name string }
来源：http://nl.colortex.cn

Ruby: class User; end
来源：http://gm.huixiangedu.cn

C#:   class User {}
来源：http://wc.lnxyls.cn

[G02] 构造函数
来源：http://vx.yuntaijiaju.cn

Py:   def __init__(self, name): self.name = name
来源：http://kt.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://fy.lnxyls.cn

JS:   constructor(name) { this.name = name; }
来源：http://yj.shxzskj.cn


<!-- 参考信息 -->