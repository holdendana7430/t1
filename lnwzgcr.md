代发 wailian999

PHP:  implode(",", $items);
来源：http://ns.shxzskj.cn

JS:   items.join(",")
来源：http://kk.shxzskj.cn

TS:   items.join(",")
来源：http://au.szxytkj.cn

Java: String.join(",", items)
来源：http://oy.bjjhwx.cn

Go:   strings.Join(items, ",")
来源：http://no.asd995.cn

Ruby: items.join(",")
来源：http://mi.jctech888.com.cn

C#:   string.Join(",", items)
来源：http://hw.yuntaijiaju.cn

[E09] 去除所有空白字符
来源：http://vz.hahajie.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://yv.jctech888.com.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://fu.huanxung.cn

JS:   s.replace(/\s+/g, "")
来源：http://oc.shxzskj.cn

TS:   s.replace(/\s+/g, "")
来源：http://ug.huanxung.cn

Java: s.replaceAll("\\s+", "")
来源：http://uy.521024.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://dg.haigaiapp.cn

Ruby: s.gsub(/\s+/, "")
来源：http://rl.chemitech.net.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ic.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://ze.szsharing.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wo.bookmarksfly.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://lb.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://ts.jianghongdianzi.cn

TS:   "7".padStart(3, "0")
来源：http://ww.szsharing.cn

Java: String.format("%03d", 7)
来源：http://qa.hahajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://kh.huanxung.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://tp.shtwfgs.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://fd.hnjuh.cn

[E11] 反转字符串
来源：http://eg.gzmigu.cn

Py:   s[::-1]
来源：http://yt.huixiangedu.cn

PHP:  strrev($s);
来源：http://sv.shxzukj.cn

JS:   [...s].reverse().join("")
来源：http://jm.huixinmuqiang.cn

TS:   [...s].reverse().join("")
来源：http://ms.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://pg.shtwfgs.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://hd.shxzukj.cn

Ruby: s.reverse
来源：http://pt.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://jh.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://xn.asd995.cn

Py:   s.count("a")
来源：http://eq.bookmarksfly.cn

PHP:  substr_count($s, "a");
来源：http://fc.wgjwhj.cn

JS:   s.split("a").length - 1
来源：http://vp.yuntaijiaju.cn

TS:   s.split("a").length - 1
来源：http://ms.szxytkj.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://sb.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://ck.shxzukj.cn

Ruby: s.count("a")
来源：http://hv.huixinmuqiang.cn

C#:   s.Count(c => c == 'a')
来源：http://gl.shxzukj.cn

[E13] 逐字符遍历
来源：http://ef.hahajie.cn

Py:   for ch in s: print(ch)
来源：http://ua.huanxung.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://pq.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ju.shtwfgs.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://oy.lnxyls.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://ce.gzmigu.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://px.asd995.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ch.shxzskj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sj.bjjhwx.cn

[E14] URL 编码与 Base64
来源：http://ca.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hk.hahajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://yc.bookmarksfly.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://by.bjjhwx.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://fr.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://gh.szsharing.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://jo.nicolike.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ku.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nd.jianghongdianzi.cn

[E15] HTML 转义 / 反转义
来源：http://bd.jianghongdianzi.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://od.hahajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ip.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://ip.jctech888.com.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://jj.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://qq.521024.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://qi.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://rh.hnjuh.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://tb.yuexingan06.cn

[E16] 数字千分位
来源：http://ew.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://er.yuexingan06.cn

PHP:  number_format(1234567);
来源：http://py.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dd.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qz.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://fb.asd995.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sj.asd995.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cp.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://bz.521024.cn

[E17] 首字母大写
来源：http://cm.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://po.lnxyls.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://fa.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tz.gzmigu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://uf.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://vb.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zu.muxihuayi.cn

Ruby: s.capitalize
来源：http://jt.bookmarksfly.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ul.asd995.cn

[E18] 模板占位符替换
来源：http://wc.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://in.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hp.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ty.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jk.szxytkj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://bi.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://up.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bu.yuexingan06.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://sc.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://mv.hnjuh.cn

Py:   s.splitlines()
来源：http://tp.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://qz.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://cr.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://ns.nszjky.cn

Java: s.lines().toList()
来源：http://rf.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://aa.huanxung.cn

Ruby: s.lines
来源：http://wt.bjjhwx.cn

C#:   s.Split('\n')
来源：http://mu.colortex.cn

[E20] 判断字符串是否为空
来源：http://jh.shxzukj.cn

Py:   if not s:
来源：http://jj.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gr.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ov.jctech888.com.cn

TS:   if (s === "") {}
来源：http://ih.9csxet.cn

Java: if (s.isEmpty()) {}
来源：http://kx.9csxet.cn

Go:   if s == "" {}
来源：http://tx.szxytkj.cn

Ruby: if s.empty?
来源：http://hs.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://tr.haigaiapp.cn

[E21] 超长截断加省略号
来源：http://em.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ju.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://dp.shxzskj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rg.muxihuayi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ol.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://vg.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://bn.yuntaijiaju.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xe.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gk.panjiajie.cn

[E22] 字节长度与字符长度
来源：http://xw.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://gf.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hp.521024.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://sz.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lv.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zm.nszjky.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ki.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://bt.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ev.panjiajie.cn

================================================================================
来源：http://xx.jctech888.com.cn

F. 文件与目录
来源：http://fg.newstarts.cn

================================================================================
来源：http://dr.szsharing.cn

[F01] 读取整个文件
来源：http://pj.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wl.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://gs.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vm.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://rx.haigaiapp.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sg.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mk.gzmigu.cn

