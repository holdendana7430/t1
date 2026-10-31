代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://dd.newstarts.cn

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://ey.yuexingan06.cn

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://bc.jianghongdianzi.cn

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://dl.huixiangedu.cn

[E06] 替换子串
来源：http://nj.nicolike.cn

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://la.chemitech.net.cn

PHP:  str_replace("a", "b", $s);
来源：http://gf.szsharing.cn

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://qr.panjiajie.cn

TS:   s.replaceAll("a", "b")
来源：http://sa.muxihuayi.cn

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://tz.nicolike.cn

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://zb.colortex.cn

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://xq.nicolike.cn

C#:   s.Replace("a", "b")
来源：http://xe.huixiangedu.cn

[E07] 按分隔符拆分
来源：http://fs.haigaiapp.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pc.nszjky.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://va.hnjuh.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://fa.wgjwhj.cn

TS:   s.split(",")
来源：http://wd.panjiajie.cn

Java: s.split(",");  s.split("\\s+")
来源：http://hf.wgjwhj.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gm.wgjwhj.cn

Ruby: s.split(",");  s.split
来源：http://qm.gzmigu.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://vy.shtwfgs.cn

[E08] 数组按分隔符合并
来源：http://kd.lnxyls.cn

Py:   ",".join(items)
来源：http://xv.szxytkj.cn

PHP:  implode(",", $items);
来源：http://pj.szsharing.cn

JS:   items.join(",")
来源：http://ih.szxytkj.cn

TS:   items.join(",")
来源：http://jl.shtwfgs.cn

Java: String.join(",", items)
来源：http://om.hahajie.cn

Go:   strings.Join(items, ",")
来源：http://sx.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://mr.huixiangedu.cn

C#:   string.Join(",", items)
来源：http://xo.haigaiapp.cn

[E09] 去除所有空白字符
来源：http://va.szsharing.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://bo.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://ub.gzmigu.cn

JS:   s.replace(/\s+/g, "")
来源：http://lp.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://wo.panjiajie.cn

Java: s.replaceAll("\\s+", "")
来源：http://xv.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://yy.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rr.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://en.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://ym.bjjhwx.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ce.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jx.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://ka.jctech888.com.cn

TS:   "7".padStart(3, "0")
来源：http://hh.huixinmuqiang.cn

Java: String.format("%03d", 7)
来源：http://kw.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://ne.chemitech.net.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://nd.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rr.lnxyls.cn

[E11] 反转字符串
来源：http://ui.huanxung.cn

Py:   s[::-1]
来源：http://qj.szsharing.cn

PHP:  strrev($s);
来源：http://io.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://qx.jctech888.com.cn

TS:   [...s].reverse().join("")
来源：http://co.muxihuayi.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://yk.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://lw.jctech888.com.cn

Ruby: s.reverse
来源：http://od.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://mx.wgjwhj.cn

[E12] 统计某字符出现次数
来源：http://lq.hnjuh.cn

Py:   s.count("a")
来源：http://rd.jctech888.com.cn

PHP:  substr_count($s, "a");
来源：http://po.shxzukj.cn

JS:   s.split("a").length - 1
来源：http://mr.asd995.cn

TS:   s.split("a").length - 1
来源：http://sp.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hq.haigaiapp.cn

Go:   strings.Count(s, "a")
来源：http://mg.colortex.cn

Ruby: s.count("a")
来源：http://sl.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://yt.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://lr.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://lr.panjiajie.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bs.521024.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ra.huixinmuqiang.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ot.yuntaijiaju.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://si.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://iz.szxytkj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tp.szsharing.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://yz.nszjky.cn

[E14] URL 编码与 Base64
来源：http://yg.shtwfgs.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://sf.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jv.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hl.jianghongdianzi.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fh.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ad.nicolike.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://pu.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hk.szsharing.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://uh.shxzskj.cn

[E15] HTML 转义 / 反转义
来源：http://fs.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://bu.521024.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ne.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://bc.gzmigu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://hx.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ff.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ks.gzmigu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xt.wgjwhj.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vw.hahajie.cn

[E16] 数字千分位
来源：http://os.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://wx.newstarts.cn

PHP:  number_format(1234567);
来源：http://uu.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ze.wgjwhj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://fl.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hx.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://bw.newstarts.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xm.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://gl.bookmarksfly.cn

[E17] 首字母大写
来源：http://wp.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://fr.bookmarksfly.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rs.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://er.9csxet.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://nt.bookmarksfly.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://et.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://du.szsharing.cn

Ruby: s.capitalize
来源：http://hz.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ku.bjjhwx.cn

[E18] 模板占位符替换
来源：http://ei.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zc.yuexingan06.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://qa.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://vo.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ey.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://uf.nszjky.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://od.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://yk.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://de.9csxet.cn

[E19] 多行文本按行拆分
来源：http://db.hahajie.cn

Py:   s.splitlines()
来源：http://mj.bookmarksfly.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://th.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://kb.nicolike.cn

TS:   s.split(/\r?\n/)
来源：http://by.colortex.cn

Java: s.lines().toList()
来源：http://bx.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://sh.muxihuayi.cn

Ruby: s.lines
来源：http://vs.yuexingan06.cn

C#:   s.Split('\n')
来源：http://yz.shtwfgs.cn

[E20] 判断字符串是否为空
来源：http://ka.9csxet.cn

Py:   if not s:
来源：http://ca.haigaiapp.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://eh.szxytkj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://uz.colortex.cn

