代发 wailian999

[E10] 左侧补零 / 定长填充
来源：http://fq.hahajie.cn

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://sh.nicolike.cn

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hp.huixinmuqiang.cn

JS:   "7".padStart(3, "0")
来源：http://tm.chemitech.net.cn

TS:   "7".padStart(3, "0")
来源：http://ep.bookmarksfly.cn

Java: String.format("%03d", 7)
来源：http://qy.hnjuh.cn

Go:   fmt.Sprintf("%03d", 7)
来源：http://do.hnjuh.cn

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://lw.shxzukj.cn

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://ac.hnjuh.cn

[E11] 反转字符串
来源：http://vr.huixiangedu.cn

Py:   s[::-1]
来源：http://xf.9csxet.cn

PHP:  strrev($s);
来源：http://wu.wgjwhj.cn

JS:   [...s].reverse().join("")
来源：http://fh.9csxet.cn

TS:   [...s].reverse().join("")
来源：http://cm.gzmigu.cn

Java: new StringBuilder(s).reverse().toString()
来源：http://hv.hahajie.cn

Go:   // 转 []rune 后倒序再转回 string
来源：http://do.lnxyls.cn

Ruby: s.reverse
来源：http://sn.nszjky.cn

C#:   new string(s.Reverse().ToArray())
来源：http://hs.shxzskj.cn

[E12] 统计某字符出现次数
来源：http://ls.yuntaijiaju.cn

Py:   s.count("a")
来源：http://kq.shtwfgs.cn

PHP:  substr_count($s, "a");
来源：http://ke.szxytkj.cn

JS:   s.split("a").length - 1
来源：http://ik.haigaiapp.cn

TS:   s.split("a").length - 1
来源：http://ye.huixinmuqiang.cn

Java: s.chars().filter(c -> c == 'a').count()
来源：http://ia.jianghongdianzi.cn

Go:   strings.Count(s, "a")
来源：http://ip.shxzskj.cn

Ruby: s.count("a")
来源：http://ey.colortex.cn

C#:   s.Count(c => c == 'a')
来源：http://oj.newstarts.cn

[E13] 逐字符遍历
来源：http://zr.yuexingan06.cn

Py:   for ch in s: print(ch)
来源：http://by.wgjwhj.cn

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://zz.newstarts.cn

JS:   for (const ch of s) { console.log(ch); }
来源：http://ny.521024.cn

TS:   for (const ch of s) { console.log(ch); }
来源：http://wi.haigaiapp.cn

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://zi.yuexingan06.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://vu.yuexingan06.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://uq.lnxyls.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://vk.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://sb.asd995.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://jc.bjjhwx.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://qs.szxytkj.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://nk.jctech888.com.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mw.muxihuayi.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://xz.bjjhwx.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mb.521024.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://tk.huixiangedu.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://dw.bookmarksfly.cn

[E15] HTML 转义 / 反转义
来源：http://jg.huanxung.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jd.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ug.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hx.lnxyls.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://zy.hahajie.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hv.colortex.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://na.muxihuayi.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://zo.huixiangedu.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zf.gzmigu.cn

[E16] 数字千分位
来源：http://pb.yuntaijiaju.cn

Py:   f"{1234567:,}"
来源：http://kl.nszjky.cn

PHP:  number_format(1234567);
来源：http://lv.asd995.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://wu.muxihuayi.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kp.521024.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://dl.jianghongdianzi.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://sb.yuexingan06.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://sh.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://bl.huixiangedu.cn

[E17] 首字母大写
来源：http://yx.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://je.521024.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://em.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://cm.wgjwhj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://dk.szsharing.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ui.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://su.wgjwhj.cn

Ruby: s.capitalize
来源：http://po.shtwfgs.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://yb.9csxet.cn

[E18] 模板占位符替换
来源：http://xu.huanxung.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ho.lnxyls.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hq.newstarts.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ph.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://vw.521024.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xy.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://ag.yuntaijiaju.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://xo.szxytkj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://vl.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://ei.shxzskj.cn

Py:   s.splitlines()
来源：http://tu.newstarts.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://pj.shtwfgs.cn

JS:   s.split(/\r?\n/)
来源：http://yi.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://xg.szxytkj.cn

Java: s.lines().toList()
来源：http://op.huixiangedu.cn

