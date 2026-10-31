代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://um.shxzskj.cn

Go:   strings.Join(strings.Fields(s), "")
来源：http://ay.huixiangedu.cn

Ruby: s.gsub(/\s+/, "")
来源：http://er.szxytkj.cn

C#:   Regex.Replace(s, @"\s+", "")
来源：http://xn.bookmarksfly.cn

[E10] 左侧补零 / 定长填充
来源：http://jo.szxytkj.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://ws.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://km.bjjhwx.cn

JS:   "7".padStart(3, "0")
来源：http://qg.panjiajie.cn

TS:   "7".padStart(3, "0")
来源：http://vx.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://pl.szsharing.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://bq.muxihuayi.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://cw.newstarts.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://el.yuexingan06.cn

[E11] 反转字符串
来源：http://jk.wgjwhj.cn

Py:   s[::-1]
来源：http://dw.shxzskj.cn

PHP:  strrev($s);
来源：http://ne.newstarts.cn

JS:   [...s].reverse().join("")
来源：http://tg.szxytkj.cn

TS:   [...s].reverse().join("")
来源：http://nd.chemitech.net.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://rn.bjjhwx.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://gq.colortex.cn

Ruby: s.reverse
来源：http://jg.lnxyls.cn

C#:   new string(s.Reverse().ToArray())
来源：http://gi.nicolike.cn

[E12] 统计某字符出现次数
来源：http://nu.lnxyls.cn

Py:   s.count("a")
来源：http://kc.asd995.cn

PHP:  substr_count($s, "a");
来源：http://et.bookmarksfly.cn

JS:   s.split("a").length - 1
来源：http://bc.nicolike.cn

TS:   s.split("a").length - 1
来源：http://bb.huanxung.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://us.wgjwhj.cn

Go:   strings.Count(s, "a")
来源：http://jv.hahajie.cn

Ruby: s.count("a")
来源：http://yy.yuntaijiaju.cn

C#:   s.Count(c => c == 'a')
来源：http://xs.nicolike.cn

[E13] 逐字符遍历
来源：http://as.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://yh.huixinmuqiang.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://qu.bjjhwx.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ki.9csxet.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://ml.nicolike.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://vc.hahajie.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://tg.jianghongdianzi.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://em.bjjhwx.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://kq.shxzskj.cn

[E14] URL 编码与 Base64
来源：http://fw.lnxyls.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://vk.panjiajie.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://nv.gzmigu.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ia.wgjwhj.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ku.jctech888.com.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mr.shxzukj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://lp.bookmarksfly.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tp.shxzukj.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://rb.huixinmuqiang.cn

[E15] HTML 转义 / 反转义
来源：http://qx.gzmigu.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://pb.yuexingan06.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://be.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://uh.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://kl.9csxet.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vf.shtwfgs.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://zf.bookmarksfly.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ta.newstarts.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xe.szxytkj.cn

[E16] 数字千分位
来源：http://pb.szsharing.cn

Py:   f"{1234567:,}"
来源：http://fg.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://fo.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://hk.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ne.yuexingan06.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://xc.hnjuh.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wf.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ke.huixiangedu.cn

C#:   1234567.ToString("N0")
来源：http://rn.haigaiapp.cn

[E17] 首字母大写
来源：http://mi.jctech888.com.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hn.yuexingan06.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://lb.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://df.shtwfgs.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://pq.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zr.szsharing.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wu.wgjwhj.cn

Ruby: s.capitalize
来源：http://qn.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://vm.muxihuayi.cn

[E18] 模板占位符替换
来源：http://ap.szxytkj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ml.hnjuh.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wf.haigaiapp.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zk.yuntaijiaju.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://kj.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://oi.jctech888.com.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ur.haigaiapp.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://rq.szsharing.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://az.asd995.cn

[E19] 多行文本按行拆分
来源：http://ue.asd995.cn

Py:   s.splitlines()
来源：http://hy.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://zm.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://ig.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://dc.nszjky.cn

Java: s.lines().toList()
来源：http://qq.panjiajie.cn

Go:   strings.Split(s, "\n")
来源：http://ul.szsharing.cn