Ruby: File.read("a.txt")
来源：http://bj.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://dz.shtwfgs.cn

[F02] 逐行读取文件
来源：http://vo.szxytkj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://on.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://um.muxihuayi.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sv.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xs.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ct.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://km.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zc.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rg.521024.cn

[F03] 写入文件（覆盖）
来源：http://pg.haigaiapp.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://go.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pc.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wg.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jn.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://sr.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://yw.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://of.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pw.lnxyls.cn

[F04] 追加写入文件
来源：http://xw.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://en.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mx.panjiajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zn.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zs.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vp.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tn.muxihuayi.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pp.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zh.bookmarksfly.cn

[F05] 判断文件或目录是否存在
来源：http://eb.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://oe.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://um.asd995.cn

JS:   fs.existsSync("a.txt")
来源：http://bj.huixinmuqiang.cn

TS:   fs.existsSync("a.txt")
来源：http://qa.9csxet.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ns.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ub.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://rc.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://lq.shtwfgs.cn

[F06] 删除文件
来源：http://kn.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://oa.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://gu.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nd.hnjuh.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dv.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://iz.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://hb.huixiangedu.cn

Ruby: File.delete("a.txt")
来源：http://dl.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://gd.shtwfgs.cn

[F07] 创建目录（含多级）
来源：http://ns.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://qc.hahajie.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ka.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hg.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yo.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fl.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jo.newstarts.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://iw.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gm.wgjwhj.cn

[F08] 遍历目录
来源：http://po.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ag.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lp.asd995.cn

JS:   fs.readdirSync("dir")
来源：http://ys.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://yj.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://se.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ec.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://gr.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://kk.szxytkj.cn

[F09] 获取文件大小
来源：http://hn.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://xf.szsharing.cn

PHP:  filesize("a.txt");
来源：http://vo.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ob.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://zy.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nk.haigaiapp.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kz.9csxet.cn

Ruby: File.size("a.txt")
来源：http://pb.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://yv.szxytkj.cn

[F10] 取文件扩展名 / 文件名
来源：http://uf.huixiangedu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gd.newstarts.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fw.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://rj.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ja.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://so.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ch.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fc.bookmarksfly.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ri.huixinmuqiang.cn

[F11] 复制与移动文件
来源：http://nw.yuexingan06.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qk.wgjwhj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vy.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yg.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jc.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://yt.521024.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://uq.yuntaijiaju.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://dl.shtwfgs.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://fd.shxzukj.cn

[F12] CSV 读写
来源：http://id.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jv.huixiangedu.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://fg.nszjky.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ph.shtwfgs.cn

TS:   // 同上
来源：http://mr.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ww.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fs.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pv.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://xw.521024.cn

================================================================================
来源：http://ry.9csxet.cn

G. 面向对象
来源：http://dt.huixiangedu.cn

================================================================================
来源：http://lr.huixinmuqiang.cn

[G01] 定义类
来源：http://oo.lnxyls.cn

Py:   class User: pass
来源：http://ac.panjiajie.cn

PHP:  class User {}
来源：http://bj.nicolike.cn

JS:   class User {}
来源：http://zp.asd995.cn

TS:   class User { name: string = ""; }
来源：http://dq.huanxung.cn

Java: class User {}
来源：http://jp.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://zz.nszjky.cn

Ruby: class User; end
来源：http://xz.asd995.cn

C#:   class User {}
来源：http://mr.asd995.cn

[G02] 构造函数
来源：http://qz.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://ni.shxzskj.cn

PHP:  public function __construct(public string $name) {}
来源：http://qq.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://tw.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://ur.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://fl.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wx.jctech888.com.cn

Ruby: def initialize(name); @name = name; end
来源：http://ib.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ju.yuntaijiaju.cn

[G03] 实例属性
来源：http://dd.yuexingan06.cn

Py:   self.name = "x"
来源：http://uo.shxzukj.cn

PHP:  public string $name = "x";
来源：http://so.asd995.cn

JS:   this.name = "x";
来源：http://vt.colortex.cn

TS:   name: string = "x";
来源：http://sg.muxihuayi.cn

Java: private String name;
来源：http://js.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gk.shxzskj.cn

Ruby: @name = "x"
来源：http://nj.bookmarksfly.cn

C#:   public string Name { get; set; } = "x";
来源：http://rc.hahajie.cn

[G04] 定义方法
来源：http://gj.chemitech.net.cn

Py:   def greet(self): return self.name
来源：http://yh.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gx.huanxung.cn

JS:   greet() { return this.name; }
来源：http://go.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://qt.521024.cn

Java: String greet() { return name; }
来源：http://hd.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://gs.panjiajie.cn

Ruby: def greet; @name; end
来源：http://ah.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://oc.wgjwhj.cn

[G05] 继承
来源：http://cf.shxzukj.cn

Py:   class Admin(User): pass
来源：http://xb.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://mt.jianghongdianzi.cn

JS:   class Admin extends User {}
来源：http://md.yuexingan06.cn

TS:   class Admin extends User {}
来源：http://jz.hnjuh.cn

Java: class Admin extends User {}
来源：http://gz.gzmigu.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rz.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://pc.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://ro.panjiajie.cn

[G06] 重写方法
来源：http://xm.colortex.cn

Py:   def greet(self): return "admin"
来源：http://hp.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jt.wgjwhj.cn

JS:   greet() { return "admin"; }
来源：http://fw.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://kr.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://rg.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rm.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://ts.hnjuh.cn


<!-- 参考信息 -->