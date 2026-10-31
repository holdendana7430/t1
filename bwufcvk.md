代发 wailian999

[E14] URL 编码与 Base64
来源：http://wk.haigaiapp.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://fn.jianghongdianzi.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://ba.hahajie.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://te.521024.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://bg.nicolike.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://zx.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wf.bjjhwx.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://xy.lnxyls.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wb.colortex.cn

[E15] HTML 转义 / 反转义
来源：http://lz.panjiajie.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://wl.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://qz.szxytkj.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://fb.521024.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://vy.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wa.jctech888.com.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rx.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://is.lnxyls.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://vz.wgjwhj.cn

[E16] 数字千分位
来源：http://mv.hahajie.cn

Py:   f"{1234567:,}"
来源：http://td.jianghongdianzi.cn

PHP:  number_format(1234567);
来源：http://bw.gzmigu.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://dx.nicolike.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://gn.shxzskj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://tn.shxzukj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xw.bookmarksfly.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://pk.newstarts.cn

C#:   1234567.ToString("N0")
来源：http://nz.bookmarksfly.cn

[E17] 首字母大写
来源：http://ei.wgjwhj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://sb.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://um.chemitech.net.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://lk.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ap.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gz.hahajie.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ct.yuexingan06.cn

Ruby: s.capitalize
来源：http://xo.asd995.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://np.hahajie.cn

[E18] 模板占位符替换
来源：http://ab.shxzskj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ws.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://kc.huixiangedu.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://gm.shxzukj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://xy.colortex.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ve.shxzskj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://cg.jctech888.com.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ik.lnxyls.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yo.gzmigu.cn

[E19] 多行文本按行拆分
来源：http://po.shtwfgs.cn

Py:   s.splitlines()
来源：http://re.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dl.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://lb.nszjky.cn

TS:   s.split(/\r?\n/)
来源：http://zg.shtwfgs.cn

Java: s.lines().toList()
来源：http://dd.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://ui.yuexingan06.cn

Ruby: s.lines
来源：http://wr.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://qq.yuntaijiaju.cn

[E20] 判断字符串是否为空
来源：http://ny.nicolike.cn

Py:   if not s:
来源：http://lg.szxytkj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://az.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ed.muxihuayi.cn

TS:   if (s === "") {}
来源：http://qa.bjjhwx.cn

Java: if (s.isEmpty()) {}
来源：http://um.gzmigu.cn

Go:   if s == "" {}
来源：http://db.lnxyls.cn

Ruby: if s.empty?
来源：http://jv.huixinmuqiang.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gc.colortex.cn

[E21] 超长截断加省略号
来源：http://jq.lnxyls.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ei.jianghongdianzi.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://ep.521024.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://vj.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ar.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ie.panjiajie.cn

Go:   // 按 rune 判断长度后截断
来源：http://kh.bjjhwx.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://dw.yuntaijiaju.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://sk.nicolike.cn

[E22] 字节长度与字符长度
来源：http://cb.szxytkj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ts.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uj.asd995.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://kr.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://my.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nt.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://cm.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://nn.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ny.colortex.cn

================================================================================
来源：http://ua.chemitech.net.cn

F. 文件与目录
来源：http://zp.nszjky.cn

================================================================================
来源：http://oc.huixinmuqiang.cn

[F01] 读取整个文件
来源：http://tt.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://lj.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://pc.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://au.huanxung.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://me.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pe.shxzskj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dg.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ej.huanxung.cn

C#:   File.ReadAllText("a.txt");
来源：http://uw.nicolike.cn

[F02] 逐行读取文件
来源：http://vl.muxihuayi.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ig.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://at.chemitech.net.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wm.huanxung.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wy.wgjwhj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hm.yuntaijiaju.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pb.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://qs.gzmigu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zt.asd995.cn

[F03] 写入文件（覆盖）
来源：http://vs.huixiangedu.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oh.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nf.gzmigu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vu.lnxyls.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fj.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://nq.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xp.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://sk.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://lz.szsharing.cn

[F04] 追加写入文件
来源：http://rq.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zs.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ld.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gf.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ee.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zw.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ag.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://eg.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hl.521024.cn

