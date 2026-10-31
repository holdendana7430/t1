代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wj.jianghongdianzi.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://rs.huixinmuqiang.cn

JS:   s.replace(/\s+/g, "")
来源：http://tb.521024.cn

TS:   s.replace(/\s+/g, "")
来源：http://xy.yuntaijiaju.cn

Java: s.replaceAll("\\s+", "")
来源：http://sp.hnjuh.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ju.yuexingan06.cn

Ruby: s.gsub(/\s+/, "")
来源：http://bh.shtwfgs.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://iu.colortex.cn

[E10] 左侧补零 / 定长填充
来源：http://jp.huixiangedu.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://rl.muxihuayi.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://aw.newstarts.cn

JS:   "7".padStart(3, "0")
来源：http://pf.asd995.cn

TS:   "7".padStart(3, "0")
来源：http://rt.nicolike.cn

Java: String.format("%03d", 7)
来源：http://cc.newstarts.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://rd.jctech888.com.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://uq.yuntaijiaju.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://an.haigaiapp.cn

[E11] 反转字符串
来源：http://zn.9csxet.cn

Py:   s[::-1]
来源：http://bf.jctech888.com.cn

PHP:  strrev($s);
来源：http://ps.szxytkj.cn

JS:   [...s].reverse().join("")
来源：http://cz.hnjuh.cn

TS:   [...s].reverse().join("")
来源：http://qa.9csxet.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://sy.gzmigu.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://xd.gzmigu.cn

Ruby: s.reverse
来源：http://fr.jctech888.com.cn

C#:   new string(s.Reverse().ToArray())
来源：http://yg.jctech888.com.cn

[E12] 统计某字符出现次数
来源：http://vl.newstarts.cn

Py:   s.count("a")
来源：http://gx.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://rs.bjjhwx.cn

JS:   s.split("a").length - 1
来源：http://oc.bjjhwx.cn

TS:   s.split("a").length - 1
来源：http://kn.nicolike.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ms.huanxung.cn

Go:   strings.Count(s, "a")
来源：http://yc.shtwfgs.cn

Ruby: s.count("a")
来源：http://zf.shtwfgs.cn

C#:   s.Count(c => c == 'a')
来源：http://zt.huixiangedu.cn

[E13] 逐字符遍历
来源：http://da.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://yf.9csxet.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://gt.nszjky.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://hf.huanxung.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://vh.chemitech.net.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://em.nicolike.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://ej.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ep.shxzukj.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://ha.nszjky.cn

[E14] URL 编码与 Base64
来源：http://jb.shxzskj.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://qb.521024.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://cj.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://kj.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://de.9csxet.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mh.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://ti.colortex.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://my.wgjwhj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://iq.lnxyls.cn

[E15] HTML 转义 / 反转义
来源：http://wa.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://fr.wgjwhj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://gd.shxzskj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kv.9csxet.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://uc.gzmigu.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://fi.hahajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ii.huixiangedu.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bz.panjiajie.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wf.jctech888.com.cn

[E16] 数字千分位
来源：http://dm.colortex.cn

Py:   f"{1234567:,}"
来源：http://ql.shxzukj.cn

PHP:  number_format(1234567);
来源：http://ib.jianghongdianzi.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qz.hahajie.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://py.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://qa.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qi.chemitech.net.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://gw.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://ar.chemitech.net.cn

[E17] 首字母大写
来源：http://mm.hnjuh.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ph.shxzukj.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://bd.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://da.yuexingan06.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zi.chemitech.net.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://om.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gc.jctech888.com.cn

Ruby: s.capitalize
来源：http://nm.newstarts.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mt.szsharing.cn

[E18] 模板占位符替换
来源：http://it.jctech888.com.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wd.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://dc.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://hq.shxzskj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://fe.shtwfgs.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pg.huanxung.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zq.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://re.newstarts.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ld.jianghongdianzi.cn

[E19] 多行文本按行拆分
来源：http://hs.shtwfgs.cn

Py:   s.splitlines()
来源：http://uj.hahajie.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yo.huanxung.cn

JS:   s.split(/\r?\n/)
来源：http://da.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://fs.wgjwhj.cn

