代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://ia.bjjhwx.cn

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://ll.huanxung.cn

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://yf.szxytkj.cn

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://qm.muxihuayi.cn

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://cl.9csxet.cn

[E15] HTML 转义 / 反转义
来源：http://vn.haigaiapp.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://oo.colortex.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://ur.shtwfgs.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sa.yuexingan06.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://gk.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://iw.wgjwhj.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://os.huanxung.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://sx.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://yo.9csxet.cn

[E16] 数字千分位
来源：http://jz.newstarts.cn

Py:   f"{1234567:,}"
来源：http://rt.shxzukj.cn

PHP:  number_format(1234567);
来源：http://vb.hahajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qz.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qc.wgjwhj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mb.chemitech.net.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://fq.9csxet.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://he.asd995.cn

C#:   1234567.ToString("N0")
来源：http://ro.muxihuayi.cn

[E17] 首字母大写
来源：http://sk.colortex.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://rn.newstarts.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://uk.lnxyls.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://vn.nszjky.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ov.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://iv.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ca.szsharing.cn

Ruby: s.capitalize
来源：http://xq.jctech888.com.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://aq.9csxet.cn

[E18] 模板占位符替换
来源：http://ws.huixinmuqiang.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://jl.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bo.asd995.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ob.jctech888.com.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://mx.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://dm.colortex.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yg.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://af.gzmigu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://kt.shxzskj.cn

[E19] 多行文本按行拆分
来源：http://oy.shtwfgs.cn

Py:   s.splitlines()
来源：http://io.shxzskj.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xw.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://ma.haigaiapp.cn

TS:   s.split(/\r?\n/)
来源：http://kw.bookmarksfly.cn

Java: s.lines().toList()
来源：http://ng.9csxet.cn

Go:   strings.Split(s, "\n")
来源：http://uy.hnjuh.cn

Ruby: s.lines
来源：http://xu.jianghongdianzi.cn

C#:   s.Split('\n')
来源：http://mc.haigaiapp.cn

[E20] 判断字符串是否为空
来源：http://ir.hnjuh.cn

Py:   if not s:
来源：http://jm.chemitech.net.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://io.shtwfgs.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qp.hahajie.cn

TS:   if (s === "") {}
来源：http://sd.hahajie.cn

Java: if (s.isEmpty()) {}
来源：http://ja.shxzskj.cn

Go:   if s == "" {}
来源：http://wx.shtwfgs.cn

Ruby: if s.empty?
来源：http://zj.huanxung.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gr.yuexingan06.cn

[E21] 超长截断加省略号
来源：http://qv.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://pg.chemitech.net.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://gx.shxzukj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://lf.newstarts.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://he.panjiajie.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mx.nicolike.cn

Go:   // 按 rune 判断长度后截断
来源：http://ib.shxzskj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://tx.panjiajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://uf.szxytkj.cn

[E22] 字节长度与字符长度
来源：http://cr.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://lv.yuexingan06.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sm.panjiajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://fb.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://es.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hr.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pe.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://xx.huixinmuqiang.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ed.jctech888.com.cn

================================================================================
来源：http://ft.wgjwhj.cn

F. 文件与目录
来源：http://be.muxihuayi.cn

================================================================================
来源：http://ph.newstarts.cn

[F01] 读取整个文件
来源：http://zz.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://em.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://uw.szxytkj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nt.hahajie.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qe.huixinmuqiang.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://as.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://oa.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://nq.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://jk.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://jk.hahajie.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mm.jianghongdianzi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wx.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gq.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://he.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ya.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lb.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://st.newstarts.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tu.muxihuayi.cn

[F03] 写入文件（覆盖）
来源：http://ou.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pe.hnjuh.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://se.9csxet.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jt.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ck.panjiajie.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://jv.shtwfgs.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://js.shxzukj.cn

Ruby: File.write("a.txt", "hi")
来源：http://ul.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://yi.huixiangedu.cn

[F04] 追加写入文件
来源：http://lz.lnxyls.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://gj.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zg.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qa.bookmarksfly.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rw.lnxyls.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ox.bookmarksfly.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ke.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ql.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ns.shxzukj.cn

[F05] 判断文件或目录是否存在
来源：http://jd.asd995.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://vu.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://zf.yuntaijiaju.cn

