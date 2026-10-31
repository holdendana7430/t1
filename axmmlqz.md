代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://xi.chemitech.net.cn

[E15] HTML 转义 / 反转义
来源：http://nd.szxytkj.cn

Py:   html.escape(s);  html.unescape(s)
来源：http://di.haigaiapp.cn

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mv.bjjhwx.cn

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://xs.asd995.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://mq.bjjhwx.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://xk.asd995.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://lw.521024.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ek.nszjky.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://kx.jctech888.com.cn

[E16] 数字千分位
来源：http://ch.huanxung.cn

Py:   f"{1234567:,}"
来源：http://bi.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://cw.yuexingan06.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ls.9csxet.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://tg.huixinmuqiang.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ea.colortex.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ni.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://fb.shxzskj.cn

C#:   1234567.ToString("N0")
来源：http://nr.bookmarksfly.cn

[E17] 首字母大写
来源：http://yg.hahajie.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://uq.szsharing.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://oh.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://sz.huixinmuqiang.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zf.bjjhwx.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://jj.szxytkj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://zn.gzmigu.cn

Ruby: s.capitalize
来源：http://tz.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wq.shxzskj.cn

[E18] 模板占位符替换
来源：http://ug.lnxyls.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hr.chemitech.net.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ak.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://kq.haigaiapp.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://nj.hahajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://gb.521024.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wg.szsharing.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://eg.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pj.chemitech.net.cn

[E19] 多行文本按行拆分
来源：http://yp.muxihuayi.cn

Py:   s.splitlines()
来源：http://wc.bjjhwx.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://lb.jianghongdianzi.cn

JS:   s.split(/\r?\n/)
来源：http://lq.huixinmuqiang.cn

TS:   s.split(/\r?\n/)
来源：http://yg.shxzukj.cn

Java: s.lines().toList()
来源：http://ew.lnxyls.cn

Go:   strings.Split(s, "\n")
来源：http://ke.shxzukj.cn

Ruby: s.lines
来源：http://ck.hnjuh.cn

C#:   s.Split('\n')
来源：http://mu.bookmarksfly.cn

[E20] 判断字符串是否为空
来源：http://uk.shtwfgs.cn

Py:   if not s:
来源：http://id.huanxung.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ir.bjjhwx.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://vu.jianghongdianzi.cn

TS:   if (s === "") {}
来源：http://bi.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://qd.lnxyls.cn

Go:   if s == "" {}
来源：http://eo.szsharing.cn

Ruby: if s.empty?
来源：http://bk.9csxet.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://gz.lnxyls.cn

[E21] 超长截断加省略号
来源：http://bp.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://iv.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sl.szxytkj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://kr.lnxyls.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fd.colortex.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://qi.huanxung.cn

Go:   // 按 rune 判断长度后截断
来源：http://xx.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wu.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cy.bjjhwx.cn

[E22] 字节长度与字符长度
来源：http://vd.lnxyls.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://bj.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ed.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rp.nicolike.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://lf.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dk.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ka.gzmigu.cn

Ruby: s.bytesize;  s.length
来源：http://vk.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ff.szsharing.cn

================================================================================
来源：http://hk.yuntaijiaju.cn

F. 文件与目录
来源：http://vh.muxihuayi.cn

================================================================================
来源：http://mr.hahajie.cn

[F01] 读取整个文件
来源：http://ab.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://vw.newstarts.cn

PHP:  file_get_contents("a.txt");
来源：http://lu.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pm.9csxet.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://dk.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://tp.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://io.szxytkj.cn

Ruby: File.read("a.txt")
来源：http://cc.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://aq.shxzskj.cn

[F02] 逐行读取文件
来源：http://qb.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zd.9csxet.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jn.lnxyls.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://et.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pt.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://gz.nicolike.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://fe.szsharing.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pb.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://qb.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://ck.newstarts.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wc.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://rc.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yp.wgjwhj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qb.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ji.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://bm.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://yw.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://nm.hnjuh.cn

[F04] 追加写入文件
来源：http://if.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://np.hnjuh.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ch.huanxung.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tt.nszjky.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://md.wgjwhj.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mr.yuntaijiaju.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gg.newstarts.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://pi.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://iz.9csxet.cn

[F05] 判断文件或目录是否存在
来源：http://ry.yuntaijiaju.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://nb.yuexingan06.cn

PHP:  file_exists("a.txt");
来源：http://zs.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://zm.jctech888.com.cn

