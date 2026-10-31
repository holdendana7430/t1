代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://ka.gzmigu.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://na.shxzskj.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://ac.lnxyls.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://lo.jianghongdianzi.cn

[E06] 替换子串
来源：http://lb.bookmarksfly.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://ej.bookmarksfly.cn

PHP:  str_replace("a", "b", $s);
来源：http://er.nszjky.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://ic.huanxung.cn

TS:   s.replaceAll("a", "b")
来源：http://zn.shxzukj.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://uy.hahajie.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://tu.shtwfgs.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://ct.yuexingan06.cn

C#:   s.Replace("a", "b")
来源：http://sn.jctech888.com.cn

[E07] 按分隔符拆分
来源：http://zx.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pc.wgjwhj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://do.huanxung.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://gc.panjiajie.cn

TS:   s.split(",")
来源：http://me.wgjwhj.cn

Java: s.split(",");  s.split("\\s+")
来源：http://im.chemitech.net.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://rs.bookmarksfly.cn

Ruby: s.split(",");  s.split
来源：http://ft.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://lp.szxytkj.cn

[E08] 数组按分隔符合并
来源：http://bx.shxzskj.cn

Py:   ",".join(items)
来源：http://oa.nszjky.cn

PHP:  implode(",", $items);
来源：http://ht.bjjhwx.cn

JS:   items.join(",")
来源：http://mu.huixiangedu.cn

TS:   items.join(",")
来源：http://sr.bjjhwx.cn

Java: String.join(",", items)
来源：http://of.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://uk.chemitech.net.cn

Ruby: items.join(",")
来源：http://pf.newstarts.cn

C#:   string.Join(",", items)
来源：http://jf.chemitech.net.cn

[E09] 去除所有空白字符
来源：http://ap.nszjky.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ke.9csxet.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hx.haigaiapp.cn

JS:   s.replace(/\s+/g, "")
来源：http://fe.yuexingan06.cn

TS:   s.replace(/\s+/g, "")
来源：http://ty.szxytkj.cn

Java: s.replaceAll("\\s+", "")
来源：http://lq.hahajie.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ov.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://iv.bjjhwx.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://su.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://gh.nszjky.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ab.newstarts.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://om.nicolike.cn

JS:   "7".padStart(3, "0")
来源：http://zr.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://pl.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://sh.szxytkj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://mh.yuntaijiaju.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://rk.hnjuh.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ju.shxzskj.cn

[E11] 反转字符串
来源：http://oq.panjiajie.cn

Py:   s[::-1]
来源：http://rs.nicolike.cn

PHP:  strrev($s);
来源：http://zu.hahajie.cn

JS:   [...s].reverse().join("")
来源：http://ty.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://ln.szsharing.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://bx.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://oa.chemitech.net.cn

Ruby: s.reverse
来源：http://cb.shxzskj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://em.asd995.cn

[E12] 统计某字符出现次数
来源：http://rb.huanxung.cn

Py:   s.count("a")
来源：http://yn.nicolike.cn

PHP:  substr_count($s, "a");
来源：http://ri.521024.cn

JS:   s.split("a").length - 1
来源：http://cj.9csxet.cn

TS:   s.split("a").length - 1
来源：http://nw.jianghongdianzi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://dr.huixiangedu.cn

Go:   strings.Count(s, "a")
来源：http://nv.shxzskj.cn

Ruby: s.count("a")
来源：http://cl.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://lb.colortex.cn

[E13] 逐字符遍历
来源：http://ix.szxytkj.cn

Py:   for ch in s: print(ch)
来源：http://nc.chemitech.net.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hp.colortex.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://dl.szxytkj.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://qq.bjjhwx.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vs.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ny.panjiajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ay.gzmigu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://qu.colortex.cn

[E14] URL 编码与 Base64
来源：http://iu.hahajie.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://tz.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://sx.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://la.hnjuh.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mf.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xp.huixinmuqiang.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://rd.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ng.jianghongdianzi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://jd.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://dd.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://cg.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ar.shxzukj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ha.yuntaijiaju.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://wv.huixinmuqiang.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cc.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gy.hnjuh.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tv.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://pf.szxytkj.cn

[E16] 数字千分位
来源：http://nc.shtwfgs.cn

Py:   f"{1234567:,}"
来源：http://pm.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://ax.lnxyls.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://nu.lnxyls.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ux.shxzukj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jz.hahajie.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fg.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ek.colortex.cn

C#:   1234567.ToString("N0")
来源：http://lw.521024.cn

[E17] 首字母大写
来源：http://cl.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ms.hahajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://np.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zm.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://se.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://uq.wgjwhj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://if.szxytkj.cn

Ruby: s.capitalize
来源：http://nm.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://fn.jianghongdianzi.cn

[E18] 模板占位符替换
来源：http://vn.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://az.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://er.lnxyls.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ph.521024.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ko.wgjwhj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://th.wgjwhj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://re.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://np.muxihuayi.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gx.lnxyls.cn

[E19] 多行文本按行拆分
来源：http://us.lnxyls.cn

Py:   s.splitlines()
来源：http://zu.panjiajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wj.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://zb.shxzskj.cn

TS:   s.split(/\r?\n/)
来源：http://kb.colortex.cn

Java: s.lines().toList()
来源：http://bf.shxzukj.cn

Go:   strings.Split(s, "\n")
来源：http://ru.shxzskj.cn

Ruby: s.lines
来源：http://zu.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://bd.colortex.cn

[E20] 判断字符串是否为空
来源：http://eg.szxytkj.cn