Go:   strings.Split(s, "\n")
来源：http://uf.hnjuh.cn

Ruby: s.lines
来源：http://kk.colortex.cn

C#:   s.Split('\n')
来源：http://uh.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://yz.huixinmuqiang.cn

Py:   if not s:
来源：http://ur.gzmigu.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hj.bookmarksfly.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://df.bjjhwx.cn

TS:   if (s === "") {}
来源：http://on.jctech888.com.cn

Java: if (s.isEmpty()) {}
来源：http://hs.9csxet.cn

Go:   if s == "" {}
来源：http://ip.hnjuh.cn

Ruby: if s.empty?
来源：http://uj.panjiajie.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yy.bjjhwx.cn

[E21] 超长截断加省略号
来源：http://go.9csxet.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pt.huixiangedu.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ox.jianghongdianzi.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wc.szxytkj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pw.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ol.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ue.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://kz.9csxet.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ss.lnxyls.cn

[E22] 字节长度与字符长度
来源：http://zz.szsharing.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hg.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uj.szsharing.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ta.9csxet.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yb.yuntaijiaju.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dr.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oa.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://xo.hnjuh.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://qy.bjjhwx.cn

================================================================================
来源：http://ie.9csxet.cn

F. 文件与目录
来源：http://uj.521024.cn

================================================================================
来源：http://ga.bookmarksfly.cn

[F01] 读取整个文件
来源：http://hy.shxzukj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gl.huixinmuqiang.cn

PHP:  file_get_contents("a.txt");
来源：http://pp.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mj.panjiajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lh.colortex.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://an.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://si.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://rh.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://wt.shtwfgs.cn

[F02] 逐行读取文件
来源：http://ck.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fz.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ci.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://da.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dn.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ue.huanxung.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qt.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://xb.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ii.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://td.panjiajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://om.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ks.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qg.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ix.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://xl.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zw.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://dk.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mb.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://hq.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fg.bjjhwx.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qm.yuntaijiaju.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dz.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tx.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://np.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gw.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://kd.huixinmuqiang.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yb.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://iz.shxzskj.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ar.colortex.cn

PHP:  file_exists("a.txt");
来源：http://jp.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://pt.521024.cn

TS:   fs.existsSync("a.txt")
来源：http://me.asd995.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ve.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rf.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://ha.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://jl.nszjky.cn

[F06] 删除文件
来源：http://pj.shtwfgs.cn

Py:   os.remove("a.txt")
来源：http://jm.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://kd.haigaiapp.cn

JS:   fs.unlinkSync("a.txt")
来源：http://lw.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://di.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://uj.wgjwhj.cn

Go:   os.Remove("a.txt")
来源：http://xq.asd995.cn

Ruby: File.delete("a.txt")
来源：http://hs.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://xv.shxzskj.cn

[F07] 创建目录（含多级）
来源：http://pr.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://md.szxytkj.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gq.hnjuh.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tw.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rc.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://oo.jctech888.com.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xf.huixiangedu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rx.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mh.jctech888.com.cn

[F08] 遍历目录
来源：http://zk.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qf.yuntaijiaju.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://fx.jianghongdianzi.cn

JS:   fs.readdirSync("dir")
来源：http://qk.shtwfgs.cn

TS:   fs.readdirSync("dir")
来源：http://qr.szxytkj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://as.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bu.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://ek.521024.cn

C#:   Directory.GetFiles("dir")
来源：http://wi.nszjky.cn

[F09] 获取文件大小
来源：http://pr.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://vg.bjjhwx.cn

PHP:  filesize("a.txt");
来源：http://ou.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ku.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://ty.colortex.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hm.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lv.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://yg.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://ck.panjiajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://yg.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://xn.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ys.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hv.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://cf.bjjhwx.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mf.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sa.lnxyls.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://tu.yuntaijiaju.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wz.jctech888.com.cn

[F11] 复制与移动文件
来源：http://oq.panjiajie.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://gu.shxzukj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://vi.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ph.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://kl.jctech888.com.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mc.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ci.szxytkj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gs.asd995.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jw.wgjwhj.cn

[F12] CSV 读写
来源：http://zy.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hj.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yf.9csxet.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://om.jianghongdianzi.cn

TS:   // 同上
来源：http://xk.szxytkj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://uh.9csxet.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ls.colortex.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zv.muxihuayi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ep.shtwfgs.cn

