代发 wailian999

C#:   s.Replace("a", "b")
来源：http://zh.szxytkj.cn

[E07] 按分隔符拆分
来源：http://kb.huanxung.cn

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://pz.shxzukj.cn

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://gw.shxzukj.cn

JS:   s.split(",");  s.split(/\s+/)
来源：http://yb.bookmarksfly.cn

TS:   s.split(",")
来源：http://zv.bookmarksfly.cn

Java: s.split(",");  s.split("\\s+")
来源：http://cs.szsharing.cn

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://gc.asd995.cn

Ruby: s.split(",");  s.split
来源：http://oi.haigaiapp.cn

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://jz.shxzskj.cn

[E08] 数组按分隔符合并
来源：http://pk.hnjuh.cn

Py:   ",".join(items)
来源：http://lr.hahajie.cn

PHP:  implode(",", $items);
来源：http://ra.bookmarksfly.cn

JS:   items.join(",")
来源：http://rs.jctech888.com.cn

TS:   items.join(",")
来源：http://we.yuexingan06.cn

Java: String.join(",", items)
来源：http://fi.shxzskj.cn

Go:   strings.Join(items, ",")
来源：http://ef.521024.cn

Ruby: items.join(",")
来源：http://tn.9csxet.cn

C#:   string.Join(",", items)
来源：http://wi.huixiangedu.cn

[E09] 去除所有空白字符
来源：http://my.jctech888.com.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://xo.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://bk.szxytkj.cn

JS:   s.replace(/\s+/g, "")
来源：http://ah.panjiajie.cn

TS:   s.replace(/\s+/g, "")
来源：http://cn.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://ax.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://hv.panjiajie.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kp.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wr.nicolike.cn

[E10] 左侧补零 / 定长填充
来源：http://du.bookmarksfly.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://um.gzmigu.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ol.jianghongdianzi.cn

JS:   "7".padStart(3, "0")
来源：http://dq.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://mw.jctech888.com.cn

Java: String.format("%03d", 7)
来源：http://re.jctech888.com.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://vt.nszjky.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://jz.wgjwhj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yq.huixiangedu.cn

[E11] 反转字符串
来源：http://dj.panjiajie.cn

Py:   s[::-1]
来源：http://xe.szsharing.cn

PHP:  strrev($s);
来源：http://qz.521024.cn

JS:   [...s].reverse().join("")
来源：http://bc.hahajie.cn

TS:   [...s].reverse().join("")
来源：http://rn.newstarts.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xd.nicolike.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xg.shtwfgs.cn

Ruby: s.reverse
来源：http://ot.jianghongdianzi.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sv.newstarts.cn

[E12] 统计某字符出现次数
来源：http://wi.jianghongdianzi.cn

Py:   s.count("a")
来源：http://fl.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://nh.colortex.cn

JS:   s.split("a").length - 1
来源：http://qa.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://re.shtwfgs.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ju.bookmarksfly.cn

Go:   strings.Count(s, "a")
来源：http://jh.lnxyls.cn

Ruby: s.count("a")
来源：http://vc.521024.cn

C#:   s.Count(c => c == 'a')
来源：http://lp.lnxyls.cn

[E13] 逐字符遍历
来源：http://gz.yuntaijiaju.cn

Py:   for ch in s: print(ch)
来源：http://dk.jctech888.com.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://am.chemitech.net.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://lz.panjiajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lf.jianghongdianzi.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://em.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://eq.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://cv.muxihuayi.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://xt.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://lx.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ng.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://dx.chemitech.net.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://gs.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://lw.panjiajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://nb.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://nm.9csxet.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://to.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://sc.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://js.yuexingan06.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qf.bookmarksfly.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ys.521024.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ns.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://to.jianghongdianzi.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://cm.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wc.jianghongdianzi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wl.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tr.panjiajie.cn

[E16] 数字千分位
来源：http://fg.hahajie.cn

Py:   f"{1234567:,}"
来源：http://yj.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://mw.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://xt.hnjuh.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://eq.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://da.521024.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xe.colortex.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oh.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://jo.haigaiapp.cn

[E17] 首字母大写
来源：http://wl.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sn.hnjuh.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://nt.shxzskj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ry.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pg.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ba.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sx.shxzskj.cn

Ruby: s.capitalize
来源：http://sq.hahajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bh.9csxet.cn

[E18] 模板占位符替换
来源：http://zl.nszjky.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bl.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://br.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://re.panjiajie.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://sj.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oo.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://bw.nszjky.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hc.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://xx.nicolike.cn

[E19] 多行文本按行拆分
来源：http://cm.nszjky.cn

Py:   s.splitlines()
来源：http://jo.jctech888.com.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tk.shxzukj.cn

JS:   s.split(/\r?\n/)
来源：http://lx.chemitech.net.cn

TS:   s.split(/\r?\n/)
来源：http://vb.hnjuh.cn

Java: s.lines().toList()
来源：http://iq.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://dw.huanxung.cn

Ruby: s.lines
来源：http://qc.yuexingan06.cn

C#:   s.Split('\n')
来源：http://sh.shxzskj.cn

[E20] 判断字符串是否为空
来源：http://ox.panjiajie.cn

Py:   if not s:
来源：http://zg.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://jn.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dc.haigaiapp.cn

TS:   if (s === "") {}
来源：http://kn.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://iz.yuexingan06.cn

