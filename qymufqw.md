代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://ij.lnxyls.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://yp.newstarts.cn

JS:   s.replace(/\s+/g, "")
来源：http://rn.colortex.cn

TS:   s.replace(/\s+/g, "")
来源：http://we.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://qj.lnxyls.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://lq.wgjwhj.cn

Ruby: s.gsub(/\s+/, "")
来源：http://kc.hahajie.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://bo.muxihuayi.cn

[E10] 左侧补零 / 定长填充
来源：http://gf.panjiajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://tr.szsharing.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nz.shxzukj.cn

JS:   "7".padStart(3, "0")
来源：http://dh.nszjky.cn

TS:   "7".padStart(3, "0")
来源：http://og.yuexingan06.cn

Java: String.format("%03d", 7)
来源：http://tq.panjiajie.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://jd.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://zu.szsharing.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://yx.muxihuayi.cn

[E11] 反转字符串
来源：http://nb.szsharing.cn

Py:   s[::-1]
来源：http://vm.haigaiapp.cn

PHP:  strrev($s);
来源：http://ck.yuexingan06.cn

JS:   [...s].reverse().join("")
来源：http://ai.shtwfgs.cn

TS:   [...s].reverse().join("")
来源：http://ie.huixinmuqiang.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://in.haigaiapp.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://db.newstarts.cn

Ruby: s.reverse
来源：http://qi.bookmarksfly.cn

C#:   new string(s.Reverse().ToArray())
来源：http://ub.shxzukj.cn

[E12] 统计某字符出现次数
来源：http://yx.haigaiapp.cn

Py:   s.count("a")
来源：http://xy.hahajie.cn

PHP:  substr_count($s, "a");
来源：http://ho.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://cj.asd995.cn

TS:   s.split("a").length - 1
来源：http://ai.muxihuayi.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ky.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://vy.jctech888.com.cn

Ruby: s.count("a")
来源：http://sv.jianghongdianzi.cn

C#:   s.Count(c => c == 'a')
来源：http://fr.hnjuh.cn

[E13] 逐字符遍历
来源：http://tw.asd995.cn

Py:   for ch in s: print(ch)
来源：http://yj.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qs.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://xt.yuntaijiaju.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://gx.huixiangedu.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vn.haigaiapp.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://gm.gzmigu.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://gr.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://oi.shtwfgs.cn

[E14] URL 编码与 Base64
来源：http://yx.bjjhwx.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ux.huixinmuqiang.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://pa.nszjky.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nd.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ty.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wv.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://tk.jctech888.com.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://bk.asd995.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://gt.wgjwhj.cn

[E15] HTML 转义 / 反转义
来源：http://ll.huixiangedu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://lx.chemitech.net.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://vm.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hf.huanxung.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://je.nicolike.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://tv.jianghongdianzi.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://xq.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ys.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cj.newstarts.cn

[E16] 数字千分位
来源：http://ql.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://zk.lnxyls.cn

PHP:  number_format(1234567);
来源：http://ft.huanxung.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://rh.nszjky.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sr.newstarts.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dp.yuexingan06.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://uc.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ge.haigaiapp.cn

C#:   1234567.ToString("N0")
来源：http://ux.9csxet.cn

[E17] 首字母大写
来源：http://ut.shtwfgs.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://al.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://if.wgjwhj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ln.haigaiapp.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ar.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://pb.shxzukj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://jx.521024.cn

Ruby: s.capitalize
来源：http://nf.muxihuayi.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nq.panjiajie.cn

[E18] 模板占位符替换
来源：http://fp.colortex.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://vo.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ks.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://yr.huixiangedu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://av.chemitech.net.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pe.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ai.huixinmuqiang.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://dl.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ci.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://pt.bookmarksfly.cn

Py:   s.splitlines()
来源：http://xn.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wq.lnxyls.cn

JS:   s.split(/\r?\n/)
来源：http://en.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://hs.shxzukj.cn

Java: s.lines().toList()
来源：http://iz.hahajie.cn

Go:   strings.Split(s, "\n")
来源：http://vn.colortex.cn

Ruby: s.lines
来源：http://yx.colortex.cn

C#:   s.Split('\n')
来源：http://ws.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://js.newstarts.cn

Py:   if not s:
来源：http://rc.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://cm.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ny.panjiajie.cn

TS:   if (s === "") {}
来源：http://qx.asd995.cn

Java: if (s.isEmpty()) {}
来源：http://nt.bookmarksfly.cn

Go:   if s == "" {}
来源：http://bi.9csxet.cn

Ruby: if s.empty?
来源：http://rb.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://dd.huanxung.cn

[E21] 超长截断加省略号
来源：http://aw.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://fc.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bx.newstarts.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vu.chemitech.net.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://xu.9csxet.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hc.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://mn.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tb.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ac.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://ws.bookmarksfly.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nk.wgjwhj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tg.szxytkj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://zp.shtwfgs.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yi.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xx.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://eo.hnjuh.cn

Ruby: s.bytesize;  s.length
来源：http://nd.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://yq.huixiangedu.cn

================================================================================
来源：http://ui.bookmarksfly.cn

F. 文件与目录
来源：http://rz.hahajie.cn

================================================================================
来源：http://os.gzmigu.cn

[F01] 读取整个文件
来源：http://rn.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://bp.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://rd.newstarts.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hg.haigaiapp.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://en.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eu.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mc.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://yo.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://rc.9csxet.cn

[F02] 逐行读取文件
来源：http://ig.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://dm.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vw.asd995.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://au.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://we.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gw.shxzukj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://xh.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fx.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://is.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://or.nicolike.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ln.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qp.jctech888.com.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cp.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://as.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vg.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mt.huixiangedu.cn

