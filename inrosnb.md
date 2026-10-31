代发 wailian999

PHP:  implode(",", $items);
来源：http://ob.chemitech.net.cn

JS:   items.join(",")
来源：http://dn.hahajie.cn

TS:   items.join(",")
来源：http://he.muxihuayi.cn

Java: String.join(",", items)
来源：http://ok.lnxyls.cn

Go:   strings.Join(items, ",")
来源：http://ij.jianghongdianzi.cn

Ruby: items.join(",")
来源：http://cr.nicolike.cn

C#:   string.Join(",", items)
来源：http://bg.hnjuh.cn

[E09] 去除所有空白字符
来源：http://rn.bookmarksfly.cn

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://pq.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://di.521024.cn

JS:   s.replace(/\s+/g, "")
来源：http://qr.yuntaijiaju.cn

TS:   s.replace(/\s+/g, "")
来源：http://hq.shtwfgs.cn

Java: s.replaceAll("\\s+", "")
来源：http://ot.szxytkj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://va.asd995.cn

Ruby: s.gsub(/\s+/, "")
来源：http://xa.bookmarksfly.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://ft.szxytkj.cn

[E10] 左侧补零 / 定长填充
来源：http://fn.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://gz.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://jt.shtwfgs.cn

JS:   "7".padStart(3, "0")
来源：http://ve.bjjhwx.cn

TS:   "7".padStart(3, "0")
来源：http://eg.shxzukj.cn

Java: String.format("%03d", 7)
来源：http://qs.shxzskj.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://zn.yuexingan06.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://sg.panjiajie.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://zi.jctech888.com.cn

[E11] 反转字符串
来源：http://po.asd995.cn

Py:   s[::-1]
来源：http://zl.nszjky.cn

PHP:  strrev($s);
来源：http://ul.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://gd.szsharing.cn

TS:   [...s].reverse().join("")
来源：http://dn.jctech888.com.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://zd.521024.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://qn.hnjuh.cn

Ruby: s.reverse
来源：http://kn.asd995.cn

C#:   new string(s.Reverse().ToArray())
来源：http://xa.asd995.cn

[E12] 统计某字符出现次数
来源：http://js.haigaiapp.cn

Py:   s.count("a")
来源：http://aq.jianghongdianzi.cn

PHP:  substr_count($s, "a");
来源：http://lx.521024.cn

JS:   s.split("a").length - 1
来源：http://xw.chemitech.net.cn

TS:   s.split("a").length - 1
来源：http://gn.huixiangedu.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gx.nicolike.cn

Go:   strings.Count(s, "a")
来源：http://np.yuexingan06.cn

Ruby: s.count("a")
来源：http://wn.yuexingan06.cn

C#:   s.Count(c => c == 'a')
来源：http://py.hahajie.cn

[E13] 逐字符遍历
来源：http://ki.shxzukj.cn

Py:   for ch in s: print(ch)
来源：http://cb.shxzukj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://bo.wgjwhj.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://il.bjjhwx.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ar.panjiajie.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://kn.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://nd.shxzukj.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://xj.newstarts.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mw.huixiangedu.cn

[E14] URL 编码与 Base64
来源：http://uv.muxihuayi.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://el.shxzskj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://kz.panjiajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://am.shxzskj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://tk.newstarts.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ty.nszjky.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tp.muxihuayi.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://kx.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://up.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://rl.bjjhwx.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lt.huixiangedu.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://jv.9csxet.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fv.newstarts.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ln.szsharing.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oi.9csxet.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://fk.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ro.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://jm.yuntaijiaju.cn

[E16] 数字千分位
来源：http://ue.huixiangedu.cn

Py:   f"{1234567:,}"
来源：http://se.chemitech.net.cn

PHP:  number_format(1234567);
来源：http://wi.shtwfgs.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zp.shxzukj.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://po.bookmarksfly.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ah.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ka.huixiangedu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fx.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://qs.hahajie.cn