[F05] 判断文件或目录是否存在
来源：http://vr.hnjuh.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://yc.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://at.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://ld.hahajie.cn

TS:   fs.existsSync("a.txt")
来源：http://hs.gzmigu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sz.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://of.jctech888.com.cn

Ruby: File.exist?("a.txt")
来源：http://xd.haigaiapp.cn

C#:   File.Exists("a.txt")
来源：http://lk.yuntaijiaju.cn

[F06] 删除文件
来源：http://kj.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://sr.colortex.cn

PHP:  unlink("a.txt");
来源：http://ls.huixiangedu.cn

JS:   fs.unlinkSync("a.txt")
来源：http://fj.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pi.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://eq.yuntaijiaju.cn

Go:   os.Remove("a.txt")
来源：http://gi.panjiajie.cn

Ruby: File.delete("a.txt")
来源：http://jb.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://bo.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://nk.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://as.gzmigu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ub.huixinmuqiang.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mw.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gp.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ww.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://um.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://qx.nszjky.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://jf.hnjuh.cn

[F08] 遍历目录
来源：http://he.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mo.muxihuayi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uw.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://cj.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://ji.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tc.haigaiapp.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ji.huixinmuqiang.cn

Ruby: Dir.children("dir")
来源：http://yp.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://bk.nszjky.cn

[F09] 获取文件大小
来源：http://cq.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://of.colortex.cn

PHP:  filesize("a.txt");
来源：http://kt.nicolike.cn

JS:   fs.statSync("a.txt").size
来源：http://rr.nszjky.cn

TS:   fs.statSync("a.txt").size
来源：http://fk.9csxet.cn

Java: Files.size(Path.of("a.txt"))
来源：http://jv.shxzukj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zd.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://vk.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://qp.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://xu.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nc.lnxyls.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ng.lnxyls.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bh.gzmigu.cn

TS:   path.extname("a.txt")
来源：http://ky.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cf.chemitech.net.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pa.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://fb.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://ux.szxytkj.cn

[F11] 复制与移动文件
来源：http://yg.haigaiapp.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://vs.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://qa.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fs.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ac.asd995.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hj.haigaiapp.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://eq.szsharing.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://yj.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ry.asd995.cn

[F12] CSV 读写
来源：http://kh.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mk.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ch.shxzukj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ym.szxytkj.cn

TS:   // 同上
来源：http://ts.9csxet.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fx.shtwfgs.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://fl.muxihuayi.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://kt.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pt.nszjky.cn

================================================================================
来源：http://ca.yuntaijiaju.cn

G. 面向对象
来源：http://uc.lnxyls.cn

================================================================================
来源：http://xn.chemitech.net.cn

[G01] 定义类
来源：http://nk.gzmigu.cn

Py:   class User: pass
来源：http://mn.wgjwhj.cn

PHP:  class User {}
来源：http://ef.hahajie.cn

JS:   class User {}
来源：http://tx.muxihuayi.cn

TS:   class User { name: string = ""; }
来源：http://le.haigaiapp.cn

Java: class User {}
来源：http://sb.panjiajie.cn

Go:   type User struct { Name string }
来源：http://zs.huanxung.cn

Ruby: class User; end
来源：http://cq.hahajie.cn

C#:   class User {}
来源：http://vg.521024.cn

[G02] 构造函数
来源：http://rl.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://yn.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://xx.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://qz.hnjuh.cn

TS:   constructor(public name: string) {}
来源：http://hx.jianghongdianzi.cn

Java: User(String name) { this.name = name; }
来源：http://bl.bjjhwx.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ke.muxihuayi.cn

Ruby: def initialize(name); @name = name; end
来源：http://xn.panjiajie.cn

C#:   public User(string name) { Name = name; }
来源：http://wm.chemitech.net.cn

[G03] 实例属性
来源：http://km.colortex.cn

Py:   self.name = "x"
来源：http://lv.shtwfgs.cn

PHP:  public string $name = "x";
来源：http://vm.nicolike.cn

JS:   this.name = "x";
来源：http://ba.colortex.cn

TS:   name: string = "x";
来源：http://wc.yuexingan06.cn