Ruby: s.lines
来源：http://tm.wgjwhj.cn

C#:   s.Split('\n')
来源：http://ms.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://hj.colortex.cn

Py:   if not s:
来源：http://rf.9csxet.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://gv.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://gy.nszjky.cn

TS:   if (s === "") {}
来源：http://bp.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://jx.hnjuh.cn

Go:   if s == "" {}
来源：http://zk.jianghongdianzi.cn

Ruby: if s.empty?
来源：http://tu.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gx.shtwfgs.cn

[E21] 超长截断加省略号
来源：http://bx.muxihuayi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hw.lnxyls.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zl.nicolike.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pn.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nv.huanxung.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ex.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://na.haigaiapp.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://nt.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ul.shxzukj.cn

[E22] 字节长度与字符长度
来源：http://bf.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ha.colortex.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ql.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://gs.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yk.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://th.yuexingan06.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://nj.jianghongdianzi.cn

Ruby: s.bytesize;  s.length
来源：http://xp.bjjhwx.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://bq.wgjwhj.cn

================================================================================
来源：http://ha.chemitech.net.cn

F. 文件与目录
来源：http://pw.nszjky.cn

================================================================================
来源：http://go.hahajie.cn

[F01] 读取整个文件
来源：http://xq.yuntaijiaju.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://rg.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://iq.colortex.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ea.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ls.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zy.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ea.newstarts.cn

Ruby: File.read("a.txt")
来源：http://qb.jianghongdianzi.cn

C#:   File.ReadAllText("a.txt");
来源：http://ia.asd995.cn

[F02] 逐行读取文件
来源：http://qg.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://nh.jctech888.com.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://aw.colortex.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gy.521024.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://db.colortex.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vz.521024.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://io.bookmarksfly.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ms.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kl.colortex.cn

[F03] 写入文件（覆盖）
来源：http://zu.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ln.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rs.lnxyls.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://cw.huixinmuqiang.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ma.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fy.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ea.9csxet.cn

Ruby: File.write("a.txt", "hi")
来源：http://ve.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://px.hahajie.cn

[F04] 追加写入文件
来源：http://ih.bjjhwx.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://az.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://kq.nszjky.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ei.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://om.shxzskj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ds.huixiangedu.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lz.hahajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eb.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://lo.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://ob.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://rd.huixiangedu.cn

PHP:  file_exists("a.txt");
来源：http://oc.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://zt.newstarts.cn

TS:   fs.existsSync("a.txt")
来源：http://qg.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ys.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ur.newstarts.cn

Ruby: File.exist?("a.txt")
来源：http://yf.asd995.cn

C#:   File.Exists("a.txt")
来源：http://qk.jctech888.com.cn

[F06] 删除文件
来源：http://mw.yuexingan06.cn

Py:   os.remove("a.txt")
来源：http://gs.wgjwhj.cn

PHP:  unlink("a.txt");
来源：http://ng.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bn.gzmigu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://rf.shxzskj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zk.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://ae.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://ll.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://wu.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://gt.521024.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ul.huanxung.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sj.huixiangedu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ay.yuexingan06.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://bq.muxihuayi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ky.hahajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sq.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://tz.gzmigu.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.szxytkj.cn

[F08] 遍历目录
来源：http://qf.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tr.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://br.szxytkj.cn

JS:   fs.readdirSync("dir")
来源：http://zx.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://el.lnxyls.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mm.shxzskj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lg.asd995.cn

Ruby: Dir.children("dir")
来源：http://ti.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://dw.bjjhwx.cn

[F09] 获取文件大小
来源：http://fn.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://jq.bookmarksfly.cn

PHP:  filesize("a.txt");
来源：http://cw.muxihuayi.cn

JS:   fs.statSync("a.txt").size
来源：http://zw.hahajie.cn

TS:   fs.statSync("a.txt").size
来源：http://ju.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ga.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://xz.nszjky.cn

Ruby: File.size("a.txt")
来源：http://xf.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ft.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://az.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zf.asd995.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://oq.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://fk.lnxyls.cn

