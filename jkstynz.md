代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://dx.521024.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://yp.9csxet.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://bb.bookmarksfly.cn

JS:   "7".padStart(3, "0")
来源：http://cv.shtwfgs.cn

TS:   "7".padStart(3, "0")
来源：http://xj.lnxyls.cn

Java: String.format("%03d", 7)
来源：http://zw.colortex.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://pt.hahajie.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://xu.9csxet.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://qf.nszjky.cn

[E11] 反转字符串
来源：http://ua.huixiangedu.cn

Py:   s[::-1]
来源：http://gs.yuntaijiaju.cn

PHP:  strrev($s);
来源：http://oa.nicolike.cn

JS:   [...s].reverse().join("")
来源：http://aw.gzmigu.cn

TS:   [...s].reverse().join("")
来源：http://co.huixiangedu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://df.szxytkj.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://ei.szxytkj.cn

Ruby: s.reverse
来源：http://wh.szxytkj.cn

C#:   new string(s.Reverse().ToArray())
来源：http://sl.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://az.521024.cn

Py:   s.count("a")
来源：http://xr.521024.cn

PHP:  substr_count($s, "a");
来源：http://ic.nszjky.cn

JS:   s.split("a").length - 1
来源：http://px.gzmigu.cn

TS:   s.split("a").length - 1
来源：http://rr.9csxet.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://rv.shxzskj.cn

Go:   strings.Count(s, "a")
来源：http://ar.521024.cn

Ruby: s.count("a")
来源：http://jp.shxzskj.cn

C#:   s.Count(c => c == 'a')
来源：http://uy.gzmigu.cn

[E13] 逐字符遍历
来源：http://sd.gzmigu.cn

Py:   for ch in s: print(ch)
来源：http://vk.huixiangedu.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://th.hnjuh.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://eo.jianghongdianzi.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://yg.shxzukj.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mg.huixinmuqiang.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://se.chemitech.net.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://ax.nszjky.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mt.huanxung.cn

[E14] URL 编码与 Base64
来源：http://xm.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xk.yuntaijiaju.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bg.shxzskj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://vl.gzmigu.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://sr.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zi.jctech888.com.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hc.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://ef.nszjky.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://ox.huixiangedu.cn

[E15] HTML 转义 / 反转义
来源：http://ah.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://sh.panjiajie.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://oa.asd995.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://lp.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zj.shtwfgs.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://ty.shxzukj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://ho.szsharing.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zs.jctech888.com.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://xh.shxzukj.cn

[E16] 数字千分位
来源：http://jm.asd995.cn

Py:   f"{1234567:,}"
来源：http://me.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://ii.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uu.shtwfgs.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://nm.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://yi.shtwfgs.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mg.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://cu.wgjwhj.cn

C#:   1234567.ToString("N0")
来源：http://bj.jctech888.com.cn

[E17] 首字母大写
来源：http://py.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sv.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://tj.asd995.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://oy.muxihuayi.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ra.jianghongdianzi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://kr.bjjhwx.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ma.nszjky.cn

Ruby: s.capitalize
来源：http://kr.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://er.hnjuh.cn

[E18] 模板占位符替换
来源：http://hp.huixiangedu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://gj.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yr.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://fv.bookmarksfly.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ea.huixiangedu.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://cy.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://be.shxzskj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nw.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://we.521024.cn

[E19] 多行文本按行拆分
来源：http://df.hahajie.cn

Py:   s.splitlines()
来源：http://ra.yuntaijiaju.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://uw.shxzskj.cn

JS:   s.split(/\r?\n/)
来源：http://at.huanxung.cn

TS:   s.split(/\r?\n/)
来源：http://bs.chemitech.net.cn

Java: s.lines().toList()
来源：http://qr.521024.cn

Go:   strings.Split(s, "\n")
来源：http://wg.nszjky.cn

Ruby: s.lines
来源：http://mh.newstarts.cn

C#:   s.Split('\n')
来源：http://bu.colortex.cn

[E20] 判断字符串是否为空
来源：http://uu.nszjky.cn

Py:   if not s:
来源：http://by.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://sb.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://jq.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ua.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://bd.jianghongdianzi.cn

