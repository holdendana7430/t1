代发 wailian999

Go:   strings.Join(items, ",")
来源：http://hm.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://nv.huixinmuqiang.cn

C#:   string.Join(",", items)
来源：http://gp.newstarts.cn

[E09] 去除所有空白字符
来源：http://pf.huixiangedu.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mz.huixiangedu.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wc.wgjwhj.cn

JS:   s.replace(/\s+/g, "")
来源：http://uo.szsharing.cn

TS:   s.replace(/\s+/g, "")
来源：http://ji.9csxet.cn

Java: s.replaceAll("\\s+", "")
来源：http://ex.shtwfgs.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://rz.nicolike.cn

Ruby: s.gsub(/\s+/, "")
来源：http://lw.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://nb.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://jx.colortex.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ia.huixinmuqiang.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://qe.gzmigu.cn

JS:   "7".padStart(3, "0")
来源：http://bw.newstarts.cn

TS:   "7".padStart(3, "0")
来源：http://mj.9csxet.cn

Java: String.format("%03d", 7)
来源：http://hl.muxihuayi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://qb.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cl.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://bn.szsharing.cn

[E11] 反转字符串
来源：http://tj.521024.cn

Py:   s[::-1]
来源：http://hp.hnjuh.cn

PHP:  strrev($s);
来源：http://qx.chemitech.net.cn

JS:   [...s].reverse().join("")
来源：http://hc.muxihuayi.cn

TS:   [...s].reverse().join("")
来源：http://uf.colortex.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://nn.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xw.nszjky.cn

Ruby: s.reverse
来源：http://dn.bjjhwx.cn

C#:   new string(s.Reverse().ToArray())
来源：http://iw.nicolike.cn

[E12] 统计某字符出现次数
来源：http://uk.muxihuayi.cn

Py:   s.count("a")
来源：http://gr.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://js.haigaiapp.cn

JS:   s.split("a").length - 1
来源：http://po.bookmarksfly.cn

TS:   s.split("a").length - 1
来源：http://df.hnjuh.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ye.lnxyls.cn

Go:   strings.Count(s, "a")
来源：http://en.9csxet.cn

Ruby: s.count("a")
来源：http://kz.shxzukj.cn

C#:   s.Count(c => c == 'a')
来源：http://pl.huixinmuqiang.cn

[E13] 逐字符遍历
来源：http://uw.bookmarksfly.cn

Py:   for ch in s: print(ch)
来源：http://dl.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rk.haigaiapp.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://nf.lnxyls.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://sk.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://gc.hnjuh.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ff.yuntaijiaju.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://qp.yuntaijiaju.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ls.521024.cn

[E14] URL 编码与 Base64
来源：http://ha.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://so.huanxung.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yd.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://qs.lnxyls.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://rh.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://id.yuexingan06.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yx.jianghongdianzi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hu.521024.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://fg.asd995.cn

[E15] HTML 转义 / 反转义
来源：http://ep.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pv.9csxet.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jl.gzmigu.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://op.szsharing.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://of.colortex.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qr.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xv.9csxet.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tr.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://er.lnxyls.cn

[E16] 数字千分位
来源：http://iz.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://en.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://da.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://eb.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://bs.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://dy.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mu.huixinmuqiang.cn

C#:   1234567.ToString("N0")
来源：http://ny.nszjky.cn

[E17] 首字母大写
来源：http://uw.bookmarksfly.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://gy.yuntaijiaju.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yr.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mo.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ul.colortex.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ft.huixiangedu.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://rh.nszjky.cn

Ruby: s.capitalize
来源：http://ym.yuntaijiaju.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://rx.panjiajie.cn

[E18] 模板占位符替换
来源：http://fv.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://zp.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pd.wgjwhj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wl.muxihuayi.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rn.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://zr.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://sg.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://sc.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://qa.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://kz.hnjuh.cn

Py:   s.splitlines()
来源：http://fa.shtwfgs.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://tl.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://lq.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://qe.nszjky.cn

Java: s.lines().toList()
来源：http://jj.hnjuh.cn

Go:   strings.Split(s, "\n")
来源：http://vq.9csxet.cn

Ruby: s.lines
来源：http://ol.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://wm.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://ri.huixiangedu.cn

Py:   if not s:
来源：http://iu.yuexingan06.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://fj.nszjky.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://do.gzmigu.cn

TS:   if (s === "") {}
来源：http://cp.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://di.hnjuh.cn

Go:   if s == "" {}
来源：http://os.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://kk.hnjuh.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hd.asd995.cn

[E21] 超长截断加省略号
来源：http://vc.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://tb.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wx.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dk.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fk.asd995.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fb.lnxyls.cn

Go:   // 按 rune 判断长度后截断
来源：http://aq.newstarts.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mg.wgjwhj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://rw.521024.cn

[E22] 字节长度与字符长度
来源：http://tg.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qm.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hb.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xg.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://bo.lnxyls.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wa.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pv.hahajie.cn

Ruby: s.bytesize;  s.length
来源：http://co.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ey.jianghongdianzi.cn

================================================================================
来源：http://it.asd995.cn

F. 文件与目录
来源：http://pc.huanxung.cn

================================================================================
来源：http://os.shxzskj.cn

[F01] 读取整个文件
来源：http://ah.bjjhwx.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://yc.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://uk.huanxung.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://im.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jz.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://mw.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://am.huanxung.cn

Ruby: File.read("a.txt")
来源：http://qq.nicolike.cn

C#:   File.ReadAllText("a.txt");
来源：http://pq.jctech888.com.cn