================================================================================
来源：http://sr.szsharing.cn

G. 面向对象
来源：http://cf.wgjwhj.cn

================================================================================
来源：http://cy.shxzukj.cn

[G01] 定义类
来源：http://ul.shxzukj.cn

Py:   class User: pass
来源：http://zu.shxzukj.cn

PHP:  class User {}
来源：http://kx.nszjky.cn

JS:   class User {}
来源：http://lk.521024.cn

TS:   class User { name: string = ""; }
来源：http://sz.shxzskj.cn

Java: class User {}
来源：http://hp.jianghongdianzi.cn

Go:   type User struct { Name string }
来源：http://in.nszjky.cn

Ruby: class User; end
来源：http://tq.huanxung.cn

C#:   class User {}
来源：http://kj.wgjwhj.cn

[G02] 构造函数
来源：http://xo.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://zh.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://zc.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://zr.newstarts.cn

TS:   constructor(public name: string) {}
来源：http://qc.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://ml.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wi.bjjhwx.cn

Ruby: def initialize(name); @name = name; end
来源：http://ph.chemitech.net.cn

C#:   public User(string name) { Name = name; }
来源：http://ws.colortex.cn

[G03] 实例属性
来源：http://qc.nszjky.cn

Py:   self.name = "x"
来源：http://ak.asd995.cn

PHP:  public string $name = "x";
来源：http://ec.panjiajie.cn

JS:   this.name = "x";
来源：http://ao.yuexingan06.cn

TS:   name: string = "x";
来源：http://fg.9csxet.cn

Java: private String name;
来源：http://fk.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://dx.shxzskj.cn

Ruby: @name = "x"
来源：http://wr.lnxyls.cn

C#:   public string Name { get; set; } = "x";
来源：http://aj.panjiajie.cn

[G04] 定义方法
来源：http://aq.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://zb.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qj.shxzskj.cn

JS:   greet() { return this.name; }
来源：http://wm.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://xc.lnxyls.cn

Java: String greet() { return name; }
来源：http://nd.nszjky.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kq.bookmarksfly.cn

Ruby: def greet; @name; end
来源：http://qu.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://re.yuntaijiaju.cn

[G05] 继承
来源：http://pi.gzmigu.cn

Py:   class Admin(User): pass
来源：http://vn.wgjwhj.cn

PHP:  class Admin extends User {}
来源：http://qt.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://bi.yuntaijiaju.cn

TS:   class Admin extends User {}
来源：http://er.jctech888.com.cn

Java: class Admin extends User {}
来源：http://ul.shtwfgs.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://dw.colortex.cn

Ruby: class Admin < User; end
来源：http://hx.szsharing.cn

C#:   class Admin : User {}
来源：http://qi.yuntaijiaju.cn

[G06] 重写方法
来源：http://dj.nszjky.cn

Py:   def greet(self): return "admin"
来源：http://iq.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://gz.colortex.cn

JS:   greet() { return "admin"; }
来源：http://yv.jianghongdianzi.cn

TS:   greet(): string { return "admin"; }
来源：http://ps.huixiangedu.cn

Java: @Override String greet() { return "admin"; }
来源：http://pd.shtwfgs.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fa.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://yr.wgjwhj.cn

C#:   public override string Greet() => "admin";
来源：http://kw.huanxung.cn

[G07] 调用父类方法
来源：http://zx.newstarts.cn

Py:   super().greet()
来源：http://yd.jctech888.com.cn

PHP:  parent::greet();
来源：http://sz.nszjky.cn

JS:   super.greet();
来源：http://mn.nszjky.cn

TS:   super.greet();
来源：http://ew.nicolike.cn

Java: super.greet();
来源：http://ss.hnjuh.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://jq.wgjwhj.cn

Ruby: super
来源：http://cf.jctech888.com.cn

C#:   base.Greet();
来源：http://he.panjiajie.cn

[G08] 静态方法与属性
来源：http://vg.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nk.yuexingan06.cn

PHP:  public static function f() {}
来源：http://ja.chemitech.net.cn

JS:   static f() {}
来源：http://sc.hnjuh.cn

TS:   static f(): void {}
来源：http://ck.shtwfgs.cn

Java: static void f() {}
来源：http://sx.hahajie.cn


<!-- 参考信息 -->