[E17] 首字母大写
来源：http://no.haigaiapp.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mk.szxytkj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sm.yuexingan06.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://gn.jctech888.com.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ut.shxzskj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://of.huixinmuqiang.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ng.jctech888.com.cn

Ruby: s.capitalize
来源：http://bv.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wy.shxzukj.cn

[E18] 模板占位符替换
来源：http://re.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://qy.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vp.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://dw.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mj.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pv.gzmigu.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://tc.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mf.wgjwhj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ij.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://ee.wgjwhj.cn

Py:   s.splitlines()
来源：http://ny.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wm.huixinmuqiang.cn

JS:   s.split(/\r?\n/)
来源：http://ej.jianghongdianzi.cn

TS:   s.split(/\r?\n/)
来源：http://ks.gzmigu.cn

Java: s.lines().toList()
来源：http://mq.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://pw.panjiajie.cn

Ruby: s.lines
来源：http://re.yuexingan06.cn

C#:   s.Split('\n')
来源：http://dp.hahajie.cn

[E20] 判断字符串是否为空
来源：http://dm.hnjuh.cn

Py:   if not s:
来源：http://ia.yuntaijiaju.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://tq.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gf.gzmigu.cn

TS:   if (s === "") {}
来源：http://gn.shxzskj.cn

Java: if (s.isEmpty()) {}
来源：http://kg.asd995.cn

Go:   if s == "" {}
来源：http://aa.panjiajie.cn

Ruby: if s.empty?
来源：http://ya.colortex.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://vl.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://dd.szsharing.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://cl.gzmigu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mo.bjjhwx.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kx.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xv.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://gn.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://vq.yuexingan06.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ff.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jb.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://ms.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ym.huanxung.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://yl.jctech888.com.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jp.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://am.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zj.colortex.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ew.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://ni.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qp.bookmarksfly.cn

================================================================================
来源：http://ja.huixinmuqiang.cn

F. 文件与目录
来源：http://pw.szxytkj.cn

================================================================================
来源：http://jj.szxytkj.cn

[F01] 读取整个文件
来源：http://yj.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tp.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://xt.bjjhwx.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wg.gzmigu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://nl.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hb.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dz.nszjky.cn

Ruby: File.read("a.txt")
来源：http://oe.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ww.haigaiapp.cn

[F02] 逐行读取文件
来源：http://yl.haigaiapp.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://oq.521024.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qh.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wz.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://qr.nszjky.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ey.yuexingan06.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://lj.huanxung.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://om.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://pi.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jr.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://oh.szsharing.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qe.jctech888.com.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zr.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mb.nicolike.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gk.haigaiapp.cn

Ruby: File.write("a.txt", "hi")
来源：http://de.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nk.chemitech.net.cn

[F04] 追加写入文件
来源：http://re.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mt.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ht.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://br.hahajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://km.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lr.9csxet.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ym.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ws.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mm.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://fn.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dg.chemitech.net.cn

PHP:  file_exists("a.txt");
来源：http://vc.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://pf.szsharing.cn

TS:   fs.existsSync("a.txt")
来源：http://gm.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lw.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ab.521024.cn

Ruby: File.exist?("a.txt")
来源：http://fw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://za.colortex.cn

[F06] 删除文件
来源：http://zs.nicolike.cn

Py:   os.remove("a.txt")
来源：http://dz.hnjuh.cn

PHP:  unlink("a.txt");
来源：http://rk.lnxyls.cn

JS:   fs.unlinkSync("a.txt")
来源：http://pk.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://db.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jl.szsharing.cn

Go:   os.Remove("a.txt")
来源：http://bn.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://wf.nicolike.cn

C#:   File.Delete("a.txt");
来源：http://zz.chemitech.net.cn

[F07] 创建目录（含多级）
来源：http://yr.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://kl.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://uc.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nc.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://km.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oh.shxzukj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://uz.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ak.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sq.huixiangedu.cn

[F08] 遍历目录
来源：http://jd.bjjhwx.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://rc.colortex.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://jg.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://ny.szxytkj.cn

TS:   fs.readdirSync("dir")
来源：http://dp.gzmigu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hk.colortex.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ai.newstarts.cn