TS:   if (s === "") {}
来源：http://vu.haigaiapp.cn

Java: if (s.isEmpty()) {}
来源：http://nl.yuexingan06.cn

Go:   if s == "" {}
来源：http://yc.huixiangedu.cn

Ruby: if s.empty?
来源：http://mw.szsharing.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dq.shxzukj.cn

[E21] 超长截断加省略号
来源：http://uf.hnjuh.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://de.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://uz.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pt.huixinmuqiang.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ob.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://js.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://xl.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wy.lnxyls.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ep.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://pl.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wy.hnjuh.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ty.huanxung.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://je.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nz.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://sf.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bn.wgjwhj.cn

Ruby: s.bytesize;  s.length
来源：http://ah.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wx.yuntaijiaju.cn

================================================================================
来源：http://oh.jctech888.com.cn

F. 文件与目录
来源：http://wb.wgjwhj.cn

================================================================================
来源：http://cj.huanxung.cn

[F01] 读取整个文件
来源：http://mo.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wu.shxzukj.cn

PHP:  file_get_contents("a.txt");
来源：http://fd.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://su.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sl.newstarts.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://be.muxihuayi.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bv.9csxet.cn

Ruby: File.read("a.txt")
来源：http://gi.huixinmuqiang.cn

C#:   File.ReadAllText("a.txt");
来源：http://kd.hnjuh.cn

[F02] 逐行读取文件
来源：http://al.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://da.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qv.szxytkj.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://si.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ex.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ms.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ao.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://vp.bookmarksfly.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://vf.colortex.cn

[F03] 写入文件（覆盖）
来源：http://mf.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://zq.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://dt.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xa.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://uh.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ah.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fn.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://rr.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ki.hnjuh.cn

[F04] 追加写入文件
来源：http://gm.hahajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://cy.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zu.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pj.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jr.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lr.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eg.asd995.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://uf.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wg.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://aw.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://td.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://sx.shxzskj.cn

JS:   fs.existsSync("a.txt")
来源：http://vo.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://kp.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ck.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://nu.bjjhwx.cn

Ruby: File.exist?("a.txt")
来源：http://sz.colortex.cn

C#:   File.Exists("a.txt")
来源：http://mg.jianghongdianzi.cn

[F06] 删除文件
来源：http://hj.shxzskj.cn

Py:   os.remove("a.txt")
来源：http://gp.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://tl.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://li.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://hu.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yl.521024.cn

Go:   os.Remove("a.txt")
来源：http://op.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://pb.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://hy.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://vj.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fs.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://tf.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wa.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ps.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lz.huanxung.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ca.521024.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dz.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sy.chemitech.net.cn

[F08] 遍历目录
来源：http://yq.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ct.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lr.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://hs.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://ar.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rl.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ar.hnjuh.cn

Ruby: Dir.children("dir")
来源：http://gw.huixiangedu.cn

C#:   Directory.GetFiles("dir")
来源：http://bx.lnxyls.cn

[F09] 获取文件大小
来源：http://gl.nszjky.cn

Py:   os.path.getsize("a.txt")
来源：http://wh.521024.cn

PHP:  filesize("a.txt");
来源：http://qv.lnxyls.cn

JS:   fs.statSync("a.txt").size
来源：http://bo.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://ga.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wb.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://bm.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://it.wgjwhj.cn

C#:   new FileInfo("a.txt").Length
来源：http://xu.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://rl.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ft.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xc.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qe.asd995.cn

TS:   path.extname("a.txt")
来源：http://il.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://li.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://kg.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://it.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://el.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://nj.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://iy.szsharing.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sp.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ru.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vh.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ug.bookmarksfly.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yw.newstarts.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://fm.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://xq.shxzskj.cn

[F12] CSV 读写
来源：http://dx.shxzskj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gz.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zr.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://lt.hahajie.cn

TS:   // 同上
来源：http://wc.colortex.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cp.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ak.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zn.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://oz.hahajie.cn

================================================================================
来源：http://si.haigaiapp.cn

G. 面向对象
来源：http://mm.bjjhwx.cn

================================================================================
来源：http://oq.huixinmuqiang.cn

[G01] 定义类
来源：http://fl.nicolike.cn

Py:   class User: pass
来源：http://lu.lnxyls.cn

PHP:  class User {}
来源：http://zk.shxzskj.cn

JS:   class User {}
来源：http://sk.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://vt.panjiajie.cn

Java: class User {}
来源：http://wv.521024.cn

Go:   type User struct { Name string }
来源：http://se.huanxung.cn

Ruby: class User; end
来源：http://sg.nicolike.cn

C#:   class User {}
来源：http://xx.lnxyls.cn

[G02] 构造函数
来源：http://po.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://ev.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://nb.shtwfgs.cn

JS:   constructor(name) { this.name = name; }
来源：http://li.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://ki.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://dl.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nb.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://le.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ab.szsharing.cn

[G03] 实例属性
来源：http://xj.huanxung.cn

Py:   self.name = "x"
来源：http://lq.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://bh.shxzukj.cn

JS:   this.name = "x";
来源：http://hm.shxzukj.cn

TS:   name: string = "x";
来源：http://cv.hahajie.cn

Java: private String name;
来源：http://xn.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gh.muxihuayi.cn

Ruby: @name = "x"
来源：http://pf.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://lg.bookmarksfly.cn

[G04] 定义方法
来源：http://kn.shtwfgs.cn

Py:   def greet(self): return self.name
来源：http://kg.szsharing.cn


<!-- 参考信息 -->