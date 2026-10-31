代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://kg.bookmarksfly.cn

PHP:  preg_replace('/\s+/', '', $s);
来源：http://kw.colortex.cn

JS:   s.replace(/\s+/g, "")
来源：http://pj.huanxung.cn

TS:   s.replace(/\s+/g, "")
来源：http://we.asd995.cn

Java: s.replaceAll("\\s+", "")
来源：http://jw.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://gw.huanxung.cn

Ruby: s.gsub(/\s+/, "")
来源：http://ja.yuntaijiaju.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://fd.bjjhwx.cn

[E10] 左侧补零 / 定长填充
来源：http://bb.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://lz.nszjky.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://ge.lnxyls.cn

JS:   "7".padStart(3, "0")
来源：http://pn.gzmigu.cn

TS:   "7".padStart(3, "0")
来源：http://oz.521024.cn

Java: String.format("%03d", 7)
来源：http://cd.bookmarksfly.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pq.bookmarksfly.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://if.lnxyls.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://rr.lnxyls.cn

[E11] 反转字符串
来源：http://gk.bookmarksfly.cn

Py:   s[::-1]
来源：http://tq.nicolike.cn

PHP:  strrev($s);
来源：http://uh.asd995.cn

JS:   [...s].reverse().join("")
来源：http://on.newstarts.cn

TS:   [...s].reverse().join("")
来源：http://re.szxytkj.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://ex.hnjuh.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://mc.wgjwhj.cn

Ruby: s.reverse
来源：http://wc.panjiajie.cn

C#:   new string(s.Reverse().ToArray())
来源：http://kl.huixiangedu.cn

[E12] 统计某字符出现次数
来源：http://va.colortex.cn

Py:   s.count("a")
来源：http://fv.colortex.cn

PHP:  substr_count($s, "a");
来源：http://sy.521024.cn

JS:   s.split("a").length - 1
来源：http://zy.huixiangedu.cn

TS:   s.split("a").length - 1
来源：http://fr.yuntaijiaju.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://gf.nszjky.cn

Go:   strings.Count(s, "a")
来源：http://kp.huixinmuqiang.cn

Ruby: s.count("a")
来源：http://xs.nszjky.cn

C#:   s.Count(c => c == 'a')
来源：http://gr.shtwfgs.cn

[E13] 逐字符遍历
来源：http://ex.huanxung.cn

Py:   for ch in s: print(ch)
来源：http://xh.szsharing.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://dj.huanxung.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ze.colortex.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://lo.shtwfgs.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://lf.newstarts.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wv.shtwfgs.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://rw.huixiangedu.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://cx.9csxet.cn

[E14] URL 编码与 Base64
来源：http://mb.nicolike.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://ub.yuexingan06.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ks.bjjhwx.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://pq.shtwfgs.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://gz.shxzskj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://fj.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://bz.shxzskj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://gl.hahajie.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lh.panjiajie.cn

[E15] HTML 转义 / 反转义
来源：http://un.9csxet.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://yq.huanxung.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ce.nszjky.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hy.haigaiapp.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vf.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ka.newstarts.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hu.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mc.haigaiapp.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://nb.nicolike.cn

[E16] 数字千分位
来源：http://nx.asd995.cn

Py:   f"{1234567:,}"
来源：http://wq.huanxung.cn

PHP:  number_format(1234567);
来源：http://ul.wgjwhj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ae.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://pb.9csxet.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://bt.nszjky.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://jv.yuntaijiaju.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ze.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://xq.yuexingan06.cn

[E17] 首字母大写
来源：http://px.lnxyls.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://li.bjjhwx.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lm.hnjuh.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://jn.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qs.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ug.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://vv.yuntaijiaju.cn

Ruby: s.capitalize
来源：http://mp.chemitech.net.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://uu.lnxyls.cn

[E18] 模板占位符替换
来源：http://pc.yuexingan06.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hv.shxzukj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yb.yuexingan06.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pq.nszjky.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vm.shxzskj.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oy.nicolike.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ub.9csxet.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ny.shtwfgs.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://jn.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://bg.521024.cn

