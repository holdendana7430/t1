代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://vz.hahajie.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ny.9csxet.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://co.szsharing.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://oj.jctech888.com.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://nv.bjjhwx.cn

[E15] HTML 转义 / 反转义
来源：http://om.asd995.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qe.shxzskj.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ii.panjiajie.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://tq.shxzskj.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://bs.jctech888.com.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://dj.panjiajie.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wd.panjiajie.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://dm.shtwfgs.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zw.colortex.cn

[E16] 数字千分位
来源：http://pb.huixinmuqiang.cn

Py:   f"{1234567:,}"
来源：http://mm.panjiajie.cn

PHP:  number_format(1234567);
来源：http://xr.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://pr.521024.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://db.chemitech.net.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ol.szxytkj.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://vb.huixinmuqiang.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ze.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://fy.9csxet.cn

[E17] 首字母大写
来源：http://yu.jianghongdianzi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://oq.9csxet.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://yx.bookmarksfly.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://bj.bjjhwx.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ze.szxytkj.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://oo.nicolike.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gt.jianghongdianzi.cn

Ruby: s.capitalize
来源：http://rx.nicolike.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://qm.szxytkj.cn

[E18] 模板占位符替换
来源：http://gv.shxzukj.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bx.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yf.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qz.yuexingan06.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://qe.9csxet.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ro.chemitech.net.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lb.shtwfgs.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ec.yuntaijiaju.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://dn.bjjhwx.cn

[E19] 多行文本按行拆分
来源：http://fd.huixiangedu.cn

Py:   s.splitlines()
来源：http://fr.szsharing.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dm.szxytkj.cn

JS:   s.split(/\r?\n/)
来源：http://ml.muxihuayi.cn

TS:   s.split(/\r?\n/)
来源：http://gs.nicolike.cn

Java: s.lines().toList()
来源：http://hy.jctech888.com.cn

Go:   strings.Split(s, "\n")
来源：http://cl.nicolike.cn

Ruby: s.lines
来源：http://jp.yuntaijiaju.cn

C#:   s.Split('\n')
来源：http://vf.gzmigu.cn

[E20] 判断字符串是否为空
来源：http://oe.hnjuh.cn

Py:   if not s:
来源：http://se.bookmarksfly.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ua.chemitech.net.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ho.shxzukj.cn

TS:   if (s === "") {}
来源：http://om.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://be.wgjwhj.cn

Go:   if s == "" {}
来源：http://ur.chemitech.net.cn

Ruby: if s.empty?
来源：http://hn.shxzskj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://eg.jianghongdianzi.cn

[E21] 超长截断加省略号
来源：http://of.yuexingan06.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jd.hahajie.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://if.yuexingan06.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://sa.nszjky.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lk.nicolike.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nz.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://zr.huanxung.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hn.gzmigu.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zt.9csxet.cn

[E22] 字节长度与字符长度
来源：http://sp.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://rc.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cw.huixiangedu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://lc.szsharing.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sm.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nm.521024.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hk.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://fp.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hu.nicolike.cn

================================================================================
来源：http://ja.yuntaijiaju.cn

F. 文件与目录
来源：http://db.yuntaijiaju.cn

================================================================================
来源：http://nz.muxihuayi.cn

[F01] 读取整个文件
来源：http://xp.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gb.bookmarksfly.cn

PHP:  file_get_contents("a.txt");
来源：http://ik.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://vj.jctech888.com.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vv.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://hk.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bl.shxzukj.cn

Ruby: File.read("a.txt")
来源：http://wx.bjjhwx.cn

C#:   File.ReadAllText("a.txt");
来源：http://kb.hnjuh.cn

[F02] 逐行读取文件
来源：http://wp.gzmigu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ux.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ej.szsharing.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sa.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ew.huanxung.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://tf.hahajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hv.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://dg.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://xu.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://nv.jianghongdianzi.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://el.colortex.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nt.bjjhwx.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bk.bookmarksfly.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wr.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ae.szxytkj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://zu.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://pc.chemitech.net.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oy.chemitech.net.cn