Py:   if not s:
来源：http://ds.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://iy.huixinmuqiang.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://nv.bookmarksfly.cn

TS:   if (s === "") {}
来源：http://as.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://go.shxzukj.cn

Go:   if s == "" {}
来源：http://zi.newstarts.cn

Ruby: if s.empty?
来源：http://oh.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ew.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://dh.haigaiapp.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wf.yuntaijiaju.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tr.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jq.jctech888.com.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ks.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://it.colortex.cn

Go:   // 按 rune 判断长度后截断
来源：http://hw.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ao.newstarts.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rg.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://dx.panjiajie.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uv.huixinmuqiang.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://lb.bookmarksfly.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://dw.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://qw.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dp.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rk.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://xh.521024.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qr.huanxung.cn

================================================================================
来源：http://ui.szxytkj.cn

F. 文件与目录
来源：http://gw.shtwfgs.cn

================================================================================
来源：http://dv.yuexingan06.cn

[F01] 读取整个文件
来源：http://kb.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mw.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://hb.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ux.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jy.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://qi.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://la.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://kf.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ab.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://ub.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://eh.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lu.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wv.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://rd.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ki.hahajie.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nl.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qr.shxzukj.cn

[F03] 写入文件（覆盖）
来源：http://pm.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xv.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vh.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jo.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://km.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://dj.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gb.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://lr.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://iy.521024.cn

[F04] 追加写入文件
来源：http://sl.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bu.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xj.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dg.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cq.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ug.shtwfgs.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://rs.szsharing.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://tt.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qb.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://np.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://zm.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://cs.newstarts.cn

JS:   fs.existsSync("a.txt")
来源：http://ku.bjjhwx.cn

TS:   fs.existsSync("a.txt")
来源：http://gv.muxihuayi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qr.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qn.521024.cn

Ruby: File.exist?("a.txt")
来源：http://te.muxihuayi.cn

C#:   File.Exists("a.txt")
来源：http://zm.yuntaijiaju.cn

[F06] 删除文件
来源：http://ll.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://ml.newstarts.cn

PHP:  unlink("a.txt");
来源：http://kx.panjiajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://re.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vy.shtwfgs.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lp.asd995.cn

Go:   os.Remove("a.txt")
来源：http://fd.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://tr.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://iw.jctech888.com.cn

[F07] 创建目录（含多级）
来源：http://bl.hahajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qu.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://il.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pr.9csxet.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://fl.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uf.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://db.panjiajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zy.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sq.panjiajie.cn

[F08] 遍历目录
来源：http://my.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rw.chemitech.net.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qp.wgjwhj.cn

JS:   fs.readdirSync("dir")
来源：http://iu.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://sf.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://xx.huixiangedu.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://eb.chemitech.net.cn

Ruby: Dir.children("dir")
来源：http://qd.shxzskj.cn

C#:   Directory.GetFiles("dir")
来源：http://eu.521024.cn

[F09] 获取文件大小
来源：http://oi.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://wx.hahajie.cn

PHP:  filesize("a.txt");
来源：http://qv.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://mx.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://dr.haigaiapp.cn

Java: Files.size(Path.of("a.txt"))
来源：http://px.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rx.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://mv.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://wd.colortex.cn

[F10] 取文件扩展名 / 文件名
来源：http://eb.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wd.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oh.shtwfgs.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://cn.newstarts.cn

TS:   path.extname("a.txt")
来源：http://fl.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ge.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ut.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://cx.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://bs.szxytkj.cn

[F11] 复制与移动文件
来源：http://xe.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://yf.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fg.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fi.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jk.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://xs.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://oe.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://cl.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://yb.huanxung.cn

[F12] CSV 读写
来源：http://rj.wgjwhj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://zf.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qu.huanxung.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ef.huanxung.cn

TS:   // 同上
来源：http://wy.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bg.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bd.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://za.yuntaijiaju.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vs.chemitech.net.cn

================================================================================
来源：http://mj.huanxung.cn

G. 面向对象
来源：http://re.jianghongdianzi.cn

================================================================================
来源：http://ou.shtwfgs.cn

[G01] 定义类
来源：http://ve.hnjuh.cn

Py:   class User: pass
来源：http://gw.wgjwhj.cn

PHP:  class User {}
来源：http://dq.szxytkj.cn

JS:   class User {}
来源：http://yi.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://al.newstarts.cn

Java: class User {}
来源：http://de.9csxet.cn

Go:   type User struct { Name string }
来源：http://nj.colortex.cn

Ruby: class User; end
来源：http://tl.muxihuayi.cn

C#:   class User {}
来源：http://hl.jianghongdianzi.cn

[G02] 构造函数
来源：http://px.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://ir.muxihuayi.cn

PHP:  public function __construct(public string $name) {}
来源：http://ty.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://hr.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://yp.hahajie.cn

Java: User(String name) { this.name = name; }
来源：http://bi.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pm.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://aj.szxytkj.cn

C#:   public User(string name) { Name = name; }
来源：http://ge.newstarts.cn

[G03] 实例属性
来源：http://sa.nicolike.cn

Py:   self.name = "x"
来源：http://tg.hnjuh.cn

PHP:  public string $name = "x";
来源：http://hn.bookmarksfly.cn

JS:   this.name = "x";
来源：http://il.szsharing.cn

TS:   name: string = "x";
来源：http://mw.shtwfgs.cn

Java: private String name;
来源：http://pt.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://of.chemitech.net.cn

Ruby: @name = "x"
来源：http://wo.hahajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://ga.huanxung.cn

[G04] 定义方法
来源：http://kd.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://ht.gzmigu.cn


<!-- 参考信息 -->