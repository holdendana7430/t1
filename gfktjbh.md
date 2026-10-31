代发 wailian999

[E14] URL 编码与 Base64
来源：http://ge.huanxung.cn

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hq.nicolike.cn

PHP:  urlencode($s);  base64_encode($s);
来源：http://xu.nicolike.cn

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://ze.chemitech.net.cn

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ll.wgjwhj.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://va.wgjwhj.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://db.lnxyls.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wz.shtwfgs.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://et.haigaiapp.cn

[E15] HTML 转义 / 反转义
来源：http://ln.nicolike.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://qj.asd995.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ir.yuntaijiaju.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://kk.chemitech.net.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://lq.bookmarksfly.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://az.chemitech.net.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://oa.shxzskj.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mg.bookmarksfly.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://cn.bookmarksfly.cn

[E16] 数字千分位
来源：http://co.shxzskj.cn

Py:   f"{1234567:,}"
来源：http://ni.muxihuayi.cn

PHP:  number_format(1234567);
来源：http://pp.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://zn.bookmarksfly.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://na.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://or.jctech888.com.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://xa.nszjky.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://am.colortex.cn

C#:   1234567.ToString("N0")
来源：http://ug.shtwfgs.cn

[E17] 首字母大写
来源：http://kj.chemitech.net.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wz.jianghongdianzi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://gf.jctech888.com.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ur.yuntaijiaju.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ly.hnjuh.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ft.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sm.nicolike.cn

Ruby: s.capitalize
来源：http://rc.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://bm.muxihuayi.cn

[E18] 模板占位符替换
来源：http://gc.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://dq.yuntaijiaju.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://br.shtwfgs.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://te.hnjuh.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://my.nicolike.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://rg.hahajie.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://lu.shxzukj.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://oj.haigaiapp.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ly.huixinmuqiang.cn

[E19] 多行文本按行拆分
来源：http://tq.bookmarksfly.cn

Py:   s.splitlines()
来源：http://fo.gzmigu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://jw.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ul.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://gx.newstarts.cn

Java: s.lines().toList()
来源：http://zy.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://xh.szxytkj.cn

Ruby: s.lines
来源：http://xm.huixiangedu.cn

C#:   s.Split('\n')
来源：http://xm.hahajie.cn

[E20] 判断字符串是否为空
来源：http://rd.szsharing.cn

Py:   if not s:
来源：http://tc.shxzukj.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://js.colortex.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ks.chemitech.net.cn

TS:   if (s === "") {}
来源：http://ku.muxihuayi.cn

Java: if (s.isEmpty()) {}
来源：http://cc.muxihuayi.cn

Go:   if s == "" {}
来源：http://bf.shtwfgs.cn

Ruby: if s.empty?
来源：http://il.newstarts.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://yj.szsharing.cn

[E21] 超长截断加省略号
来源：http://ik.panjiajie.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://id.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://oe.nszjky.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dt.wgjwhj.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://pp.lnxyls.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mo.szsharing.cn

Go:   // 按 rune 判断长度后截断
来源：http://pm.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://uc.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wa.hahajie.cn

[E22] 字节长度与字符长度
来源：http://an.521024.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jb.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://rz.hnjuh.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ik.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lp.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nh.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://jx.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://ss.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ps.newstarts.cn

================================================================================
来源：http://wd.521024.cn

F. 文件与目录
来源：http://gb.newstarts.cn

================================================================================
来源：http://hz.shxzskj.cn

[F01] 读取整个文件
来源：http://ft.nicolike.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://xy.szxytkj.cn

PHP:  file_get_contents("a.txt");
来源：http://eo.muxihuayi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://oq.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://sf.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ys.haigaiapp.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lq.szsharing.cn

Ruby: File.read("a.txt")
来源：http://po.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://au.nszjky.cn

[F02] 逐行读取文件
来源：http://vd.szsharing.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://cu.huanxung.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ar.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bu.9csxet.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zl.haigaiapp.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://kz.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://af.lnxyls.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ca.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://oh.asd995.cn

[F03] 写入文件（覆盖）
来源：http://uq.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mr.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://pl.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sl.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ng.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://et.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fc.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://wf.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://is.gzmigu.cn