Go:   if s == "" {}
来源：http://wn.colortex.cn

Ruby: if s.empty?
来源：http://dj.shxzukj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://la.shxzukj.cn

[E21] 超长截断加省略号
来源：http://va.jctech888.com.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ye.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gy.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://qe.yuexingan06.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hx.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jq.asd995.cn

Go:   // 按 rune 判断长度后截断
来源：http://in.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://oi.muxihuayi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dn.huixiangedu.cn

[E22] 字节长度与字符长度
来源：http://kp.newstarts.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://sl.jianghongdianzi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sh.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hw.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nu.szsharing.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jw.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wm.shxzukj.cn

Ruby: s.bytesize;  s.length
来源：http://lt.jctech888.com.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ym.bjjhwx.cn

================================================================================
来源：http://et.huixinmuqiang.cn

F. 文件与目录
来源：http://cx.jctech888.com.cn

================================================================================
来源：http://bs.muxihuayi.cn

[F01] 读取整个文件
来源：http://wi.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://dx.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://uf.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://uq.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ud.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zk.colortex.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jc.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://oe.haigaiapp.cn

C#:   File.ReadAllText("a.txt");
来源：http://pe.jianghongdianzi.cn

[F02] 逐行读取文件
来源：http://ma.chemitech.net.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://pb.gzmigu.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://uh.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jg.hahajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jl.lnxyls.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lj.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ph.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://eu.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ae.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://rb.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oo.szsharing.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://cl.chemitech.net.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xn.szxytkj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://nh.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xi.newstarts.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fq.nszjky.cn

Ruby: File.write("a.txt", "hi")
来源：http://js.yuntaijiaju.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ne.nszjky.cn

[F04] 追加写入文件
来源：http://eu.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yr.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yt.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://db.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ar.521024.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://bg.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://oi.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ig.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ia.muxihuayi.cn

[F05] 判断文件或目录是否存在
来源：http://jx.wgjwhj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sq.shxzukj.cn

PHP:  file_exists("a.txt");
来源：http://hv.haigaiapp.cn

JS:   fs.existsSync("a.txt")
来源：http://ie.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://gl.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rv.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://iw.9csxet.cn

Ruby: File.exist?("a.txt")
来源：http://rp.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://ot.hnjuh.cn

[F06] 删除文件
来源：http://dv.hahajie.cn

Py:   os.remove("a.txt")
来源：http://kl.9csxet.cn

PHP:  unlink("a.txt");
来源：http://gd.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://aw.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ht.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lg.szxytkj.cn

Go:   os.Remove("a.txt")
来源：http://yk.huanxung.cn

Ruby: File.delete("a.txt")
来源：http://oe.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://rf.nszjky.cn

[F07] 创建目录（含多级）
来源：http://yh.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://iq.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ez.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ik.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yf.yuexingan06.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ve.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://bz.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gr.shxzskj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mj.shtwfgs.cn

[F08] 遍历目录
来源：http://xy.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vv.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://bu.bjjhwx.cn

JS:   fs.readdirSync("dir")
来源：http://mm.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://we.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fh.hnjuh.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ht.lnxyls.cn

Ruby: Dir.children("dir")
来源：http://rf.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://ug.shxzskj.cn

[F09] 获取文件大小
来源：http://tg.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://mi.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://cw.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://kv.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://fv.bookmarksfly.cn

Java: Files.size(Path.of("a.txt"))
来源：http://oo.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zx.shtwfgs.cn

Ruby: File.size("a.txt")
来源：http://or.jianghongdianzi.cn

C#:   new FileInfo("a.txt").Length
来源：http://qj.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://wb.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://kh.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://dj.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://om.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://vf.huixinmuqiang.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ek.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rj.bookmarksfly.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://xu.asd995.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ug.panjiajie.cn

[F11] 复制与移动文件
来源：http://nw.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://qy.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ep.bjjhwx.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://as.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rl.521024.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://kv.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://rp.muxihuayi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ia.bookmarksfly.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ru.gzmigu.cn

[F12] CSV 读写
来源：http://ky.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ny.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://pu.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zu.shxzukj.cn