Go:   if s == "" {}
来源：http://zu.shxzukj.cn

Ruby: if s.empty?
来源：http://ap.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://oc.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://zu.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ox.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ok.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://tk.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sy.jianghongdianzi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ky.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://ay.shtwfgs.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://du.colortex.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gq.asd995.cn

[E22] 字节长度与字符长度
来源：http://ye.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://pq.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://xz.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kf.gzmigu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nk.shxzskj.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wv.gzmigu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dm.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://at.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yl.hahajie.cn

================================================================================
来源：http://cw.bjjhwx.cn

F. 文件与目录
来源：http://lb.nszjky.cn

================================================================================
来源：http://kq.bookmarksfly.cn

[F01] 读取整个文件
来源：http://un.huixinmuqiang.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rw.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://gh.huixinmuqiang.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ny.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://cw.bookmarksfly.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fh.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rm.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://in.jctech888.com.cn

C#:   File.ReadAllText("a.txt");
来源：http://fu.hnjuh.cn

[F02] 逐行读取文件
来源：http://kr.hnjuh.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://rl.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ju.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hn.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fk.shxzukj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cs.9csxet.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vj.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qb.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bt.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://ro.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://dj.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ko.shtwfgs.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://do.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jg.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mz.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://rt.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://vx.shxzukj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ml.lnxyls.cn

[F04] 追加写入文件
来源：http://ua.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jo.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xy.521024.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://sb.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ut.shxzukj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ng.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ks.nszjky.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://aj.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://qv.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://hy.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sn.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://jm.chemitech.net.cn

JS:   fs.existsSync("a.txt")
来源：http://vc.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ks.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sy.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cz.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://wb.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://au.yuntaijiaju.cn

[F06] 删除文件
来源：http://xk.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://mc.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ih.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://yb.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dv.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ix.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://if.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://sk.haigaiapp.cn

C#:   File.Delete("a.txt");
来源：http://no.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://nc.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bi.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jz.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zr.haigaiapp.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gz.nicolike.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://nn.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://fv.jianghongdianzi.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rg.asd995.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://yc.colortex.cn

[F08] 遍历目录
来源：http://or.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vq.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mt.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://pg.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://on.wgjwhj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qg.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://dw.asd995.cn

Ruby: Dir.children("dir")
来源：http://fk.huanxung.cn

C#:   Directory.GetFiles("dir")
来源：http://of.huixiangedu.cn

[F09] 获取文件大小
来源：http://gm.jianghongdianzi.cn

Py:   os.path.getsize("a.txt")
来源：http://ju.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://ae.panjiajie.cn

JS:   fs.statSync("a.txt").size
来源：http://lg.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://on.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lp.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zo.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://nl.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://xd.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://gv.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://fn.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tq.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://uw.hahajie.cn

TS:   path.extname("a.txt")
来源：http://zn.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://jv.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ym.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dn.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://cm.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://df.hnjuh.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dc.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vw.colortex.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://in.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wi.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wx.nicolike.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mi.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kq.shxzukj.cn

[F12] CSV 读写
来源：http://wi.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qr.shxzskj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mb.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xs.bjjhwx.cn

TS:   // 同上
来源：http://cl.jianghongdianzi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mj.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hm.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fe.lnxyls.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ut.shtwfgs.cn

================================================================================
来源：http://jz.szxytkj.cn

G. 面向对象
来源：http://ox.szsharing.cn

================================================================================
来源：http://ug.huanxung.cn

[G01] 定义类
来源：http://xi.hahajie.cn

Py:   class User: pass
来源：http://li.shtwfgs.cn

PHP:  class User {}
来源：http://gi.9csxet.cn

JS:   class User {}
来源：http://hf.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ij.huanxung.cn

Java: class User {}
来源：http://el.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://dm.szsharing.cn

Ruby: class User; end
来源：http://hm.bjjhwx.cn

C#:   class User {}
来源：http://tl.hahajie.cn

[G02] 构造函数
来源：http://us.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://am.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://tq.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://jz.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://zr.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://zw.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wj.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://aq.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://vs.szsharing.cn

[G03] 实例属性
来源：http://ai.nicolike.cn

Py:   self.name = "x"
来源：http://ys.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://re.muxihuayi.cn

JS:   this.name = "x";
来源：http://pk.panjiajie.cn

TS:   name: string = "x";
来源：http://iz.szsharing.cn

Java: private String name;
来源：http://ia.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lu.haigaiapp.cn

Ruby: @name = "x"
来源：http://aj.szxytkj.cn

C#:   public string Name { get; set; } = "x";
来源：http://mp.gzmigu.cn

[G04] 定义方法
来源：http://bx.huanxung.cn

Py:   def greet(self): return self.name
来源：http://dz.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pp.9csxet.cn

JS:   greet() { return this.name; }
来源：http://yi.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://sl.chemitech.net.cn

Java: String greet() { return name; }
来源：http://le.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://uy.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://kk.521024.cn

C#:   public string Greet() => Name;
来源：http://mr.szxytkj.cn

[G05] 继承
来源：http://dc.szxytkj.cn

Py:   class Admin(User): pass
来源：http://fw.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://qa.nicolike.cn

JS:   class Admin extends User {}
来源：http://pw.panjiajie.cn

TS:   class Admin extends User {}
来源：http://tw.jctech888.com.cn


<!-- 参考信息 -->