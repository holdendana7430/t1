代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://xc.521024.cn

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://zt.nszjky.cn

Ruby: s.each_char { |ch| puts ch }
来源：http://tl.hahajie.cn

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://we.shxzukj.cn

[E14] URL 编码与 Base64
来源：http://cg.huixiangedu.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://xl.szsharing.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://bh.jianghongdianzi.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://xy.huanxung.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bj.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ei.huixiangedu.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yq.haigaiapp.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://fb.hnjuh.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://lr.shxzukj.cn

[E15] HTML 转义 / 反转义
来源：http://ul.hahajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://jc.lnxyls.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hr.szsharing.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://vf.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://cw.wgjwhj.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://zn.yuexingan06.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://gp.shxzukj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://bk.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://fg.chemitech.net.cn

[E16] 数字千分位
来源：http://he.haigaiapp.cn

Py:   f"{1234567:,}"
来源：http://bd.bookmarksfly.cn

PHP:  number_format(1234567);
来源：http://wf.colortex.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://uj.huixiangedu.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://op.gzmigu.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://po.huanxung.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yk.huanxung.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ju.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://dm.hnjuh.cn

[E17] 首字母大写
来源：http://xh.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ld.gzmigu.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://sd.colortex.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ao.colortex.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.huixinmuqiang.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ps.nszjky.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gw.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://tn.shxzskj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://sw.shxzukj.cn

[E18] 模板占位符替换
来源：http://fn.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fp.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ng.szxytkj.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://og.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nw.jctech888.com.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://qq.hnjuh.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hv.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wu.nszjky.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dr.9csxet.cn

[E19] 多行文本按行拆分
来源：http://mn.bjjhwx.cn

Py:   s.splitlines()
来源：http://dd.szxytkj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lb.hnjuh.cn

JS:   s.split(/\r?\n/)
来源：http://oz.szxytkj.cn

TS:   s.split(/\r?\n/)
来源：http://yp.haigaiapp.cn

Java: s.lines().toList()
来源：http://wq.jianghongdianzi.cn

Go:   strings.Split(s, "\n")
来源：http://ud.lnxyls.cn

Ruby: s.lines
来源：http://ps.gzmigu.cn

C#:   s.Split('\n')
来源：http://yf.bjjhwx.cn

[E20] 判断字符串是否为空
来源：http://jw.bjjhwx.cn

Py:   if not s:
来源：http://yt.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ry.hahajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hk.huixinmuqiang.cn

TS:   if (s === "") {}
来源：http://ph.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://xj.szxytkj.cn

Go:   if s == "" {}
来源：http://iq.huixiangedu.cn

Ruby: if s.empty?
来源：http://gh.yuntaijiaju.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eq.szsharing.cn

[E21] 超长截断加省略号
来源：http://qw.yuntaijiaju.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://kj.panjiajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ax.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://nt.colortex.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mc.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oc.shxzskj.cn

Go:   // 按 rune 判断长度后截断
来源：http://ij.asd995.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://jp.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hg.hahajie.cn

[E22] 字节长度与字符长度
来源：http://pk.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://at.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://jm.chemitech.net.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://qh.muxihuayi.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://em.yuexingan06.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://en.szsharing.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ix.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://hp.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://rb.szxytkj.cn

================================================================================
来源：http://td.jctech888.com.cn

F. 文件与目录
来源：http://sp.bookmarksfly.cn

================================================================================
来源：http://gp.gzmigu.cn

[F01] 读取整个文件
来源：http://vt.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ys.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://vr.shtwfgs.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vq.chemitech.net.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bc.hnjuh.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://nf.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ux.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://km.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://rt.hnjuh.cn

[F02] 逐行读取文件
来源：http://kb.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fs.nszjky.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yl.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ux.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lr.bjjhwx.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://iy.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ej.colortex.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://du.colortex.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://bo.newstarts.cn

[F03] 写入文件（覆盖）
来源：http://so.muxihuayi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://sz.lnxyls.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://vd.jianghongdianzi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vu.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://gk.asd995.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://vr.panjiajie.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gr.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://ha.asd995.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://me.nszjky.cn

