代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://zp.bjjhwx.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://lz.panjiajie.cn

JS:   s.replace(/\s+/g, "")
来源：http://qh.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://vj.yuexingan06.cn

Java: s.replaceAll("\\s+", "")
来源：http://uy.nicolike.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gw.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://id.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://rf.521024.cn

[E10] 左侧补零 / 定长填充
来源：http://eh.haigaiapp.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://pt.hnjuh.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://nr.hnjuh.cn

JS:   "7".padStart(3, "0")
来源：http://fn.shxzskj.cn

TS:   "7".padStart(3, "0")
来源：http://ri.haigaiapp.cn

Java: String.format("%03d", 7)
来源：http://jf.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://tf.shxzukj.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xe.bjjhwx.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://vi.chemitech.net.cn

[E11] 反转字符串
来源：http://gd.nicolike.cn

Py:   s[::-1]
来源：http://vr.bjjhwx.cn

PHP:  strrev($s);
来源：http://qv.gzmigu.cn

JS:   [...s].reverse().join("")
来源：http://mw.haigaiapp.cn

TS:   [...s].reverse().join("")
来源：http://ml.shtwfgs.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://xc.jianghongdianzi.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ui.newstarts.cn

Ruby: s.reverse
来源：http://wc.huixiangedu.cn

C#:   new string(s.Reverse().ToArray())
来源：http://zl.nszjky.cn

[E12] 统计某字符出现次数
来源：http://bx.wgjwhj.cn

Py:   s.count("a")
来源：http://dv.shxzukj.cn

PHP:  substr_count($s, "a");
来源：http://zl.9csxet.cn

JS:   s.split("a").length - 1
来源：http://jk.szxytkj.cn

TS:   s.split("a").length - 1
来源：http://kp.panjiajie.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://qj.yuntaijiaju.cn

Go:   strings.Count(s, "a")
来源：http://gs.521024.cn

Ruby: s.count("a")
来源：http://sv.9csxet.cn

C#:   s.Count(c => c == 'a')
来源：http://ak.huanxung.cn

[E13] 逐字符遍历
来源：http://gx.asd995.cn

Py:   for ch in s: print(ch)
来源：http://cv.gzmigu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://ot.lnxyls.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://kt.hahajie.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://cs.nszjky.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://oq.wgjwhj.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://cs.hahajie.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ia.shtwfgs.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://sl.hahajie.cn

[E14] URL 编码与 Base64
来源：http://ew.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wa.wgjwhj.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://jq.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://jy.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://kg.szsharing.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://cz.asd995.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bo.yuexingan06.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://nx.haigaiapp.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ud.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://ly.521024.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://rb.bjjhwx.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://rt.huixinmuqiang.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fl.szxytkj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bx.shxzskj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://oh.bjjhwx.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://iv.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ky.colortex.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://le.hnjuh.cn

[E16] 数字千分位
来源：http://ol.hnjuh.cn

Py:   f"{1234567:,}"
来源：http://ij.shxzskj.cn

PHP:  number_format(1234567);
来源：http://po.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://vb.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xo.bjjhwx.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://jo.huixinmuqiang.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lg.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wd.yuntaijiaju.cn

C#:   1234567.ToString("N0")
来源：http://hg.bjjhwx.cn

[E17] 首字母大写
来源：http://wr.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://lf.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mw.shxzukj.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ee.asd995.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ma.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://xp.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://be.hahajie.cn

Ruby: s.capitalize
来源：http://by.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://ra.asd995.cn

[E18] 模板占位符替换
来源：http://hv.wgjwhj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://rp.jianghongdianzi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://vg.gzmigu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://di.huixinmuqiang.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://du.haigaiapp.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://an.newstarts.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://gp.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://lk.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kc.asd995.cn

[E19] 多行文本按行拆分
来源：http://gk.huanxung.cn

Py:   s.splitlines()
来源：http://ey.shxzukj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://fz.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://gx.yuexingan06.cn

