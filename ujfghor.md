代发 wailian999

PHP:  implode(",", $items);
来源：http://fa.9csxet.cn

JS:   items.join(",")
来源：http://fg.newstarts.cn

TS:   items.join(",")
来源：http://ip.jctech888.com.cn

Java: String.join(",", items)
来源：http://fx.asd995.cn

Go:   strings.Join(items, ",")
来源：http://lp.yuntaijiaju.cn

Ruby: items.join(",")
来源：http://ee.gzmigu.cn

C#:   string.Join(",", items)
来源：http://tw.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://pt.haigaiapp.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://to.shxzukj.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://xc.shxzskj.cn

JS:   s.replace(/\s+/g, "")
来源：http://pf.szxytkj.cn

TS:   s.replace(/\s+/g, "")
来源：http://re.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://rh.yuexingan06.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://sz.nszjky.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ee.lnxyls.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://tk.chemitech.net.cn

[E10] 左侧补零 / 定长填充
来源：http://db.yuexingan06.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://zv.panjiajie.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://fd.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://fw.huanxung.cn

TS:   "7".padStart(3, "0")
来源：http://jw.huixiangedu.cn

Java: String.format("%03d", 7)
来源：http://hj.jianghongdianzi.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zw.bjjhwx.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sg.gzmigu.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wy.yuntaijiaju.cn

[E11] 反转字符串
来源：http://yt.bookmarksfly.cn

Py:   s[::-1]
来源：http://dq.wgjwhj.cn

PHP:  strrev($s);
来源：http://kd.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://yi.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://dn.bjjhwx.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ji.chemitech.net.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hj.asd995.cn

Ruby: s.reverse
来源：http://yg.szsharing.cn

C#:   new string(s.Reverse().ToArray())
来源：http://uz.huixinmuqiang.cn

[E12] 统计某字符出现次数
来源：http://bf.jctech888.com.cn

Py:   s.count("a")
来源：http://cg.szsharing.cn

PHP:  substr_count($s, "a");
来源：http://pp.nszjky.cn

JS:   s.split("a").length - 1
来源：http://te.muxihuayi.cn

TS:   s.split("a").length - 1
来源：http://gs.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://id.jctech888.com.cn

Go:   strings.Count(s, "a")
来源：http://nf.colortex.cn

Ruby: s.count("a")
来源：http://iz.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://xw.nicolike.cn

[E13] 逐字符遍历
来源：http://yx.huixinmuqiang.cn

Py:   for ch in s: print(ch)
来源：http://nc.yuexingan06.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://rl.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ce.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://bf.huixinmuqiang.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xf.bookmarksfly.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://fv.huixinmuqiang.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ge.szxytkj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://rc.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://jj.colortex.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hr.haigaiapp.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qq.wgjwhj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ve.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://zq.gzmigu.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hu.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://vb.gzmigu.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ye.newstarts.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://pj.nicolike.cn

[E15] HTML 转义 / 反转义
来源：http://dm.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://dj.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vo.haigaiapp.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kg.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ko.521024.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vv.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://yb.asd995.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://cn.hahajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zh.chemitech.net.cn

[E16] 数字千分位
来源：http://jh.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://py.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://it.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bj.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ri.haigaiapp.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://og.lnxyls.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ot.shxzukj.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wq.panjiajie.cn

C#:   1234567.ToString("N0")
来源：http://si.shtwfgs.cn

[E17] 首字母大写
来源：http://fl.yuexingan06.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://go.nszjky.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://jc.nicolike.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ve.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://um.nicolike.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://li.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://nm.wgjwhj.cn

Ruby: s.capitalize
来源：http://cg.huixinmuqiang.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yo.gzmigu.cn

[E18] 模板占位符替换
来源：http://ks.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vi.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vr.nicolike.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://xf.huanxung.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://af.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ns.panjiajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://se.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nx.huanxung.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://id.hahajie.cn

[E19] 多行文本按行拆分
来源：http://yd.haigaiapp.cn

Py:   s.splitlines()
来源：http://tb.9csxet.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qp.haigaiapp.cn

JS:   s.split(/\r?\n/)
来源：http://jv.newstarts.cn

TS:   s.split(/\r?\n/)
来源：http://sw.huixinmuqiang.cn

Java: s.lines().toList()
来源：http://mb.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://eg.521024.cn

Ruby: s.lines
来源：http://gw.muxihuayi.cn

C#:   s.Split('\n')
来源：http://tb.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://ly.hnjuh.cn

Py:   if not s:
来源：http://lc.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yh.521024.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ei.9csxet.cn

TS:   if (s === "") {}
来源：http://zt.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://pu.asd995.cn

Go:   if s == "" {}
来源：http://vo.huixinmuqiang.cn

Ruby: if s.empty?
来源：http://vf.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wk.huixinmuqiang.cn

[E21] 超长截断加省略号
来源：http://fa.bookmarksfly.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qb.shtwfgs.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qc.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ij.9csxet.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xp.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://rb.yuexingan06.cn

Go:   // 按 rune 判断长度后截断
来源：http://kg.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wz.haigaiapp.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://vp.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://ri.huixinmuqiang.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://zq.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.muxihuayi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://iq.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zc.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ht.hahajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pc.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://dj.chemitech.net.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gz.szxytkj.cn

================================================================================
来源：http://aq.nicolike.cn