[F04] 追加写入文件
来源：http://bk.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jq.huixinmuqiang.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ni.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ja.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://aa.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://de.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://dw.haigaiapp.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hv.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://il.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://zn.panjiajie.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fd.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://hz.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ub.jianghongdianzi.cn

TS:   fs.existsSync("a.txt")
来源：http://gb.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://br.nicolike.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mg.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://mz.yuntaijiaju.cn

C#:   File.Exists("a.txt")
来源：http://nw.szxytkj.cn

[F06] 删除文件
来源：http://er.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://cb.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://li.nszjky.cn

JS:   fs.unlinkSync("a.txt")
来源：http://la.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://au.huanxung.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://on.huixinmuqiang.cn

Go:   os.Remove("a.txt")
来源：http://we.9csxet.cn

Ruby: File.delete("a.txt")
来源：http://li.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://ef.colortex.cn

[F07] 创建目录（含多级）
来源：http://ox.huixinmuqiang.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://eo.szsharing.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vz.szsharing.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kb.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gz.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://bw.nszjky.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://zj.yuntaijiaju.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wi.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wp.shtwfgs.cn

[F08] 遍历目录
来源：http://bz.jianghongdianzi.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zg.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ym.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://as.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://na.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://tb.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wb.yuntaijiaju.cn

Ruby: Dir.children("dir")
来源：http://ua.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://hw.szxytkj.cn

[F09] 获取文件大小
来源：http://tc.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://oa.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://gh.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://qk.szxytkj.cn

TS:   fs.statSync("a.txt").size
来源：http://sf.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ke.panjiajie.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://iz.colortex.cn

Ruby: File.size("a.txt")
来源：http://mk.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://bd.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://gb.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qv.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qp.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lf.nicolike.cn

TS:   path.extname("a.txt")
来源：http://nt.panjiajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ba.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://dw.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wf.shtwfgs.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lx.yuexingan06.cn

[F11] 复制与移动文件
来源：http://nd.shtwfgs.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ho.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://fr.huanxung.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://da.chemitech.net.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fx.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://pu.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://xk.jianghongdianzi.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://an.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mi.shxzskj.cn

[F12] CSV 读写
来源：http://kk.bjjhwx.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://fa.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://zg.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://zo.9csxet.cn

TS:   // 同上
来源：http://su.haigaiapp.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hf.521024.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://nn.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xk.shxzukj.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://nj.yuntaijiaju.cn

================================================================================
来源：http://ih.colortex.cn

G. 面向对象
来源：http://gg.lnxyls.cn

================================================================================
来源：http://nb.panjiajie.cn

[G01] 定义类
来源：http://nf.colortex.cn

Py:   class User: pass
来源：http://so.huixiangedu.cn

PHP:  class User {}
来源：http://gt.hnjuh.cn

JS:   class User {}
来源：http://tf.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ep.newstarts.cn

Java: class User {}
来源：http://tf.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://ip.hahajie.cn

Ruby: class User; end
来源：http://ov.huixiangedu.cn

C#:   class User {}
来源：http://vt.panjiajie.cn

[G02] 构造函数
来源：http://ak.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://gl.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://wj.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://ek.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://nh.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://pm.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nw.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://kf.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://no.hnjuh.cn

[G03] 实例属性
来源：http://ow.hahajie.cn

Py:   self.name = "x"
来源：http://xh.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://md.bookmarksfly.cn

JS:   this.name = "x";
来源：http://mq.shxzskj.cn

TS:   name: string = "x";
来源：http://rw.bookmarksfly.cn

Java: private String name;
来源：http://zk.haigaiapp.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://eh.hnjuh.cn

Ruby: @name = "x"
来源：http://xf.szsharing.cn

C#:   public string Name { get; set; } = "x";
来源：http://vx.9csxet.cn

[G04] 定义方法
来源：http://vc.huixiangedu.cn

Py:   def greet(self): return self.name
来源：http://dk.hnjuh.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ki.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://xb.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://nz.nszjky.cn

Java: String greet() { return name; }
来源：http://ao.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://vy.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://em.shtwfgs.cn