Py:   s.splitlines()
来源：http://ze.huixinmuqiang.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://cj.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://ol.panjiajie.cn

TS:   s.split(/\r?\n/)
来源：http://ov.huixiangedu.cn

Java: s.lines().toList()
来源：http://en.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://zw.colortex.cn

Ruby: s.lines
来源：http://xf.huanxung.cn

C#:   s.Split('\n')
来源：http://bf.9csxet.cn

[E20] 判断字符串是否为空
来源：http://sv.wgjwhj.cn

Py:   if not s:
来源：http://aa.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ih.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://zv.newstarts.cn

TS:   if (s === "") {}
来源：http://ly.nszjky.cn

Java: if (s.isEmpty()) {}
来源：http://if.shtwfgs.cn

Go:   if s == "" {}
来源：http://lv.yuexingan06.cn

Ruby: if s.empty?
来源：http://iw.lnxyls.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xs.hahajie.cn

[E21] 超长截断加省略号
来源：http://bu.huixinmuqiang.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://bc.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gv.chemitech.net.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dk.bookmarksfly.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mb.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://tv.521024.cn

Go:   // 按 rune 判断长度后截断
来源：http://xe.nicolike.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://do.shtwfgs.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://iu.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://hg.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://es.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gt.lnxyls.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qs.haigaiapp.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zx.huixinmuqiang.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://vn.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://rq.yuexingan06.cn

Ruby: s.bytesize;  s.length
来源：http://vb.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gs.lnxyls.cn

================================================================================
来源：http://sb.szxytkj.cn

F. 文件与目录
来源：http://qf.hahajie.cn

================================================================================
来源：http://lc.nicolike.cn

[F01] 读取整个文件
来源：http://wt.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://zr.hnjuh.cn

PHP:  file_get_contents("a.txt");
来源：http://qa.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vj.jianghongdianzi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wr.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sa.huixinmuqiang.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://kx.szsharing.cn

Ruby: File.read("a.txt")
来源：http://kk.lnxyls.cn

C#:   File.ReadAllText("a.txt");
来源：http://qc.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://sj.huixinmuqiang.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://sw.nicolike.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://qf.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://kf.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ju.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wz.chemitech.net.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ny.shtwfgs.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jo.lnxyls.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://by.521024.cn

[F03] 写入文件（覆盖）
来源：http://tn.szxytkj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://tu.huanxung.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lw.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jw.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://up.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://yy.hahajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mc.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://vw.jctech888.com.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://uu.wgjwhj.cn

[F04] 追加写入文件
来源：http://hn.nicolike.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hq.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://je.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zi.muxihuayi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gs.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://lg.hnjuh.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qs.gzmigu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ia.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://xc.huixiangedu.cn

[F05] 判断文件或目录是否存在
来源：http://fo.521024.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vc.yuntaijiaju.cn

PHP:  file_exists("a.txt");
来源：http://mn.yuexingan06.cn

JS:   fs.existsSync("a.txt")
来源：http://ey.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://ec.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://hv.huixinmuqiang.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mt.shxzukj.cn

Ruby: File.exist?("a.txt")
来源：http://hn.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://rz.wgjwhj.cn

[F06] 删除文件
来源：http://dz.9csxet.cn

Py:   os.remove("a.txt")
来源：http://gu.nszjky.cn

PHP:  unlink("a.txt");
来源：http://oo.huixinmuqiang.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ja.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://kj.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lc.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://wn.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://om.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://tv.asd995.cn

[F07] 创建目录（含多级）
来源：http://mz.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fb.hnjuh.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://if.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ir.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://aw.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yh.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://am.hahajie.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://aw.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ow.szxytkj.cn

[F08] 遍历目录
来源：http://cw.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ce.nicolike.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://op.gzmigu.cn

JS:   fs.readdirSync("dir")
来源：http://ok.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://fk.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ph.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://oc.9csxet.cn

Ruby: Dir.children("dir")
来源：http://xb.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://so.jctech888.com.cn

[F09] 获取文件大小
来源：http://rb.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://kv.szxytkj.cn

PHP:  filesize("a.txt");
来源：http://lt.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://sz.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://nt.yuexingan06.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pb.shxzskj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ks.huixiangedu.cn