[F04] 追加写入文件
来源：http://xi.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://yy.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sm.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ky.jctech888.com.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ry.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://gf.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hk.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wq.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sm.huixinmuqiang.cn

[F05] 判断文件或目录是否存在
来源：http://sj.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://cy.nszjky.cn

PHP:  file_exists("a.txt");
来源：http://tg.bjjhwx.cn

JS:   fs.existsSync("a.txt")
来源：http://kw.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://ld.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ri.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fm.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://wf.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://ox.chemitech.net.cn

[F06] 删除文件
来源：http://yq.huixiangedu.cn

Py:   os.remove("a.txt")
来源：http://wd.colortex.cn

PHP:  unlink("a.txt");
来源：http://se.szsharing.cn

JS:   fs.unlinkSync("a.txt")
来源：http://bn.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://df.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://nj.panjiajie.cn

Go:   os.Remove("a.txt")
来源：http://sn.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://dk.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://zk.9csxet.cn

[F07] 创建目录（含多级）
来源：http://gk.yuexingan06.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://da.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ko.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zu.panjiajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mi.lnxyls.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ll.bookmarksfly.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xn.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ki.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://gw.hahajie.cn

[F08] 遍历目录
来源：http://zg.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ob.jctech888.com.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hw.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://fk.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://st.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gp.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xq.9csxet.cn

Ruby: Dir.children("dir")
来源：http://yt.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://of.asd995.cn

[F09] 获取文件大小
来源：http://jt.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://fx.nszjky.cn

PHP:  filesize("a.txt");
来源：http://ul.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://ef.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://zf.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://wf.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://ip.huanxung.cn

Ruby: File.size("a.txt")
来源：http://co.521024.cn

C#:   new FileInfo("a.txt").Length
来源：http://hm.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ho.huixinmuqiang.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://cp.szxytkj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wr.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://on.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://zr.hnjuh.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ny.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mz.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gd.nszjky.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zp.yuexingan06.cn

[F11] 复制与移动文件
来源：http://mv.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://bm.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://gy.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bo.huanxung.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ab.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://dq.szxytkj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://im.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hb.muxihuayi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sz.hahajie.cn

[F12] CSV 读写
来源：http://xy.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ap.jianghongdianzi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qj.lnxyls.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qn.jctech888.com.cn

TS:   // 同上
来源：http://hp.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://eq.lnxyls.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://md.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xs.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sd.9csxet.cn

================================================================================
来源：http://iw.jianghongdianzi.cn

G. 面向对象
来源：http://yi.9csxet.cn

================================================================================
来源：http://un.huanxung.cn

[G01] 定义类
来源：http://ye.bjjhwx.cn

Py:   class User: pass
来源：http://qo.yuntaijiaju.cn

PHP:  class User {}
来源：http://km.haigaiapp.cn

JS:   class User {}
来源：http://yf.yuntaijiaju.cn

TS:   class User { name: string = ""; }
来源：http://yx.szsharing.cn

Java: class User {}
来源：http://bt.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://fm.gzmigu.cn

Ruby: class User; end
来源：http://do.haigaiapp.cn

C#:   class User {}
来源：http://ut.shxzskj.cn

[G02] 构造函数
来源：http://au.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://eu.asd995.cn

PHP:  public function __construct(public string $name) {}
来源：http://ty.huixiangedu.cn

JS:   constructor(name) { this.name = name; }
来源：http://yv.521024.cn

TS:   constructor(public name: string) {}
来源：http://we.huixinmuqiang.cn

Java: User(String name) { this.name = name; }
来源：http://tp.haigaiapp.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://aw.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://em.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://al.szsharing.cn

[G03] 实例属性
来源：http://mw.huixiangedu.cn

Py:   self.name = "x"
来源：http://ya.asd995.cn

PHP:  public string $name = "x";
来源：http://ko.muxihuayi.cn

JS:   this.name = "x";
来源：http://cx.nicolike.cn

TS:   name: string = "x";
来源：http://yc.9csxet.cn

Java: private String name;
来源：http://xy.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://vy.huixiangedu.cn

Ruby: @name = "x"
来源：http://zy.shtwfgs.cn

C#:   public string Name { get; set; } = "x";
来源：http://zn.bjjhwx.cn

[G04] 定义方法
来源：http://yu.colortex.cn