[F02] 逐行读取文件
来源：http://oh.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mn.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yq.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://iu.wgjwhj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ko.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://al.szxytkj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://is.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qe.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lk.haigaiapp.cn

[F03] 写入文件（覆盖）
来源：http://hw.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mh.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://zb.nicolike.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pn.bjjhwx.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xv.huixinmuqiang.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://es.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://of.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://cp.newstarts.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gu.szxytkj.cn

[F04] 追加写入文件
来源：http://id.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://eu.521024.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://jc.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ja.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zv.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vt.huanxung.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ml.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qz.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pp.yuntaijiaju.cn

[F05] 判断文件或目录是否存在
来源：http://gh.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ug.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://pp.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://qw.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://xr.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ea.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fw.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://nd.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://go.muxihuayi.cn

[F06] 删除文件
来源：http://hf.colortex.cn

Py:   os.remove("a.txt")
来源：http://gj.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ud.jianghongdianzi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ez.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://aw.bookmarksfly.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cc.jianghongdianzi.cn

Go:   os.Remove("a.txt")
来源：http://ki.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://ry.szxytkj.cn

C#:   File.Delete("a.txt");
来源：http://qj.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://su.panjiajie.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gj.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ee.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jj.muxihuayi.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://di.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uy.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vj.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://og.yuexingan06.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://fl.muxihuayi.cn

[F08] 遍历目录
来源：http://mx.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wl.521024.cn

JS:   fs.readdirSync("dir")
来源：http://es.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://hg.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://rd.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ih.colortex.cn

Ruby: Dir.children("dir")
来源：http://ku.gzmigu.cn

C#:   Directory.GetFiles("dir")
来源：http://rx.muxihuayi.cn

[F09] 获取文件大小
来源：http://tf.colortex.cn

Py:   os.path.getsize("a.txt")
来源：http://bt.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://wh.jctech888.com.cn

JS:   fs.statSync("a.txt").size
来源：http://wv.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://mu.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vf.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ip.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://rs.hnjuh.cn

C#:   new FileInfo("a.txt").Length
来源：http://sa.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://hs.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://rh.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://vn.panjiajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://no.nszjky.cn

TS:   path.extname("a.txt")
来源：http://wo.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xx.gzmigu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yt.colortex.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://vu.szsharing.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://fm.lnxyls.cn

[F11] 复制与移动文件
来源：http://rh.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://xe.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://td.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ih.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vq.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fo.chemitech.net.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zy.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://iw.9csxet.cn

[F12] CSV 读写
来源：http://ot.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nm.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://up.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://gz.hahajie.cn

TS:   // 同上
来源：http://cc.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://us.yuntaijiaju.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bm.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ub.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lh.szsharing.cn

================================================================================
来源：http://ia.szxytkj.cn

G. 面向对象
来源：http://qx.wgjwhj.cn

================================================================================
来源：http://nu.bjjhwx.cn

[G01] 定义类
来源：http://ft.nicolike.cn

Py:   class User: pass
来源：http://tp.521024.cn

PHP:  class User {}
来源：http://lp.521024.cn

JS:   class User {}
来源：http://yt.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://nq.asd995.cn

Java: class User {}
来源：http://ig.gzmigu.cn

Go:   type User struct { Name string }
来源：http://ox.jctech888.com.cn

Ruby: class User; end
来源：http://bp.newstarts.cn

C#:   class User {}
来源：http://cw.bjjhwx.cn

[G02] 构造函数
来源：http://xg.shxzukj.cn

Py:   def __init__(self, name): self.name = name
来源：http://wq.shtwfgs.cn

PHP:  public function __construct(public string $name) {}
来源：http://bb.9csxet.cn

JS:   constructor(name) { this.name = name; }
来源：http://kw.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://of.newstarts.cn

Java: User(String name) { this.name = name; }
来源：http://hd.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://zy.haigaiapp.cn

Ruby: def initialize(name); @name = name; end
来源：http://na.shtwfgs.cn

C#:   public User(string name) { Name = name; }
来源：http://zt.jianghongdianzi.cn

[G03] 实例属性
来源：http://bh.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://ay.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://el.haigaiapp.cn

JS:   this.name = "x";
来源：http://zu.yuntaijiaju.cn

TS:   name: string = "x";
来源：http://sl.asd995.cn

Java: private String name;
来源：http://xz.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sk.szxytkj.cn

Ruby: @name = "x"
来源：http://ml.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://bt.yuexingan06.cn

[G04] 定义方法
来源：http://jd.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://vo.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ia.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://qp.shxzskj.cn

TS:   greet(): string { return this.name; }
来源：http://jt.panjiajie.cn

Java: String greet() { return name; }
来源：http://gv.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xw.asd995.cn

Ruby: def greet; @name; end
来源：http://ux.newstarts.cn

C#:   public string Greet() => Name;
来源：http://vz.yuexingan06.cn

[G05] 继承
来源：http://ev.newstarts.cn

Py:   class Admin(User): pass
来源：http://gf.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://wh.gzmigu.cn

JS:   class Admin extends User {}
来源：http://lo.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://nm.nszjky.cn

Java: class Admin extends User {}
来源：http://vg.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lj.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://bc.shxzukj.cn

C#:   class Admin : User {}
来源：http://ca.muxihuayi.cn

[G06] 重写方法
来源：http://ft.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://dr.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://oi.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://tw.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://hs.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://cd.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://al.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ry.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://fq.shxzskj.cn

[G07] 调用父类方法
来源：http://pj.hahajie.cn

Py:   super().greet()
来源：http://nf.colortex.cn

PHP:  parent::greet();
来源：http://br.9csxet.cn


<!-- 参考信息 -->