TS:   path.extname("a.txt")
来源：http://yy.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://pw.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://qa.muxihuayi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://bl.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ll.bjjhwx.cn

[F11] 复制与移动文件
来源：http://hb.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ji.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://lj.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rr.hnjuh.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://cq.szxytkj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://en.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ej.huanxung.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wh.wgjwhj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nt.gzmigu.cn

[F12] CSV 读写
来源：http://ye.szsharing.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://td.newstarts.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lk.yuexingan06.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bd.gzmigu.cn

TS:   // 同上
来源：http://bk.nszjky.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vu.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xq.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mc.shxzskj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ss.521024.cn

================================================================================
来源：http://ap.huixinmuqiang.cn

G. 面向对象
来源：http://rn.bjjhwx.cn

================================================================================
来源：http://pz.newstarts.cn

[G01] 定义类
来源：http://ff.szxytkj.cn

Py:   class User: pass
来源：http://dl.jctech888.com.cn

PHP:  class User {}
来源：http://cb.yuntaijiaju.cn

JS:   class User {}
来源：http://kc.lnxyls.cn

TS:   class User { name: string = ""; }
来源：http://jr.newstarts.cn

Java: class User {}
来源：http://jf.szxytkj.cn

Go:   type User struct { Name string }
来源：http://gp.muxihuayi.cn

Ruby: class User; end
来源：http://qj.yuntaijiaju.cn

C#:   class User {}
来源：http://nh.szsharing.cn

[G02] 构造函数
来源：http://ps.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://ig.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://jo.shxzukj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ta.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://du.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://gu.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vv.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ye.gzmigu.cn

C#:   public User(string name) { Name = name; }
来源：http://oa.huixinmuqiang.cn

[G03] 实例属性
来源：http://zw.wgjwhj.cn

Py:   self.name = "x"
来源：http://pi.9csxet.cn

PHP:  public string $name = "x";
来源：http://im.chemitech.net.cn

JS:   this.name = "x";
来源：http://rx.521024.cn

TS:   name: string = "x";
来源：http://cn.huixiangedu.cn

Java: private String name;
来源：http://ab.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://gb.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://ql.colortex.cn

C#:   public string Name { get; set; } = "x";
来源：http://zj.wgjwhj.cn

[G04] 定义方法
来源：http://ua.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://qm.huixiangedu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vn.shxzukj.cn

JS:   greet() { return this.name; }
来源：http://iu.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://wh.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://hc.jianghongdianzi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://za.lnxyls.cn

Ruby: def greet; @name; end
来源：http://bp.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://sj.jctech888.com.cn

[G05] 继承
来源：http://rf.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://jt.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://hq.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://wz.huanxung.cn

TS:   class Admin extends User {}
来源：http://ms.huixiangedu.cn

Java: class Admin extends User {}
来源：http://ew.521024.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://uh.newstarts.cn

Ruby: class Admin < User; end
来源：http://xa.jianghongdianzi.cn

C#:   class Admin : User {}
来源：http://me.newstarts.cn

[G06] 重写方法
来源：http://ix.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://ls.hnjuh.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ln.jctech888.com.cn

JS:   greet() { return "admin"; }
来源：http://sv.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://vb.shxzskj.cn

Java: @Override String greet() { return "admin"; }
来源：http://az.hnjuh.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ut.asd995.cn

Ruby: def greet; "admin"; end
来源：http://cm.yuntaijiaju.cn

C#:   public override string Greet() => "admin";
来源：http://hu.yuexingan06.cn

[G07] 调用父类方法
来源：http://ok.hnjuh.cn

Py:   super().greet()
来源：http://vs.521024.cn

PHP:  parent::greet();
来源：http://gf.jianghongdianzi.cn

JS:   super.greet();
来源：http://ff.shtwfgs.cn

TS:   super.greet();
来源：http://xt.nszjky.cn

Java: super.greet();
来源：http://bn.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://do.huixiangedu.cn

Ruby: super
来源：http://ib.gzmigu.cn

C#:   base.Greet();
来源：http://yb.chemitech.net.cn

[G08] 静态方法与属性
来源：http://fs.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xe.lnxyls.cn


<!-- 参考信息 -->