C#:   public string Greet() => Name;
来源：http://up.szxytkj.cn

[G05] 继承
来源：http://lc.jctech888.com.cn

Py:   class Admin(User): pass
来源：http://pe.colortex.cn

PHP:  class Admin extends User {}
来源：http://vw.jctech888.com.cn

JS:   class Admin extends User {}
来源：http://bs.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ff.gzmigu.cn

Java: class Admin extends User {}
来源：http://sg.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rd.huanxung.cn

Ruby: class Admin < User; end
来源：http://tc.haigaiapp.cn

C#:   class Admin : User {}
来源：http://oi.nszjky.cn

[G06] 重写方法
来源：http://ff.yuexingan06.cn

Py:   def greet(self): return "admin"
来源：http://gg.szsharing.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sc.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://ao.chemitech.net.cn

TS:   greet(): string { return "admin"; }
来源：http://hk.newstarts.cn

Java: @Override String greet() { return "admin"; }
来源：http://mm.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://tg.bjjhwx.cn

Ruby: def greet; "admin"; end
来源：http://ym.nicolike.cn

C#:   public override string Greet() => "admin";
来源：http://rk.szxytkj.cn

[G07] 调用父类方法
来源：http://tt.szxytkj.cn

Py:   super().greet()
来源：http://iy.9csxet.cn

PHP:  parent::greet();
来源：http://rk.szxytkj.cn

JS:   super.greet();
来源：http://hk.hnjuh.cn

TS:   super.greet();
来源：http://mq.haigaiapp.cn

Java: super.greet();
来源：http://lf.jctech888.com.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://tl.jianghongdianzi.cn

Ruby: super
来源：http://nr.muxihuayi.cn

C#:   base.Greet();
来源：http://le.chemitech.net.cn

[G08] 静态方法与属性
来源：http://mk.9csxet.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://vj.yuexingan06.cn

PHP:  public static function f() {}
来源：http://vw.panjiajie.cn

JS:   static f() {}
来源：http://sv.hahajie.cn

TS:   static f(): void {}
来源：http://nr.hahajie.cn

Java: static void f() {}
来源：http://pd.bookmarksfly.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://kn.shxzskj.cn

Ruby: def self.f; end
来源：http://rp.nicolike.cn

C#:   public static void F() {}
来源：http://fr.hahajie.cn

[G09] 接口 / 抽象类
来源：http://ks.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://zn.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zt.gzmigu.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ru.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://pn.huixiangedu.cn

Java: interface Shape { double area(); }
来源：http://ue.shxzskj.cn

Go:   type Shape interface { Area() float64 }
来源：http://um.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sp.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://if.bjjhwx.cn

[G10] 访问控制
来源：http://qn.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://ne.panjiajie.cn

PHP:  public / protected / private
来源：http://tk.521024.cn

JS:   #private 字段；其余公开
来源：http://an.panjiajie.cn

TS:   public / protected / private
来源：http://mu.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://td.newstarts.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://rk.haigaiapp.cn

Ruby: public / protected / private
来源：http://wd.nszjky.cn

C#:   public / protected / private / internal
来源：http://zb.asd995.cn

[G11] getter / setter
来源：http://tj.shxzskj.cn

Py:   @property 与 @x.setter
来源：http://uw.bjjhwx.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://qh.szxytkj.cn

JS:   get name() { return this._name; }
来源：http://uh.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://cj.shtwfgs.cn

Java: public String getName() { return name; }
来源：http://vc.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://md.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://sf.521024.cn

C#:   public string Name { get; set; }
来源：http://lx.wgjwhj.cn

[G12] 对象转字符串
来源：http://ge.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://bn.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ct.shxzskj.cn

JS:   toString() { return this.name; }
来源：http://yn.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://bp.asd995.cn

Java: @Override public String toString() { return name; }
来源：http://vc.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://mi.bookmarksfly.cn

Ruby: def to_s; @name; end
来源：http://sn.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://ec.521024.cn

[G13] 判断对象类型
来源：http://uw.hahajie.cn


<!-- 参考信息 -->