Java: s.lines().toList()
来源：http://uj.bjjhwx.cn

Go:   strings.Split(s, "\n")
来源：http://vt.9csxet.cn

Ruby: s.lines
来源：http://qb.hahajie.cn

C#:   s.Split('\n')
来源：http://um.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://dd.huanxung.cn

Py:   if not s:
来源：http://od.jctech888.com.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hd.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qa.asd995.cn

TS:   if (s === "") {}
来源：http://ny.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://yj.nszjky.cn

Go:   if s == "" {}
来源：http://uh.nicolike.cn

Ruby: if s.empty?
来源：http://zq.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ch.shxzukj.cn

[E21] 超长截断加省略号
来源：http://tf.shxzskj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://sr.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tx.bookmarksfly.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://jp.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://at.shxzskj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hf.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://er.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xh.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cv.nicolike.cn

[E22] 字节长度与字符长度
来源：http://rl.colortex.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://oh.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://if.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ei.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://so.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vb.9csxet.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ah.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://pp.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gl.shxzskj.cn

================================================================================
来源：http://ea.hahajie.cn

F. 文件与目录
来源：http://xn.9csxet.cn

================================================================================
来源：http://oi.hnjuh.cn

[F01] 读取整个文件
来源：http://rq.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hu.wgjwhj.cn

PHP:  file_get_contents("a.txt");
来源：http://ti.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://yh.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vn.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://eo.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://yz.colortex.cn

Ruby: File.read("a.txt")
来源：http://of.muxihuayi.cn

C#:   File.ReadAllText("a.txt");
来源：http://fv.gzmigu.cn

[F02] 逐行读取文件
来源：http://qi.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qc.haigaiapp.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pp.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vf.yuexingan06.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://qw.9csxet.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://yz.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ud.chemitech.net.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://nd.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://of.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://ci.huixinmuqiang.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hi.shxzukj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://gn.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wc.nszjky.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xr.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://uk.bjjhwx.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://jf.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://xa.szxytkj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://kn.521024.cn

[F04] 追加写入文件
来源：http://uh.bookmarksfly.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://qm.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xk.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dy.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wn.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ai.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oj.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ej.newstarts.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://nt.shxzskj.cn

[F05] 判断文件或目录是否存在
来源：http://lx.bjjhwx.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hb.gzmigu.cn

PHP:  file_exists("a.txt");
来源：http://ww.lnxyls.cn

JS:   fs.existsSync("a.txt")
来源：http://el.muxihuayi.cn

TS:   fs.existsSync("a.txt")
来源：http://lm.szxytkj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://db.haigaiapp.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://zi.gzmigu.cn

Ruby: File.exist?("a.txt")
来源：http://tf.huixinmuqiang.cn

C#:   File.Exists("a.txt")
来源：http://li.szsharing.cn

[F06] 删除文件
来源：http://qq.521024.cn

Py:   os.remove("a.txt")
来源：http://ga.newstarts.cn

PHP:  unlink("a.txt");
来源：http://nf.bjjhwx.cn

JS:   fs.unlinkSync("a.txt")
来源：http://rq.yuexingan06.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vb.huixinmuqiang.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://aq.shtwfgs.cn

Go:   os.Remove("a.txt")
来源：http://ic.lnxyls.cn

Ruby: File.delete("a.txt")
来源：http://gr.bookmarksfly.cn

C#:   File.Delete("a.txt");
来源：http://gi.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://av.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bq.bjjhwx.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://qq.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ln.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iv.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://eg.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ig.shxzskj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aw.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://qg.wgjwhj.cn

[F08] 遍历目录
来源：http://yl.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://lm.szxytkj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wn.colortex.cn

JS:   fs.readdirSync("dir")
来源：http://hn.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://lp.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zn.9csxet.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://om.nicolike.cn

Ruby: Dir.children("dir")
来源：http://kt.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://pv.lnxyls.cn

[F09] 获取文件大小
来源：http://ss.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://jr.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://gx.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://mz.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://hf.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://by.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yb.521024.cn

Ruby: File.size("a.txt")
来源：http://kz.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://bz.shxzukj.cn