TS:   // 同上
来源：http://kc.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://xb.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ur.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://jm.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rq.shxzskj.cn

================================================================================
来源：http://vy.colortex.cn

G. 面向对象
来源：http://ct.yuexingan06.cn

================================================================================
来源：http://fm.huixiangedu.cn

[G01] 定义类
来源：http://ov.chemitech.net.cn

Py:   class User: pass
来源：http://vt.shxzskj.cn

PHP:  class User {}
来源：http://tf.asd995.cn

JS:   class User {}
来源：http://xt.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://xi.colortex.cn

Java: class User {}
来源：http://dp.521024.cn

Go:   type User struct { Name string }
来源：http://qk.bookmarksfly.cn

Ruby: class User; end
来源：http://fb.bjjhwx.cn

C#:   class User {}
来源：http://gs.colortex.cn

[G02] 构造函数
来源：http://rr.newstarts.cn

Py:   def __init__(self, name): self.name = name
来源：http://vl.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://ru.muxihuayi.cn

JS:   constructor(name) { this.name = name; }
来源：http://sb.huanxung.cn

TS:   constructor(public name: string) {}
来源：http://er.jctech888.com.cn

Java: User(String name) { this.name = name; }
来源：http://mx.huixiangedu.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xt.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ji.lnxyls.cn

C#:   public User(string name) { Name = name; }
来源：http://ao.shxzskj.cn

[G03] 实例属性
来源：http://jd.huixiangedu.cn

Py:   self.name = "x"
来源：http://rg.hnjuh.cn

PHP:  public string $name = "x";
来源：http://tp.9csxet.cn

JS:   this.name = "x";
来源：http://og.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://cf.yuexingan06.cn

Java: private String name;
来源：http://er.hahajie.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ny.shtwfgs.cn

Ruby: @name = "x"
来源：http://kw.wgjwhj.cn

C#:   public string Name { get; set; } = "x";
来源：http://td.shxzskj.cn

[G04] 定义方法
来源：http://dj.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://wd.panjiajie.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://sm.nicolike.cn

JS:   greet() { return this.name; }
来源：http://pc.521024.cn

TS:   greet(): string { return this.name; }
来源：http://aq.chemitech.net.cn

Java: String greet() { return name; }
来源：http://ud.huixiangedu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://su.hahajie.cn

Ruby: def greet; @name; end
来源：http://xy.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://zw.521024.cn

[G05] 继承
来源：http://sv.hahajie.cn

Py:   class Admin(User): pass
来源：http://ik.9csxet.cn

PHP:  class Admin extends User {}
来源：http://dv.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://js.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://nd.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://lk.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tu.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://gy.9csxet.cn

C#:   class Admin : User {}
来源：http://li.muxihuayi.cn

[G06] 重写方法
来源：http://lv.nicolike.cn

Py:   def greet(self): return "admin"
来源：http://sz.jctech888.com.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://eq.gzmigu.cn

JS:   greet() { return "admin"; }
来源：http://hy.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://km.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://wb.jianghongdianzi.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://ms.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://js.521024.cn

C#:   public override string Greet() => "admin";
来源：http://zu.colortex.cn

[G07] 调用父类方法
来源：http://sx.nszjky.cn

Py:   super().greet()
来源：http://la.huixiangedu.cn

PHP:  parent::greet();
来源：http://ul.nszjky.cn

JS:   super.greet();
来源：http://ch.hahajie.cn

TS:   super.greet();
来源：http://qe.jianghongdianzi.cn

Java: super.greet();
来源：http://dd.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://zc.hnjuh.cn

Ruby: super
来源：http://kq.hnjuh.cn

C#:   base.Greet();
来源：http://ji.yuexingan06.cn

[G08] 静态方法与属性
来源：http://kl.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xl.chemitech.net.cn

PHP:  public static function f() {}
来源：http://po.panjiajie.cn

JS:   static f() {}
来源：http://ne.panjiajie.cn

TS:   static f(): void {}
来源：http://ej.colortex.cn

Java: static void f() {}
来源：http://gs.jctech888.com.cn


<!-- 参考信息 -->