JS:   fs.existsSync("a.txt")
来源：http://cd.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://gl.shtwfgs.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://km.shxzukj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://af.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://iz.jianghongdianzi.cn

C#:   File.Exists("a.txt")
来源：http://wt.9csxet.cn

[F06] 删除文件
来源：http://wk.jianghongdianzi.cn

Py:   os.remove("a.txt")
来源：http://ez.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://jm.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://gc.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zl.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://bs.muxihuayi.cn

Go:   os.Remove("a.txt")
来源：http://mp.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://kl.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://dv.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://hy.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ke.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hf.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ef.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yg.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://uf.shtwfgs.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ir.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dl.lnxyls.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vl.szsharing.cn

[F08] 遍历目录
来源：http://un.huanxung.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ax.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ls.yuntaijiaju.cn

JS:   fs.readdirSync("dir")
来源：http://qm.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://mw.9csxet.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://it.huanxung.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ab.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://kv.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://te.asd995.cn

[F09] 获取文件大小
来源：http://vq.lnxyls.cn

Py:   os.path.getsize("a.txt")
来源：http://kd.asd995.cn

PHP:  filesize("a.txt");
来源：http://pk.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://rp.shxzukj.cn

TS:   fs.statSync("a.txt").size
来源：http://gd.yuntaijiaju.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sn.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://uk.bookmarksfly.cn

Ruby: File.size("a.txt")
来源：http://ex.huixiangedu.cn

C#:   new FileInfo("a.txt").Length
来源：http://qj.szsharing.cn

[F10] 取文件扩展名 / 文件名
来源：http://qz.panjiajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mo.yuexingan06.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ty.shxzskj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://jg.szsharing.cn

TS:   path.extname("a.txt")
来源：http://vj.shxzskj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://oe.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ok.haigaiapp.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ne.shxzukj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://rz.9csxet.cn

[F11] 复制与移动文件
来源：http://up.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ol.lnxyls.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ve.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xf.gzmigu.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rd.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ta.bjjhwx.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ic.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://av.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ek.haigaiapp.cn

[F12] CSV 读写
来源：http://mx.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://ux.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://gu.yuntaijiaju.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wg.newstarts.cn

TS:   // 同上
来源：http://yn.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://cy.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://qd.wgjwhj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tu.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ef.colortex.cn

================================================================================
来源：http://da.chemitech.net.cn

G. 面向对象
来源：http://ex.lnxyls.cn

================================================================================
来源：http://oy.nicolike.cn

[G01] 定义类
来源：http://gq.9csxet.cn

Py:   class User: pass
来源：http://tc.newstarts.cn

PHP:  class User {}
来源：http://zi.muxihuayi.cn

JS:   class User {}
来源：http://jg.asd995.cn

TS:   class User { name: string = ""; }
来源：http://gu.panjiajie.cn

Java: class User {}
来源：http://nm.hnjuh.cn

Go:   type User struct { Name string }
来源：http://kp.jianghongdianzi.cn

Ruby: class User; end
来源：http://hh.chemitech.net.cn

C#:   class User {}
来源：http://of.shxzskj.cn

[G02] 构造函数
来源：http://py.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://ja.jctech888.com.cn

PHP:  public function __construct(public string $name) {}
来源：http://wi.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://ti.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://rn.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://pe.lnxyls.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pp.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://xv.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://qn.shxzukj.cn

[G03] 实例属性
来源：http://vo.haigaiapp.cn

Py:   self.name = "x"
来源：http://ck.asd995.cn

PHP:  public string $name = "x";
来源：http://cr.hahajie.cn

JS:   this.name = "x";
来源：http://cu.szxytkj.cn

TS:   name: string = "x";
来源：http://io.huixiangedu.cn

Java: private String name;
来源：http://ts.szxytkj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hr.huixiangedu.cn

Ruby: @name = "x"
来源：http://it.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://te.shxzskj.cn

[G04] 定义方法
来源：http://xo.colortex.cn

Py:   def greet(self): return self.name
来源：http://sc.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ba.szxytkj.cn

JS:   greet() { return this.name; }
来源：http://vn.nicolike.cn

TS:   greet(): string { return this.name; }
来源：http://mb.szsharing.cn