Ruby: Dir.children("dir")
来源：http://qr.szsharing.cn

C#:   Directory.GetFiles("dir")
来源：http://cn.newstarts.cn

[F09] 获取文件大小
来源：http://vv.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://oi.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://hz.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://sz.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://ew.jianghongdianzi.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oj.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ff.huanxung.cn

Ruby: File.size("a.txt")
来源：http://zx.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://lx.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ta.wgjwhj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kf.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ps.asd995.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wp.chemitech.net.cn

TS:   path.extname("a.txt")
来源：http://tb.nicolike.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nf.huixinmuqiang.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dy.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://td.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ss.asd995.cn

[F11] 复制与移动文件
来源：http://zo.huixinmuqiang.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fi.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://xh.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tk.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pd.shxzukj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ik.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://es.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://an.szxytkj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ut.bjjhwx.cn

[F12] CSV 读写
来源：http://sa.lnxyls.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lr.yuntaijiaju.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://nr.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qh.521024.cn

TS:   // 同上
来源：http://cm.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://li.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fc.shxzskj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://pr.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rf.huixiangedu.cn

================================================================================
来源：http://qj.colortex.cn

G. 面向对象
来源：http://cc.shtwfgs.cn

================================================================================
来源：http://wb.huixiangedu.cn

[G01] 定义类
来源：http://ve.szxytkj.cn

Py:   class User: pass
来源：http://lq.muxihuayi.cn

PHP:  class User {}
来源：http://kd.szxytkj.cn

JS:   class User {}
来源：http://je.panjiajie.cn

TS:   class User { name: string = ""; }
来源：http://bk.jianghongdianzi.cn

Java: class User {}
来源：http://zn.shxzukj.cn

Go:   type User struct { Name string }
来源：http://em.lnxyls.cn

Ruby: class User; end
来源：http://xh.jianghongdianzi.cn

C#:   class User {}
来源：http://ya.521024.cn

[G02] 构造函数
来源：http://vh.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://hn.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://sp.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://zr.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://ee.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://ia.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ns.nicolike.cn

Ruby: def initialize(name); @name = name; end
来源：http://uj.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://hm.yuexingan06.cn

[G03] 实例属性
来源：http://ar.shxzskj.cn

Py:   self.name = "x"
来源：http://eu.hnjuh.cn

PHP:  public string $name = "x";
来源：http://ip.hnjuh.cn

JS:   this.name = "x";
来源：http://dg.panjiajie.cn

TS:   name: string = "x";
来源：http://kh.521024.cn

Java: private String name;
来源：http://pc.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://me.lnxyls.cn

Ruby: @name = "x"
来源：http://en.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://og.bookmarksfly.cn

[G04] 定义方法
来源：http://yl.huanxung.cn

Py:   def greet(self): return self.name
来源：http://no.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pd.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://nl.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://fv.bjjhwx.cn

Java: String greet() { return name; }
来源：http://la.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://zs.hahajie.cn

Ruby: def greet; @name; end
来源：http://mx.nszjky.cn

C#:   public string Greet() => Name;
来源：http://io.bjjhwx.cn

[G05] 继承
来源：http://yb.shxzukj.cn

Py:   class Admin(User): pass
来源：http://sh.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://lv.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://ll.chemitech.net.cn

TS:   class Admin extends User {}
来源：http://vg.jctech888.com.cn

Java: class Admin extends User {}
来源：http://cw.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ey.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://zr.haigaiapp.cn

C#:   class Admin : User {}
来源：http://ib.newstarts.cn

[G06] 重写方法
来源：http://st.huanxung.cn

Py:   def greet(self): return "admin"
来源：http://fv.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ro.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://zq.nicolike.cn

TS:   greet(): string { return "admin"; }
来源：http://aw.asd995.cn

Java: @Override String greet() { return "admin"; }
来源：http://va.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ns.colortex.cn

Ruby: def greet; "admin"; end
来源：http://ny.shxzskj.cn


<!-- 参考信息 -->