TS:   fs.existsSync("a.txt")
来源：http://jb.nszjky.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ag.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://on.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://gj.gzmigu.cn

C#:   File.Exists("a.txt")
来源：http://bh.huanxung.cn

[F06] 删除文件
来源：http://ij.jctech888.com.cn

Py:   os.remove("a.txt")
来源：http://ja.haigaiapp.cn

PHP:  unlink("a.txt");
来源：http://ti.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tl.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://qn.huixiangedu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mn.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://jg.521024.cn

Ruby: File.delete("a.txt")
来源：http://nj.asd995.cn

C#:   File.Delete("a.txt");
来源：http://mn.szxytkj.cn

[F07] 创建目录（含多级）
来源：http://dn.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://oq.bookmarksfly.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pn.shxzukj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kc.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vx.panjiajie.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://vc.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://of.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://gm.shxzukj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wy.haigaiapp.cn

[F08] 遍历目录
来源：http://tt.panjiajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fe.shxzskj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://to.shxzukj.cn

JS:   fs.readdirSync("dir")
来源：http://mx.nszjky.cn

TS:   fs.readdirSync("dir")
来源：http://oh.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ae.bookmarksfly.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wc.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://uu.jctech888.com.cn

C#:   Directory.GetFiles("dir")
来源：http://jc.wgjwhj.cn

[F09] 获取文件大小
来源：http://hj.muxihuayi.cn

Py:   os.path.getsize("a.txt")
来源：http://qn.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://ox.yuntaijiaju.cn

JS:   fs.statSync("a.txt").size
来源：http://fm.chemitech.net.cn

TS:   fs.statSync("a.txt").size
来源：http://fx.huanxung.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gg.chemitech.net.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vv.nicolike.cn

Ruby: File.size("a.txt")
来源：http://ta.bookmarksfly.cn

C#:   new FileInfo("a.txt").Length
来源：http://tz.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://kw.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://is.jctech888.com.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://yp.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://zl.shxzskj.cn

TS:   path.extname("a.txt")
来源：http://xo.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://iy.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ng.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mz.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vq.colortex.cn

[F11] 复制与移动文件
来源：http://xj.chemitech.net.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nz.szxytkj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://rn.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zs.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bw.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://fg.wgjwhj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://lj.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://lz.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ql.panjiajie.cn

[F12] CSV 读写
来源：http://ih.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lz.bookmarksfly.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mc.szsharing.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wp.jctech888.com.cn

TS:   // 同上
来源：http://bu.yuntaijiaju.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ca.chemitech.net.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://iu.hahajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hj.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://vm.nszjky.cn

================================================================================
来源：http://hu.lnxyls.cn

G. 面向对象
来源：http://nb.haigaiapp.cn

================================================================================
来源：http://no.nszjky.cn

[G01] 定义类
来源：http://fr.haigaiapp.cn

Py:   class User: pass
来源：http://nm.gzmigu.cn

PHP:  class User {}
来源：http://ez.szxytkj.cn

JS:   class User {}
来源：http://qe.521024.cn

TS:   class User { name: string = ""; }
来源：http://ip.jctech888.com.cn

Java: class User {}
来源：http://zb.yuexingan06.cn

Go:   type User struct { Name string }
来源：http://iv.chemitech.net.cn

Ruby: class User; end
来源：http://wr.muxihuayi.cn

C#:   class User {}
来源：http://my.521024.cn

[G02] 构造函数
来源：http://oz.muxihuayi.cn

Py:   def __init__(self, name): self.name = name
来源：http://tt.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://hh.huanxung.cn

JS:   constructor(name) { this.name = name; }
来源：http://xc.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://tv.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://rv.shxzskj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tq.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://xt.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://xg.shxzukj.cn

[G03] 实例属性
来源：http://zt.jctech888.com.cn

Py:   self.name = "x"
来源：http://qk.9csxet.cn

PHP:  public string $name = "x";
来源：http://zz.521024.cn

JS:   this.name = "x";
来源：http://mn.nicolike.cn

TS:   name: string = "x";
来源：http://ko.panjiajie.cn

Java: private String name;
来源：http://kx.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fh.hnjuh.cn

Ruby: @name = "x"
来源：http://mv.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://cl.521024.cn

[G04] 定义方法
来源：http://ph.hnjuh.cn

Py:   def greet(self): return self.name
来源：http://mh.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wa.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://lr.szsharing.cn

TS:   greet(): string { return this.name; }
来源：http://ao.521024.cn