Java: String greet() { return name; }
来源：http://ku.colortex.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ww.shxzskj.cn

Ruby: def greet; @name; end
来源：http://nn.huanxung.cn

C#:   public string Greet() => Name;
来源：http://tl.jianghongdianzi.cn

[G05] 继承
来源：http://tp.521024.cn

Py:   class Admin(User): pass
来源：http://vf.nszjky.cn

PHP:  class Admin extends User {}
来源：http://jz.shtwfgs.cn

JS:   class Admin extends User {}
来源：http://qi.9csxet.cn

TS:   class Admin extends User {}
来源：http://sa.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://fn.szsharing.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hb.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://yp.panjiajie.cn

C#:   class Admin : User {}
来源：http://at.bookmarksfly.cn

[G06] 重写方法
来源：http://jr.chemitech.net.cn

Py:   def greet(self): return "admin"
来源：http://me.shxzukj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://kk.yuexingan06.cn

JS:   greet() { return "admin"; }
来源：http://xh.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://jk.szxytkj.cn

Java: @Override String greet() { return "admin"; }
来源：http://oa.colortex.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://pz.lnxyls.cn

Ruby: def greet; "admin"; end
来源：http://jl.lnxyls.cn

C#:   public override string Greet() => "admin";
来源：http://wq.huixiangedu.cn

[G07] 调用父类方法
来源：http://oz.colortex.cn

Py:   super().greet()
来源：http://yg.asd995.cn

PHP:  parent::greet();
来源：http://hr.yuntaijiaju.cn

JS:   super.greet();
来源：http://yq.jianghongdianzi.cn

TS:   super.greet();
来源：http://yb.9csxet.cn

Java: super.greet();
来源：http://hp.gzmigu.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://kz.shxzukj.cn

Ruby: super
来源：http://en.wgjwhj.cn

C#:   base.Greet();
来源：http://rk.shtwfgs.cn

[G08] 静态方法与属性
来源：http://aa.wgjwhj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://uo.shxzukj.cn

PHP:  public static function f() {}
来源：http://ua.colortex.cn

JS:   static f() {}
来源：http://yg.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://xz.shxzskj.cn

Java: static void f() {}
来源：http://fz.colortex.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ax.panjiajie.cn

Ruby: def self.f; end
来源：http://nw.bjjhwx.cn

C#:   public static void F() {}
来源：http://wt.szsharing.cn

[G09] 接口 / 抽象类
来源：http://qw.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://hs.nicolike.cn

PHP:  interface Shape { public function area(): float; }
来源：http://al.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://mm.yuexingan06.cn

TS:   interface Shape { area(): number; }
来源：http://ss.colortex.cn

Java: interface Shape { double area(); }
来源：http://wc.haigaiapp.cn

Go:   type Shape interface { Area() float64 }
来源：http://kb.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ib.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://te.muxihuayi.cn

[G10] 访问控制
来源：http://td.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://pq.gzmigu.cn

PHP:  public / protected / private
来源：http://fy.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://bi.panjiajie.cn

TS:   public / protected / private
来源：http://zi.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://sl.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://kd.nszjky.cn

Ruby: public / protected / private
来源：http://op.lnxyls.cn

C#:   public / protected / private / internal
来源：http://gl.asd995.cn

[G11] getter / setter
来源：http://zt.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://hc.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://lr.jctech888.com.cn

JS:   get name() { return this._name; }
来源：http://gj.jctech888.com.cn

TS:   get name(): string { return this._name; }
来源：http://cj.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://el.lnxyls.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ik.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://hr.bjjhwx.cn

C#:   public string Name { get; set; }
来源：http://an.nszjky.cn

[G12] 对象转字符串
来源：http://kb.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://mv.shxzukj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://fj.521024.cn

JS:   toString() { return this.name; }
来源：http://uy.huanxung.cn

TS:   toString(): string { return this.name; }
来源：http://qj.szxytkj.cn

Java: @Override public String toString() { return name; }
来源：http://pp.jianghongdianzi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://qv.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://jn.hnjuh.cn

C#:   public override string ToString() => Name;
来源：http://hz.haigaiapp.cn

[G13] 判断对象类型
来源：http://zm.huixiangedu.cn


<!-- 参考信息 -->