Ruby: File.size("a.txt")
来源：http://mo.panjiajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://wg.shtwfgs.cn

[F10] 取文件扩展名 / 文件名
来源：http://jh.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xs.nszjky.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rl.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ot.nszjky.cn

TS:   path.extname("a.txt")
来源：http://rm.newstarts.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vl.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ss.yuntaijiaju.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pn.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lz.colortex.cn

[F11] 复制与移动文件
来源：http://wq.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ka.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oa.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fr.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://iu.lnxyls.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fd.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yq.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vt.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pt.521024.cn

[F12] CSV 读写
来源：http://mw.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sd.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sb.521024.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://if.nicolike.cn

TS:   // 同上
来源：http://bf.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://lk.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bb.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yy.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fl.jianghongdianzi.cn

================================================================================
来源：http://ln.shtwfgs.cn

G. 面向对象
来源：http://qx.nicolike.cn

================================================================================
来源：http://oe.jctech888.com.cn

[G01] 定义类
来源：http://td.jctech888.com.cn

Py:   class User: pass
来源：http://as.yuexingan06.cn

PHP:  class User {}
来源：http://ac.huanxung.cn

JS:   class User {}
来源：http://sq.szxytkj.cn

TS:   class User { name: string = ""; }
来源：http://yr.asd995.cn

Java: class User {}
来源：http://nb.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://tf.nszjky.cn

Ruby: class User; end
来源：http://pq.colortex.cn

C#:   class User {}
来源：http://hq.hahajie.cn

[G02] 构造函数
来源：http://tv.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://dw.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://lj.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://dk.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ds.nszjky.cn

Java: User(String name) { this.name = name; }
来源：http://ty.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lq.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jg.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ig.muxihuayi.cn

[G03] 实例属性
来源：http://xm.szsharing.cn

Py:   self.name = "x"
来源：http://rc.jctech888.com.cn

PHP:  public string $name = "x";
来源：http://na.hnjuh.cn

JS:   this.name = "x";
来源：http://gk.hahajie.cn

TS:   name: string = "x";
来源：http://rh.521024.cn

Java: private String name;
来源：http://ru.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ee.wgjwhj.cn

Ruby: @name = "x"
来源：http://uq.huixiangedu.cn

C#:   public string Name { get; set; } = "x";
来源：http://pl.jctech888.com.cn

[G04] 定义方法
来源：http://qi.wgjwhj.cn

Py:   def greet(self): return self.name
来源：http://tz.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://tl.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://zu.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://iw.chemitech.net.cn

Java: String greet() { return name; }
来源：http://mn.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://rh.jianghongdianzi.cn

Ruby: def greet; @name; end
来源：http://hv.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://om.gzmigu.cn

[G05] 继承
来源：http://rf.nszjky.cn

Py:   class Admin(User): pass
来源：http://jt.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://qe.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://sh.szxytkj.cn

TS:   class Admin extends User {}
来源：http://js.yuntaijiaju.cn

Java: class Admin extends User {}
来源：http://yc.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rn.huixinmuqiang.cn

Ruby: class Admin < User; end
来源：http://pf.hahajie.cn

C#:   class Admin : User {}
来源：http://hj.jianghongdianzi.cn

[G06] 重写方法
来源：http://xk.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://en.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yc.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://al.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://uh.nszjky.cn

Java: @Override String greet() { return "admin"; }
来源：http://dz.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://qg.muxihuayi.cn

Ruby: def greet; "admin"; end
来源：http://cq.huixiangedu.cn

C#:   public override string Greet() => "admin";
来源：http://am.bookmarksfly.cn

[G07] 调用父类方法
来源：http://hm.panjiajie.cn

Py:   super().greet()
来源：http://ko.shxzukj.cn

PHP:  parent::greet();
来源：http://yb.shtwfgs.cn

JS:   super.greet();
来源：http://kt.asd995.cn

TS:   super.greet();
来源：http://xe.shxzukj.cn

Java: super.greet();
来源：http://ds.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://rb.haigaiapp.cn


<!-- 参考信息 -->