Java: String greet() { return name; }
来源：http://gd.muxihuayi.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nu.nicolike.cn

Ruby: def greet; @name; end
来源：http://vy.szsharing.cn

C#:   public string Greet() => Name;
来源：http://sm.huanxung.cn

[G05] 继承
来源：http://dg.gzmigu.cn

Py:   class Admin(User): pass
来源：http://qt.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://cl.huanxung.cn

JS:   class Admin extends User {}
来源：http://jv.bjjhwx.cn

TS:   class Admin extends User {}
来源：http://ra.panjiajie.cn

Java: class Admin extends User {}
来源：http://br.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ne.9csxet.cn

Ruby: class Admin < User; end
来源：http://np.lnxyls.cn

C#:   class Admin : User {}
来源：http://uc.jianghongdianzi.cn

[G06] 重写方法
来源：http://pr.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://bz.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://im.haigaiapp.cn

JS:   greet() { return "admin"; }
来源：http://ct.521024.cn

TS:   greet(): string { return "admin"; }
来源：http://aw.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://pp.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yd.nszjky.cn

Ruby: def greet; "admin"; end
来源：http://es.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://ai.huanxung.cn

[G07] 调用父类方法
来源：http://dm.shtwfgs.cn

Py:   super().greet()
来源：http://rs.521024.cn

PHP:  parent::greet();
来源：http://xx.gzmigu.cn

JS:   super.greet();
来源：http://bf.bjjhwx.cn

TS:   super.greet();
来源：http://ej.huixinmuqiang.cn

Java: super.greet();
来源：http://jc.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ep.wgjwhj.cn

Ruby: super
来源：http://tu.newstarts.cn

C#:   base.Greet();
来源：http://ia.shxzukj.cn

[G08] 静态方法与属性
来源：http://bg.szxytkj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hd.panjiajie.cn

PHP:  public static function f() {}
来源：http://wn.521024.cn

JS:   static f() {}
来源：http://uc.shtwfgs.cn

TS:   static f(): void {}
来源：http://xj.9csxet.cn

Java: static void f() {}
来源：http://du.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://yl.huixiangedu.cn

Ruby: def self.f; end
来源：http://za.huanxung.cn

C#:   public static void F() {}
来源：http://vz.nicolike.cn

[G09] 接口 / 抽象类
来源：http://wx.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://rg.yuexingan06.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ap.huixinmuqiang.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ob.9csxet.cn

TS:   interface Shape { area(): number; }
来源：http://he.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://fi.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://ob.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://cn.521024.cn

C#:   interface IShape { double Area(); }
来源：http://be.yuexingan06.cn

[G10] 访问控制
来源：http://fr.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://ex.yuexingan06.cn

PHP:  public / protected / private
来源：http://eb.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://an.lnxyls.cn

TS:   public / protected / private
来源：http://lq.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://ul.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://xj.9csxet.cn

Ruby: public / protected / private
来源：http://mt.wgjwhj.cn

C#:   public / protected / private / internal
来源：http://hk.jctech888.com.cn

[G11] getter / setter
来源：http://kd.panjiajie.cn

Py:   @property 与 @x.setter
来源：http://wd.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://um.colortex.cn

JS:   get name() { return this._name; }
来源：http://qb.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://vo.jctech888.com.cn

Java: public String getName() { return name; }
来源：http://al.huanxung.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://an.newstarts.cn

Ruby: attr_accessor :name
来源：http://be.colortex.cn

C#:   public string Name { get; set; }
来源：http://yb.jctech888.com.cn

[G12] 对象转字符串
来源：http://sf.huixinmuqiang.cn

Py:   def __str__(self): return self.name
来源：http://vc.bookmarksfly.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ub.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://pq.shtwfgs.cn

TS:   toString(): string { return this.name; }
来源：http://vg.shtwfgs.cn

Java: @Override public String toString() { return name; }
来源：http://zf.szsharing.cn

Go:   func (u User) String() string { return u.Name }
来源：http://db.asd995.cn

Ruby: def to_s; @name; end
来源：http://jj.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://zr.asd995.cn

[G13] 判断对象类型
来源：http://ym.9csxet.cn

Py:   isinstance(u, User)
来源：http://sl.panjiajie.cn

PHP:  $u instanceof User
来源：http://mj.wgjwhj.cn

JS:   u instanceof User
来源：http://vg.panjiajie.cn

TS:   u instanceof User
来源：http://ak.colortex.cn


<!-- 参考信息 -->