Java: private String name;
来源：http://ib.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nu.bjjhwx.cn

Ruby: @name = "x"
来源：http://xy.521024.cn

C#:   public string Name { get; set; } = "x";
来源：http://ws.huixinmuqiang.cn

[G04] 定义方法
来源：http://vl.jianghongdianzi.cn

Py:   def greet(self): return self.name
来源：http://rg.jianghongdianzi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://nv.shtwfgs.cn

JS:   greet() { return this.name; }
来源：http://oa.szxytkj.cn

TS:   greet(): string { return this.name; }
来源：http://oi.jctech888.com.cn

Java: String greet() { return name; }
来源：http://xp.shxzukj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bj.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://mm.shxzskj.cn

C#:   public string Greet() => Name;
来源：http://te.huixinmuqiang.cn

[G05] 继承
来源：http://bb.shtwfgs.cn

Py:   class Admin(User): pass
来源：http://iy.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://wr.muxihuayi.cn

JS:   class Admin extends User {}
来源：http://fe.wgjwhj.cn

TS:   class Admin extends User {}
来源：http://km.hnjuh.cn

Java: class Admin extends User {}
来源：http://ce.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://va.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://pl.asd995.cn

C#:   class Admin : User {}
来源：http://ct.colortex.cn

[G06] 重写方法
来源：http://zt.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://im.bookmarksfly.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://uj.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://tx.huanxung.cn

TS:   greet(): string { return "admin"; }
来源：http://hx.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://su.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fm.huixiangedu.cn

Ruby: def greet; "admin"; end
来源：http://gu.521024.cn

C#:   public override string Greet() => "admin";
来源：http://td.szsharing.cn

[G07] 调用父类方法
来源：http://ue.521024.cn

Py:   super().greet()
来源：http://kx.521024.cn

PHP:  parent::greet();
来源：http://xx.panjiajie.cn

JS:   super.greet();
来源：http://tc.colortex.cn

TS:   super.greet();
来源：http://pj.haigaiapp.cn

Java: super.greet();
来源：http://fa.shxzukj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ce.hnjuh.cn

Ruby: super
来源：http://dm.colortex.cn

C#:   base.Greet();
来源：http://qy.gzmigu.cn

[G08] 静态方法与属性
来源：http://ud.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ib.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://wh.huanxung.cn

JS:   static f() {}
来源：http://tn.jctech888.com.cn

TS:   static f(): void {}
来源：http://eh.panjiajie.cn

Java: static void f() {}
来源：http://pi.nszjky.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ze.gzmigu.cn

Ruby: def self.f; end
来源：http://uy.gzmigu.cn

C#:   public static void F() {}
来源：http://fd.szxytkj.cn

[G09] 接口 / 抽象类
来源：http://ax.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://fp.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://no.bjjhwx.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xq.hnjuh.cn

TS:   interface Shape { area(): number; }
来源：http://co.wgjwhj.cn

Java: interface Shape { double area(); }
来源：http://pn.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://vz.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://oc.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://zu.shxzukj.cn

[G10] 访问控制
来源：http://ya.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://mg.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://gh.9csxet.cn

JS:   #private 字段；其余公开
来源：http://qo.shxzukj.cn

TS:   public / protected / private
来源：http://cv.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://tc.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xc.huixiangedu.cn

Ruby: public / protected / private
来源：http://zv.lnxyls.cn

C#:   public / protected / private / internal
来源：http://jk.wgjwhj.cn

[G11] getter / setter
来源：http://la.nicolike.cn

Py:   @property 与 @x.setter
来源：http://tr.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://jc.521024.cn

JS:   get name() { return this._name; }
来源：http://ju.shxzukj.cn

TS:   get name(): string { return this._name; }
来源：http://zb.nszjky.cn

Java: public String getName() { return name; }
来源：http://ue.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xg.lnxyls.cn

Ruby: attr_accessor :name
来源：http://cv.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://og.nszjky.cn

[G12] 对象转字符串
来源：http://dl.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://dd.hahajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yy.huixinmuqiang.cn

JS:   toString() { return this.name; }
来源：http://mt.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://eq.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://az.newstarts.cn


<!-- 参考信息 -->