[F04] 追加写入文件
来源：http://zn.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fl.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rv.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pa.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bx.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://fo.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qo.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nt.colortex.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hy.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://oo.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pz.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://um.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://ba.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://kq.wgjwhj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://jo.lnxyls.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mf.bookmarksfly.cn

Ruby: File.exist?("a.txt")
来源：http://vo.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://zr.hahajie.cn

[F06] 删除文件
来源：http://uw.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://pd.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://as.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qe.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://te.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ik.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://pr.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://pk.chemitech.net.cn

C#:   File.Delete("a.txt");
来源：http://md.jianghongdianzi.cn

[F07] 创建目录（含多级）
来源：http://ad.nicolike.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fs.colortex.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vc.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wx.hnjuh.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ss.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://md.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://an.hnjuh.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ln.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pq.yuntaijiaju.cn

[F08] 遍历目录
来源：http://xw.yuntaijiaju.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://qn.huixiangedu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://sl.huixinmuqiang.cn

JS:   fs.readdirSync("dir")
来源：http://pa.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://th.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://vz.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mi.asd995.cn

Ruby: Dir.children("dir")
来源：http://ji.wgjwhj.cn

C#:   Directory.GetFiles("dir")
来源：http://km.nicolike.cn

[F09] 获取文件大小
来源：http://po.gzmigu.cn

Py:   os.path.getsize("a.txt")
来源：http://ad.panjiajie.cn

PHP:  filesize("a.txt");
来源：http://yd.hnjuh.cn

JS:   fs.statSync("a.txt").size
来源：http://bm.haigaiapp.cn

TS:   fs.statSync("a.txt").size
来源：http://ku.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://yf.yuexingan06.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zw.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://qy.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ox.521024.cn

[F10] 取文件扩展名 / 文件名
来源：http://nf.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tb.wgjwhj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nn.huanxung.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ct.newstarts.cn

TS:   path.extname("a.txt")
来源：http://pq.szxytkj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://du.shxzukj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://by.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gp.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://qr.shtwfgs.cn

[F11] 复制与移动文件
来源：http://is.yuntaijiaju.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://en.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://oj.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bu.szsharing.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://tz.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ww.szsharing.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ic.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://xf.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://pq.hahajie.cn

[F12] CSV 读写
来源：http://qb.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eo.9csxet.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://yj.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://xy.huixiangedu.cn

TS:   // 同上
来源：http://qp.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vy.newstarts.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ih.jianghongdianzi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fb.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://uj.nicolike.cn

================================================================================
来源：http://gt.gzmigu.cn

G. 面向对象
来源：http://vg.huixinmuqiang.cn

================================================================================
来源：http://py.521024.cn

[G01] 定义类
来源：http://lc.hahajie.cn

Py:   class User: pass
来源：http://qk.haigaiapp.cn

PHP:  class User {}
来源：http://lu.szsharing.cn

JS:   class User {}
来源：http://dm.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://fk.asd995.cn

Java: class User {}
来源：http://ar.nicolike.cn

Go:   type User struct { Name string }
来源：http://eb.yuexingan06.cn

Ruby: class User; end
来源：http://hb.lnxyls.cn

C#:   class User {}
来源：http://pq.shxzukj.cn

[G02] 构造函数
来源：http://lm.szxytkj.cn

Py:   def __init__(self, name): self.name = name
来源：http://ey.9csxet.cn

PHP:  public function __construct(public string $name) {}
来源：http://yx.bjjhwx.cn

JS:   constructor(name) { this.name = name; }
来源：http://lc.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://kq.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://yn.hnjuh.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://vg.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://zx.huixinmuqiang.cn

C#:   public User(string name) { Name = name; }
来源：http://ni.9csxet.cn

[G03] 实例属性
来源：http://ar.chemitech.net.cn

Py:   self.name = "x"
来源：http://uz.bjjhwx.cn

PHP:  public string $name = "x";
来源：http://ho.colortex.cn