TS:   s.split(/\r?\n/)
来源：http://fj.asd995.cn

Java: s.lines().toList()
来源：http://hc.wgjwhj.cn

Go:   strings.Split(s, "\n")
来源：http://ht.wgjwhj.cn

Ruby: s.lines
来源：http://ap.huanxung.cn

C#:   s.Split('\n')
来源：http://fu.jianghongdianzi.cn

[E20] 判断字符串是否为空
来源：http://zh.lnxyls.cn

Py:   if not s:
来源：http://kh.lnxyls.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://dh.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ar.lnxyls.cn

TS:   if (s === "") {}
来源：http://wa.shxzukj.cn

Java: if (s.isEmpty()) {}
来源：http://to.wgjwhj.cn

Go:   if s == "" {}
来源：http://ez.nszjky.cn

Ruby: if s.empty?
来源：http://dz.chemitech.net.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ey.shxzukj.cn

[E21] 超长截断加省略号
来源：http://kb.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qw.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://qv.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fm.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://up.wgjwhj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://fc.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://ei.jianghongdianzi.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://xm.hnjuh.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://jl.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://wr.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nd.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://si.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ty.shxzskj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yr.hnjuh.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://kc.haigaiapp.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://am.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://jx.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cv.bjjhwx.cn

================================================================================
来源：http://ul.panjiajie.cn

F. 文件与目录
来源：http://rd.bjjhwx.cn

================================================================================
来源：http://ly.huixiangedu.cn

[F01] 读取整个文件
来源：http://nu.bookmarksfly.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zj.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://lx.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://jy.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qk.nicolike.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zr.nicolike.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://vd.huanxung.cn

Ruby: File.read("a.txt")
来源：http://fz.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://wj.shxzukj.cn

[F02] 逐行读取文件
来源：http://ih.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bv.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ag.newstarts.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gv.asd995.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yl.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://oh.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ec.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ta.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://li.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://kd.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uh.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ol.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ga.muxihuayi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fd.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vy.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://de.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://mb.panjiajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://al.shtwfgs.cn

[F04] 追加写入文件
来源：http://sl.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wh.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ck.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qk.shxzskj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://oo.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bt.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gy.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://so.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://jy.chemitech.net.cn

[F05] 判断文件或目录是否存在
来源：http://hf.hahajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://qj.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://nn.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://il.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://cm.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ry.gzmigu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ql.haigaiapp.cn

Ruby: File.exist?("a.txt")
来源：http://xu.shtwfgs.cn

C#:   File.Exists("a.txt")
来源：http://fh.jctech888.com.cn

[F06] 删除文件
来源：http://fl.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://bg.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://bn.wgjwhj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://le.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nf.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wt.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://md.nszjky.cn

Ruby: File.delete("a.txt")
来源：http://fk.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://vd.gzmigu.cn

[F07] 创建目录（含多级）
来源：http://pv.shtwfgs.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://dj.shtwfgs.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pw.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bu.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pp.hahajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://qf.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://tn.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://cj.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ml.521024.cn

[F08] 遍历目录
来源：http://ck.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ph.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xg.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://ai.asd995.cn

TS:   fs.readdirSync("dir")
来源：http://sm.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wy.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ux.huixiangedu.cn

Ruby: Dir.children("dir")
来源：http://qd.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://ky.jctech888.com.cn

[F09] 获取文件大小
来源：http://tv.shxzukj.cn

Py:   os.path.getsize("a.txt")
来源：http://mj.shtwfgs.cn

PHP:  filesize("a.txt");
来源：http://dq.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://gy.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://nn.hnjuh.cn

Java: Files.size(Path.of("a.txt"))
来源：http://zc.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pi.hnjuh.cn

Ruby: File.size("a.txt")
来源：http://zv.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://vp.yuntaijiaju.cn