[F10] 取文件扩展名 / 文件名
来源：http://ax.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://gx.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://fw.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://co.huanxung.cn

TS:   path.extname("a.txt")
来源：http://yd.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tf.newstarts.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mz.shxzskj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://uf.hnjuh.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://uy.yuntaijiaju.cn

[F11] 复制与移动文件
来源：http://uu.shxzukj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gj.panjiajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mp.nszjky.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hi.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bq.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://du.shxzukj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jb.wgjwhj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://of.haigaiapp.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hj.haigaiapp.cn

[F12] CSV 读写
来源：http://od.huanxung.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vc.bjjhwx.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qd.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ho.shtwfgs.cn

TS:   // 同上
来源：http://oz.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://bq.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fb.szsharing.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ov.huixinmuqiang.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sl.lnxyls.cn

================================================================================
来源：http://zm.newstarts.cn

G. 面向对象
来源：http://ds.shxzukj.cn

================================================================================
来源：http://rz.gzmigu.cn

[G01] 定义类
来源：http://ii.shxzukj.cn

Py:   class User: pass
来源：http://eu.shtwfgs.cn

PHP:  class User {}
来源：http://rp.nicolike.cn

JS:   class User {}
来源：http://nl.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://er.szsharing.cn

Java: class User {}
来源：http://oy.shxzukj.cn

Go:   type User struct { Name string }
来源：http://cs.gzmigu.cn

Ruby: class User; end
来源：http://lx.newstarts.cn

C#:   class User {}
来源：http://wm.newstarts.cn

[G02] 构造函数
来源：http://ld.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://oh.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://pk.panjiajie.cn

JS:   constructor(name) { this.name = name; }
来源：http://nv.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://vo.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://mk.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ly.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ji.shxzukj.cn

C#:   public User(string name) { Name = name; }
来源：http://ki.szxytkj.cn

[G03] 实例属性
来源：http://mj.jctech888.com.cn

Py:   self.name = "x"
来源：http://wz.9csxet.cn

PHP:  public string $name = "x";
来源：http://fa.shxzukj.cn

JS:   this.name = "x";
来源：http://go.huanxung.cn

TS:   name: string = "x";
来源：http://tl.9csxet.cn

Java: private String name;
来源：http://sm.gzmigu.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kx.yuexingan06.cn

Ruby: @name = "x"
来源：http://ta.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://qs.asd995.cn

[G04] 定义方法
来源：http://ph.nszjky.cn

Py:   def greet(self): return self.name
来源：http://dy.shxzskj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://um.huanxung.cn

JS:   greet() { return this.name; }
来源：http://fr.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://jx.muxihuayi.cn

Java: String greet() { return name; }
来源：http://ac.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fs.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://ck.newstarts.cn

C#:   public string Greet() => Name;
来源：http://kt.bjjhwx.cn

[G05] 继承
来源：http://xy.panjiajie.cn

Py:   class Admin(User): pass
来源：http://kg.yuexingan06.cn

PHP:  class Admin extends User {}
来源：http://bz.shxzskj.cn

JS:   class Admin extends User {}
来源：http://ea.shxzskj.cn

TS:   class Admin extends User {}
来源：http://pt.szsharing.cn

Java: class Admin extends User {}
来源：http://cy.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://jz.nszjky.cn

Ruby: class Admin < User; end
来源：http://xz.chemitech.net.cn

C#:   class Admin : User {}
来源：http://kr.huixinmuqiang.cn

[G06] 重写方法
来源：http://zf.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://im.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sq.huixiangedu.cn

JS:   greet() { return "admin"; }
来源：http://cj.asd995.cn

TS:   greet(): string { return "admin"; }
来源：http://hi.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://np.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://eg.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://oa.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://hq.yuexingan06.cn

[G07] 调用父类方法
来源：http://qx.szsharing.cn

Py:   super().greet()
来源：http://mr.szxytkj.cn

PHP:  parent::greet();
来源：http://gs.bjjhwx.cn

JS:   super.greet();
来源：http://pw.nicolike.cn

TS:   super.greet();
来源：http://pw.jctech888.com.cn

Java: super.greet();
来源：http://rz.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://vj.huixiangedu.cn


<!-- 参考信息 -->