JS:   this.name = "x";
来源：http://pi.jctech888.com.cn

TS:   name: string = "x";
来源：http://fh.9csxet.cn

Java: private String name;
来源：http://wi.nszjky.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://da.yuntaijiaju.cn

Ruby: @name = "x"
来源：http://ac.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://bl.nszjky.cn

[G04] 定义方法
来源：http://gt.asd995.cn

Py:   def greet(self): return self.name
来源：http://kh.bookmarksfly.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://gl.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://aq.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://bc.szxytkj.cn

Java: String greet() { return name; }
来源：http://ne.newstarts.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hr.gzmigu.cn

Ruby: def greet; @name; end
来源：http://kc.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://um.bjjhwx.cn

[G05] 继承
来源：http://am.lnxyls.cn

Py:   class Admin(User): pass
来源：http://dw.lnxyls.cn

PHP:  class Admin extends User {}
来源：http://fs.bookmarksfly.cn

JS:   class Admin extends User {}
来源：http://qg.asd995.cn

TS:   class Admin extends User {}
来源：http://pb.szsharing.cn

Java: class Admin extends User {}
来源：http://je.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hb.nicolike.cn

Ruby: class Admin < User; end
来源：http://gl.huanxung.cn

C#:   class Admin : User {}
来源：http://uk.wgjwhj.cn

[G06] 重写方法
来源：http://xi.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://fh.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://se.asd995.cn

JS:   greet() { return "admin"; }
来源：http://iy.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ey.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://vg.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://kb.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://yd.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://cs.lnxyls.cn

[G07] 调用父类方法
来源：http://xf.bjjhwx.cn

Py:   super().greet()
来源：http://jd.gzmigu.cn

PHP:  parent::greet();
来源：http://az.nszjky.cn

JS:   super.greet();
来源：http://hv.panjiajie.cn

TS:   super.greet();
来源：http://ar.chemitech.net.cn

Java: super.greet();
来源：http://rx.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xf.huixiangedu.cn

Ruby: super
来源：http://vq.huanxung.cn

C#:   base.Greet();
来源：http://gw.newstarts.cn

[G08] 静态方法与属性
来源：http://hj.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qp.panjiajie.cn

PHP:  public static function f() {}
来源：http://ec.nicolike.cn

JS:   static f() {}
来源：http://cb.shxzskj.cn

TS:   static f(): void {}
来源：http://ec.asd995.cn

Java: static void f() {}
来源：http://he.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://em.szsharing.cn

Ruby: def self.f; end
来源：http://uj.panjiajie.cn

C#:   public static void F() {}
来源：http://nq.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://fw.chemitech.net.cn

Py:   from abc import ABC, abstractmethod
来源：http://aj.huixiangedu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://od.yuntaijiaju.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ay.szsharing.cn

TS:   interface Shape { area(): number; }
来源：http://rp.muxihuayi.cn

Java: interface Shape { double area(); }
来源：http://wc.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://es.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mj.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://mi.gzmigu.cn

[G10] 访问控制
来源：http://gw.szxytkj.cn

Py:   约定 _protected / __private（不强制）
来源：http://sc.shxzskj.cn

PHP:  public / protected / private
来源：http://yg.nicolike.cn

JS:   #private 字段；其余公开
来源：http://fk.bjjhwx.cn

TS:   public / protected / private
来源：http://jw.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://bu.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://sf.yuexingan06.cn

Ruby: public / protected / private
来源：http://uf.lnxyls.cn

C#:   public / protected / private / internal
来源：http://bl.shxzukj.cn

[G11] getter / setter
来源：http://mj.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://ul.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hg.9csxet.cn

JS:   get name() { return this._name; }
来源：http://cc.shxzskj.cn

TS:   get name(): string { return this._name; }
来源：http://bu.hahajie.cn

Java: public String getName() { return name; }
来源：http://pa.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://vw.9csxet.cn

Ruby: attr_accessor :name
来源：http://rt.asd995.cn

C#:   public string Name { get; set; }
来源：http://pz.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://pn.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://iz.colortex.cn


<!-- 参考信息 -->