[F10] 取文件扩展名 / 文件名
来源：http://il.chemitech.net.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://jk.521024.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rz.jianghongdianzi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wv.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://lc.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://tp.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gq.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ke.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lz.nszjky.cn

[F11] 复制与移动文件
来源：http://pm.jctech888.com.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jk.9csxet.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ov.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ee.shxzskj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://pg.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://uo.gzmigu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fq.panjiajie.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://jw.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kp.chemitech.net.cn

[F12] CSV 读写
来源：http://uy.gzmigu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nd.hnjuh.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://is.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ur.gzmigu.cn

TS:   // 同上
来源：http://sx.hahajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://pl.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gl.chemitech.net.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://di.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ve.colortex.cn

================================================================================
来源：http://vf.shxzukj.cn

G. 面向对象
来源：http://aj.hahajie.cn

================================================================================
来源：http://te.jctech888.com.cn

[G01] 定义类
来源：http://cs.szxytkj.cn

Py:   class User: pass
来源：http://vw.yuexingan06.cn

PHP:  class User {}
来源：http://lg.haigaiapp.cn

JS:   class User {}
来源：http://oj.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://fg.colortex.cn

Java: class User {}
来源：http://ir.szsharing.cn

Go:   type User struct { Name string }
来源：http://sc.haigaiapp.cn

Ruby: class User; end
来源：http://wh.haigaiapp.cn

C#:   class User {}
来源：http://rg.colortex.cn

[G02] 构造函数
来源：http://pz.colortex.cn

Py:   def __init__(self, name): self.name = name
来源：http://jv.gzmigu.cn

PHP:  public function __construct(public string $name) {}
来源：http://qn.szsharing.cn

JS:   constructor(name) { this.name = name; }
来源：http://yp.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://rm.521024.cn

Java: User(String name) { this.name = name; }
来源：http://gy.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://fi.huixiangedu.cn

Ruby: def initialize(name); @name = name; end
来源：http://tj.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://db.nicolike.cn

[G03] 实例属性
来源：http://xw.haigaiapp.cn

Py:   self.name = "x"
来源：http://fj.newstarts.cn

PHP:  public string $name = "x";
来源：http://id.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://ia.gzmigu.cn

TS:   name: string = "x";
来源：http://lo.hnjuh.cn

Java: private String name;
来源：http://pg.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nv.nszjky.cn

Ruby: @name = "x"
来源：http://zy.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://kz.szxytkj.cn

[G04] 定义方法
来源：http://gy.nicolike.cn

Py:   def greet(self): return self.name
来源：http://vl.szsharing.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://td.szsharing.cn

JS:   greet() { return this.name; }
来源：http://cw.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://zj.haigaiapp.cn

Java: String greet() { return name; }
来源：http://uq.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ur.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://yi.nszjky.cn

C#:   public string Greet() => Name;
来源：http://ts.panjiajie.cn

[G05] 继承
来源：http://ek.huanxung.cn

Py:   class Admin(User): pass
来源：http://xz.colortex.cn

PHP:  class Admin extends User {}
来源：http://fa.colortex.cn

JS:   class Admin extends User {}
来源：http://lp.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://go.huixiangedu.cn

Java: class Admin extends User {}
来源：http://zx.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://qb.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://xf.9csxet.cn

C#:   class Admin : User {}
来源：http://rm.shxzukj.cn

[G06] 重写方法
来源：http://ag.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://fw.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tw.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ge.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://qk.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://di.shxzskj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://lv.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://of.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://fq.wgjwhj.cn

[G07] 调用父类方法
来源：http://ff.nszjky.cn

Py:   super().greet()
来源：http://iz.huixiangedu.cn

PHP:  parent::greet();
来源：http://dl.nicolike.cn

JS:   super.greet();
来源：http://gk.nicolike.cn

TS:   super.greet();
来源：http://qw.bookmarksfly.cn

Java: super.greet();
来源：http://tj.newstarts.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hj.haigaiapp.cn


<!-- 参考信息 -->