Ruby: File.write("a.txt", "hi")
来源：http://vc.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ge.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://zf.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://pe.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yu.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cl.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ml.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qi.newstarts.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://yu.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://bu.jctech888.com.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://kr.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://na.9csxet.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pd.asd995.cn

PHP:  file_exists("a.txt");
来源：http://sq.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://gd.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://ab.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ul.521024.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ja.szxytkj.cn

Ruby: File.exist?("a.txt")
来源：http://cx.asd995.cn

C#:   File.Exists("a.txt")
来源：http://lj.jianghongdianzi.cn

[F06] 删除文件
来源：http://mv.szxytkj.cn

Py:   os.remove("a.txt")
来源：http://nz.colortex.cn

PHP:  unlink("a.txt");
来源：http://xs.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://de.haigaiapp.cn

TS:   fs.unlinkSync("a.txt")
来源：http://oh.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://jh.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://cy.wgjwhj.cn

Ruby: File.delete("a.txt")
来源：http://zd.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://mx.szsharing.cn

[F07] 创建目录（含多级）
来源：http://tv.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iy.shxzskj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oi.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://im.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xj.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://lt.muxihuayi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ps.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://uu.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hx.chemitech.net.cn

[F08] 遍历目录
来源：http://ea.newstarts.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ox.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ek.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://tr.wgjwhj.cn

TS:   fs.readdirSync("dir")
来源：http://ra.yuntaijiaju.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://nh.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://pl.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://gq.asd995.cn

C#:   Directory.GetFiles("dir")
来源：http://lw.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://oc.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://ml.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://ex.huanxung.cn

JS:   fs.statSync("a.txt").size
来源：http://ou.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://uv.521024.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gi.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://al.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://va.shxzskj.cn

C#:   new FileInfo("a.txt").Length
来源：http://mz.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://zw.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cy.panjiajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://lx.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fx.muxihuayi.cn

TS:   path.extname("a.txt")
来源：http://oc.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://me.521024.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ea.jctech888.com.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://et.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wy.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://wq.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wq.huixiangedu.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zf.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xi.asd995.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ge.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ed.hnjuh.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tl.haigaiapp.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ut.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kv.bjjhwx.cn

[F12] CSV 读写
来源：http://wp.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ye.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ok.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://dl.gzmigu.cn

TS:   // 同上
来源：http://uu.bookmarksfly.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pm.panjiajie.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://po.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xx.bjjhwx.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://bj.521024.cn

================================================================================
来源：http://xp.jianghongdianzi.cn

G. 面向对象
来源：http://bx.panjiajie.cn

================================================================================
来源：http://lj.panjiajie.cn

[G01] 定义类
来源：http://ul.jctech888.com.cn

Py:   class User: pass
来源：http://bs.shxzskj.cn

PHP:  class User {}
来源：http://tz.bookmarksfly.cn

JS:   class User {}
来源：http://wn.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://dg.huixinmuqiang.cn

Java: class User {}
来源：http://ou.colortex.cn

Go:   type User struct { Name string }
来源：http://ge.wgjwhj.cn

Ruby: class User; end
来源：http://xq.nszjky.cn

C#:   class User {}
来源：http://ab.lnxyls.cn

[G02] 构造函数
来源：http://gv.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://nn.lnxyls.cn

PHP:  public function __construct(public string $name) {}
来源：http://du.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://nk.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://xo.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://yt.wgjwhj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ce.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://kz.huixiangedu.cn

C#:   public User(string name) { Name = name; }
来源：http://mz.huanxung.cn

[G03] 实例属性
来源：http://yc.jctech888.com.cn

Py:   self.name = "x"
来源：http://ni.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://mn.huixiangedu.cn

JS:   this.name = "x";
来源：http://ny.wgjwhj.cn

TS:   name: string = "x";
来源：http://bh.bjjhwx.cn

Java: private String name;
来源：http://ft.colortex.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://we.gzmigu.cn

Ruby: @name = "x"
来源：http://xf.shxzukj.cn

C#:   public string Name { get; set; } = "x";
来源：http://pf.muxihuayi.cn

[G04] 定义方法
来源：http://rr.9csxet.cn

Py:   def greet(self): return self.name
来源：http://zm.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ax.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://ci.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://ae.wgjwhj.cn

Java: String greet() { return name; }
来源：http://vp.haigaiapp.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rk.jctech888.com.cn

Ruby: def greet; @name; end
来源：http://ch.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://mm.shxzskj.cn

[G05] 继承
来源：http://cn.huixinmuqiang.cn

Py:   class Admin(User): pass
来源：http://he.yuntaijiaju.cn

PHP:  class Admin extends User {}
来源：http://zq.asd995.cn

JS:   class Admin extends User {}
来源：http://og.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://bw.szsharing.cn

Java: class Admin extends User {}
来源：http://dm.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://lz.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://bc.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://he.shxzskj.cn

[G06] 重写方法
来源：http://th.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://aq.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gt.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://ye.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://ok.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://lx.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://el.colortex.cn

Ruby: def greet; "admin"; end
来源：http://eq.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://bf.shxzukj.cn

[G07] 调用父类方法
来源：http://nq.9csxet.cn

Py:   super().greet()
来源：http://mn.shtwfgs.cn

PHP:  parent::greet();
来源：http://jp.hahajie.cn

JS:   super.greet();
来源：http://zi.shxzskj.cn

TS:   super.greet();
来源：http://op.shxzskj.cn

Java: super.greet();
来源：http://kg.nszjky.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nk.jianghongdianzi.cn


<!-- 参考信息 -->