Py:   def greet(self): return self.name
来源：http://tk.chemitech.net.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ij.nicolike.cn

JS:   greet() { return this.name; }
来源：http://pc.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://dr.nszjky.cn

Java: String greet() { return name; }
来源：http://xp.521024.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://qa.nicolike.cn

Ruby: def greet; @name; end
来源：http://va.huixinmuqiang.cn

C#:   public string Greet() => Name;
来源：http://uy.shxzukj.cn

[G05] 继承
来源：http://kf.colortex.cn

Py:   class Admin(User): pass
来源：http://by.nszjky.cn

PHP:  class Admin extends User {}
来源：http://es.nszjky.cn

JS:   class Admin extends User {}
来源：http://xb.asd995.cn

TS:   class Admin extends User {}
来源：http://by.521024.cn

Java: class Admin extends User {}
来源：http://vg.newstarts.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://at.bookmarksfly.cn

Ruby: class Admin < User; end
来源：http://oz.nszjky.cn

C#:   class Admin : User {}
来源：http://mm.nicolike.cn

[G06] 重写方法
来源：http://oc.jctech888.com.cn

Py:   def greet(self): return "admin"
来源：http://fg.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fu.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://jc.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://ip.wgjwhj.cn

Java: @Override String greet() { return "admin"; }
来源：http://pp.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://cf.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://ye.haigaiapp.cn

C#:   public override string Greet() => "admin";
来源：http://lq.shtwfgs.cn

[G07] 调用父类方法
来源：http://fb.shxzskj.cn

Py:   super().greet()
来源：http://ab.shxzskj.cn

PHP:  parent::greet();
来源：http://zy.lnxyls.cn

JS:   super.greet();
来源：http://on.huixinmuqiang.cn

TS:   super.greet();
来源：http://le.szxytkj.cn

Java: super.greet();
来源：http://rt.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://xt.shxzukj.cn

Ruby: super
来源：http://fi.haigaiapp.cn

C#:   base.Greet();
来源：http://vm.colortex.cn

[G08] 静态方法与属性
来源：http://jb.nszjky.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nj.hahajie.cn

PHP:  public static function f() {}
来源：http://bv.hnjuh.cn

JS:   static f() {}
来源：http://rk.gzmigu.cn

TS:   static f(): void {}
来源：http://hf.muxihuayi.cn

Java: static void f() {}
来源：http://ub.hnjuh.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://he.panjiajie.cn

Ruby: def self.f; end
来源：http://ob.huixiangedu.cn

C#:   public static void F() {}
来源：http://zw.szsharing.cn

[G09] 接口 / 抽象类
来源：http://dw.yuntaijiaju.cn

Py:   from abc import ABC, abstractmethod
来源：http://en.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ds.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mm.wgjwhj.cn

TS:   interface Shape { area(): number; }
来源：http://es.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://bw.9csxet.cn

Go:   type Shape interface { Area() float64 }
来源：http://qi.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bj.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://io.bjjhwx.cn

[G10] 访问控制
来源：http://wo.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://ca.yuexingan06.cn

PHP:  public / protected / private
来源：http://dp.bjjhwx.cn

JS:   #private 字段；其余公开
来源：http://ni.szxytkj.cn

TS:   public / protected / private
来源：http://ex.panjiajie.cn

Java: public / protected / private / 默认包级
来源：http://ps.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ol.yuexingan06.cn

Ruby: public / protected / private
来源：http://ui.9csxet.cn

C#:   public / protected / private / internal
来源：http://ru.huixinmuqiang.cn

[G11] getter / setter
来源：http://ff.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://fn.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://tb.hahajie.cn

JS:   get name() { return this._name; }
来源：http://mv.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://cm.yuexingan06.cn

Java: public String getName() { return name; }
来源：http://ut.yuntaijiaju.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mz.nicolike.cn

Ruby: attr_accessor :name
来源：http://yv.huanxung.cn

C#:   public string Name { get; set; }
来源：http://zh.muxihuayi.cn

[G12] 对象转字符串
来源：http://rp.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://xs.shtwfgs.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zv.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://di.haigaiapp.cn

TS:   toString(): string { return this.name; }
来源：http://fr.521024.cn

Java: @Override public String toString() { return name; }
来源：http://ur.muxihuayi.cn


<!-- 参考信息 -->