F. 文件与目录
来源：http://hs.jctech888.com.cn

================================================================================
来源：http://ok.bjjhwx.cn

[F01] 读取整个文件
来源：http://sk.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://cw.jianghongdianzi.cn

PHP:  file_get_contents("a.txt");
来源：http://aq.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vg.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vz.gzmigu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pv.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://pz.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://hn.yuntaijiaju.cn

C#:   File.ReadAllText("a.txt");
来源：http://mx.bookmarksfly.cn

[F02] 逐行读取文件
来源：http://yv.nszjky.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://am.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://px.haigaiapp.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://oz.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://an.newstarts.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://xu.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://jt.shxzukj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wn.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lt.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://ph.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://da.haigaiapp.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://bt.haigaiapp.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sn.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gr.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lg.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ga.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://dv.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://zn.colortex.cn

[F04] 追加写入文件
来源：http://as.wgjwhj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mi.9csxet.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ae.asd995.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tq.shxzukj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nh.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pt.wgjwhj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ay.shtwfgs.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ui.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://gx.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://kd.shxzukj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wh.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://hc.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://ke.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://wz.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://nr.shtwfgs.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wx.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://xd.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://ed.newstarts.cn

[F06] 删除文件
来源：http://rv.haigaiapp.cn

Py:   os.remove("a.txt")
来源：http://lx.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://zs.hahajie.cn

JS:   fs.unlinkSync("a.txt")
来源：http://os.521024.cn

TS:   fs.unlinkSync("a.txt")
来源：http://re.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tk.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://if.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://jb.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://ld.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://kz.nszjky.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ep.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qn.yuexingan06.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://sa.gzmigu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://eq.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ow.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xo.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://od.nicolike.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sh.bookmarksfly.cn

[F08] 遍历目录
来源：http://rf.jctech888.com.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lk.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fs.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://qu.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://xq.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://py.asd995.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://sf.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://tr.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://yp.huanxung.cn

[F09] 获取文件大小
来源：http://qi.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ke.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://ze.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://nx.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://wd.hahajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://vr.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hq.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://cm.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://uo.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ln.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://sw.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ik.newstarts.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kn.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://pg.szsharing.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://yd.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ls.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dn.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://tr.shxzukj.cn

[F11] 复制与移动文件
来源：http://ez.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://er.nicolike.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dk.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kw.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lr.haigaiapp.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kn.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hn.shtwfgs.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://al.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fl.muxihuayi.cn

[F12] CSV 读写
来源：http://tz.jianghongdianzi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://kc.hahajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://dr.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qw.jctech888.com.cn

TS:   // 同上
来源：http://ex.shxzukj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zs.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://cw.szxytkj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://cv.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lg.yuexingan06.cn

================================================================================
来源：http://gl.bjjhwx.cn

G. 面向对象
来源：http://qw.yuntaijiaju.cn

================================================================================
来源：http://vg.hahajie.cn

[G01] 定义类
来源：http://ht.wgjwhj.cn

Py:   class User: pass
来源：http://yc.huixiangedu.cn

PHP:  class User {}
来源：http://re.521024.cn

JS:   class User {}
来源：http://ki.nszjky.cn

TS:   class User { name: string = ""; }
来源：http://tt.hnjuh.cn

Java: class User {}
来源：http://yu.szsharing.cn

Go:   type User struct { Name string }
来源：http://qt.huixinmuqiang.cn

Ruby: class User; end
来源：http://hh.jianghongdianzi.cn

C#:   class User {}
来源：http://vz.shxzskj.cn

[G02] 构造函数
来源：http://kg.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://sl.huixiangedu.cn

PHP:  public function __construct(public string $name) {}
来源：http://kt.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ld.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://ul.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://cw.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wm.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://hb.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://qk.yuexingan06.cn

[G03] 实例属性
来源：http://ce.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://pj.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://xj.chemitech.net.cn

JS:   this.name = "x";
来源：http://po.nicolike.cn

TS:   name: string = "x";
来源：http://dm.9csxet.cn

Java: private String name;
来源：http://uk.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kt.szxytkj.cn

Ruby: @name = "x"
来源：http://ha.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://tn.szsharing.cn

[G04] 定义方法
来源：http://bj.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://pv.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://xw.szsharing.cn

JS:   greet() { return this.name; }
来源：http://xc.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://ov.yuexingan06.cn

Java: String greet() { return name; }
来源：http://sd.9csxet.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ql.shxzukj.cn

Ruby: def greet; @name; end
来源：http://nr.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://mc.yuntaijiaju.cn

[G05] 继承
来源：http://gc.szsharing.cn

Py:   class Admin(User): pass
来源：http://yw.colortex.cn

PHP:  class Admin extends User {}
来源：http://uz.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://um.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://qh.yuexingan06.cn

Java: class Admin extends User {}
来源：http://br.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ti.9csxet.cn

Ruby: class Admin < User; end
来源：http://ch.bjjhwx.cn

C#:   class Admin : User {}
来源：http://fd.panjiajie.cn

[G06] 重写方法
来源：http://tt.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://pw.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://na.szsharing.cn

JS:   greet() { return "admin"; }
来源：http://sr.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://lg.yuntaijiaju.cn

Java: @Override String greet() { return "admin"; }
来源：http://an.szsharing.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ou.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://in.yuexingan06.cn


<!-- 参考信息 -->