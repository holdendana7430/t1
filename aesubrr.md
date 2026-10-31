代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://jz.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ka.asd995.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mv.huanxung.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://rg.haigaiapp.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ak.chemitech.net.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ba.szxytkj.cn

[E16] 数字千分位
来源：http://jw.9csxet.cn

Py:   f"{1234567:,}"
来源：http://tb.jctech888.com.cn

PHP:  number_format(1234567);
来源：http://dc.shxzukj.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://th.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://xz.szxytkj.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ej.yuntaijiaju.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ck.hahajie.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wl.shtwfgs.cn

C#:   1234567.ToString("N0")
来源：http://mc.jctech888.com.cn

[E17] 首字母大写
来源：http://es.newstarts.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ew.haigaiapp.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://xm.jianghongdianzi.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://kq.panjiajie.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://is.muxihuayi.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://sc.shtwfgs.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ly.hnjuh.cn

Ruby: s.capitalize
来源：http://bp.panjiajie.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://lt.nicolike.cn

[E18] 模板占位符替换
来源：http://rt.bookmarksfly.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://oe.bjjhwx.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://ut.9csxet.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://qm.colortex.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://ef.szsharing.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://ru.muxihuayi.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://on.hahajie.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://bx.shxzskj.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://yn.shxzukj.cn

[E19] 多行文本按行拆分
来源：http://xl.chemitech.net.cn

Py:   s.splitlines()
来源：http://hu.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://yb.nszjky.cn

JS:   s.split(/\r?\n/)
来源：http://ak.szsharing.cn

TS:   s.split(/\r?\n/)
来源：http://xg.haigaiapp.cn

Java: s.lines().toList()
来源：http://la.chemitech.net.cn

Go:   strings.Split(s, "\n")
来源：http://ru.nszjky.cn

Ruby: s.lines
来源：http://xb.huanxung.cn

C#:   s.Split('\n')
来源：http://fg.shxzukj.cn

[E20] 判断字符串是否为空
来源：http://sv.szxytkj.cn

Py:   if not s:
来源：http://ya.newstarts.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mh.nicolike.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hx.shtwfgs.cn

TS:   if (s === "") {}
来源：http://fo.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://ie.nicolike.cn

Go:   if s == "" {}
来源：http://sx.shxzskj.cn

Ruby: if s.empty?
来源：http://vu.muxihuayi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qo.newstarts.cn

[E21] 超长截断加省略号
来源：http://ke.jianghongdianzi.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ar.jctech888.com.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://kk.9csxet.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gz.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dz.muxihuayi.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://ym.huixinmuqiang.cn

Go:   // 按 rune 判断长度后截断
来源：http://us.bookmarksfly.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ww.hahajie.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://zp.jctech888.com.cn

[E22] 字节长度与字符长度
来源：http://si.wgjwhj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hh.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://tx.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hb.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://sx.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zt.chemitech.net.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yv.huixinmuqiang.cn

Ruby: s.bytesize;  s.length
来源：http://jr.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://fd.nszjky.cn

================================================================================
来源：http://ss.muxihuayi.cn

F. 文件与目录
来源：http://tk.lnxyls.cn

================================================================================
来源：http://dx.muxihuayi.cn

[F01] 读取整个文件
来源：http://lc.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ap.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://pr.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ar.colortex.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lh.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://vp.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://fs.jianghongdianzi.cn

Ruby: File.read("a.txt")
来源：http://yg.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://uo.muxihuayi.cn

[F02] 逐行读取文件
来源：http://jl.9csxet.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mc.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://vr.hnjuh.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lx.shxzskj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fg.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ys.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ha.bjjhwx.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ur.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://eb.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://xe.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://st.521024.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://fy.shxzukj.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://zx.haigaiapp.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qc.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lr.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://te.bookmarksfly.cn

Ruby: File.write("a.txt", "hi")
来源：http://aw.huixiangedu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ul.bookmarksfly.cn

[F04] 追加写入文件
来源：http://as.jianghongdianzi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wc.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pp.shtwfgs.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://rc.521024.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tq.hnjuh.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ow.asd995.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://qq.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://ju.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://la.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://rb.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ln.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://mh.huixiangedu.cn

JS:   fs.existsSync("a.txt")
来源：http://tg.huanxung.cn

TS:   fs.existsSync("a.txt")
来源：http://sk.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://fo.jctech888.com.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mz.shxzskj.cn

Ruby: File.exist?("a.txt")
来源：http://xz.szsharing.cn

C#:   File.Exists("a.txt")
来源：http://by.bjjhwx.cn

[F06] 删除文件
来源：http://tk.yuntaijiaju.cn

Py:   os.remove("a.txt")
来源：http://fq.jianghongdianzi.cn

PHP:  unlink("a.txt");
来源：http://ip.chemitech.net.cn

JS:   fs.unlinkSync("a.txt")
来源：http://px.huixiangedu.cn

TS:   fs.unlinkSync("a.txt")
来源：http://of.wgjwhj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wf.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://uy.bookmarksfly.cn

Ruby: File.delete("a.txt")
来源：http://jb.shtwfgs.cn

C#:   File.Delete("a.txt");
来源：http://ci.panjiajie.cn

[F07] 创建目录（含多级）
来源：http://qx.colortex.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://cb.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://iv.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://as.newstarts.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ai.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wc.jianghongdianzi.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dr.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hp.bjjhwx.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://nz.asd995.cn

[F08] 遍历目录
来源：http://qv.shxzukj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ap.huanxung.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lo.nicolike.cn

JS:   fs.readdirSync("dir")
来源：http://fo.muxihuayi.cn

TS:   fs.readdirSync("dir")
来源：http://yt.shtwfgs.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hj.panjiajie.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qy.asd995.cn

Ruby: Dir.children("dir")
来源：http://az.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://bo.yuexingan06.cn

[F09] 获取文件大小
来源：http://za.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://gd.muxihuayi.cn

PHP:  filesize("a.txt");
来源：http://pt.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://nh.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://je.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bb.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://tq.nszjky.cn

Ruby: File.size("a.txt")
来源：http://ee.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://qj.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://yf.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://te.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bk.wgjwhj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gl.szsharing.cn

TS:   path.extname("a.txt")
来源：http://yo.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xz.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://yd.yuexingan06.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://rj.newstarts.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xl.colortex.cn

[F11] 复制与移动文件
来源：http://rw.9csxet.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hx.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://bk.haigaiapp.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://xy.9csxet.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gd.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lv.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://qb.asd995.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wf.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://nl.szxytkj.cn

[F12] CSV 读写
来源：http://tg.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qb.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://en.szxytkj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bw.huanxung.cn

TS:   // 同上
来源：http://go.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://gj.colortex.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://om.nicolike.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://tx.szsharing.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ze.bookmarksfly.cn

================================================================================
来源：http://tj.hnjuh.cn

G. 面向对象
来源：http://jf.521024.cn

================================================================================
来源：http://fz.jctech888.com.cn

[G01] 定义类
来源：http://qd.chemitech.net.cn

Py:   class User: pass
来源：http://ew.colortex.cn

PHP:  class User {}
来源：http://wl.yuexingan06.cn

JS:   class User {}
来源：http://sb.asd995.cn

TS:   class User { name: string = ""; }
来源：http://ly.hnjuh.cn

Java: class User {}
来源：http://mt.muxihuayi.cn

Go:   type User struct { Name string }
来源：http://ci.gzmigu.cn

Ruby: class User; end
来源：http://te.hahajie.cn

C#:   class User {}
来源：http://ln.nszjky.cn

[G02] 构造函数
来源：http://mj.chemitech.net.cn

Py:   def __init__(self, name): self.name = name
来源：http://eo.jianghongdianzi.cn

PHP:  public function __construct(public string $name) {}
来源：http://mi.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://ox.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://bi.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://xb.shxzukj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://cq.jianghongdianzi.cn

Ruby: def initialize(name); @name = name; end
来源：http://ss.muxihuayi.cn

C#:   public User(string name) { Name = name; }
来源：http://co.szsharing.cn

[G03] 实例属性
来源：http://ny.chemitech.net.cn

Py:   self.name = "x"
来源：http://qg.chemitech.net.cn

PHP:  public string $name = "x";
来源：http://zo.colortex.cn

JS:   this.name = "x";
来源：http://hl.bookmarksfly.cn

TS:   name: string = "x";
来源：http://mu.gzmigu.cn

Java: private String name;
来源：http://cz.szsharing.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nh.9csxet.cn

Ruby: @name = "x"
来源：http://tt.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://oi.hahajie.cn

[G04] 定义方法
来源：http://yj.521024.cn

Py:   def greet(self): return self.name
来源：http://xk.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://hq.lnxyls.cn

JS:   greet() { return this.name; }
来源：http://ng.yuexingan06.cn

TS:   greet(): string { return this.name; }
来源：http://yu.nszjky.cn

Java: String greet() { return name; }
来源：http://zs.shtwfgs.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://xf.panjiajie.cn

Ruby: def greet; @name; end
来源：http://wm.huanxung.cn

C#:   public string Greet() => Name;
来源：http://lt.yuexingan06.cn

[G05] 继承
来源：http://na.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://ma.bjjhwx.cn

PHP:  class Admin extends User {}
来源：http://us.colortex.cn

JS:   class Admin extends User {}
来源：http://nc.szxytkj.cn

TS:   class Admin extends User {}
来源：http://bk.nszjky.cn

Java: class Admin extends User {}
来源：http://ut.yuntaijiaju.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ed.muxihuayi.cn

Ruby: class Admin < User; end
来源：http://we.gzmigu.cn

C#:   class Admin : User {}
来源：http://cz.panjiajie.cn

[G06] 重写方法
来源：http://lk.muxihuayi.cn

Py:   def greet(self): return "admin"
来源：http://es.wgjwhj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://og.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://mu.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://jk.panjiajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://lf.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.yuntaijiaju.cn

Ruby: def greet; "admin"; end
来源：http://yl.yuexingan06.cn

C#:   public override string Greet() => "admin";
来源：http://ql.huixinmuqiang.cn

[G07] 调用父类方法
来源：http://di.jianghongdianzi.cn

Py:   super().greet()
来源：http://yr.bookmarksfly.cn

PHP:  parent::greet();
来源：http://ik.yuexingan06.cn

JS:   super.greet();
来源：http://ee.nicolike.cn

TS:   super.greet();
来源：http://cb.szxytkj.cn

Java: super.greet();
来源：http://ie.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://dy.yuexingan06.cn

Ruby: super
来源：http://zd.nicolike.cn

C#:   base.Greet();
来源：http://ew.chemitech.net.cn

[G08] 静态方法与属性
来源：http://cf.hahajie.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://cb.shxzukj.cn

PHP:  public static function f() {}
来源：http://sc.nszjky.cn

JS:   static f() {}
来源：http://um.szsharing.cn

TS:   static f(): void {}
来源：http://jy.huixinmuqiang.cn

Java: static void f() {}
来源：http://lf.lnxyls.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fb.521024.cn

Ruby: def self.f; end
来源：http://jp.lnxyls.cn

C#:   public static void F() {}
来源：http://fc.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://es.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://im.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://kv.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bl.huixinmuqiang.cn

TS:   interface Shape { area(): number; }
来源：http://sk.lnxyls.cn

Java: interface Shape { double area(); }
来源：http://na.huixinmuqiang.cn

Go:   type Shape interface { Area() float64 }
来源：http://uc.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yp.huanxung.cn

C#:   interface IShape { double Area(); }
来源：http://dk.wgjwhj.cn

[G10] 访问控制
来源：http://gz.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://ci.jctech888.com.cn

PHP:  public / protected / private
来源：http://ds.panjiajie.cn

JS:   #private 字段；其余公开
来源：http://rf.szxytkj.cn

TS:   public / protected / private
来源：http://gl.chemitech.net.cn

Java: public / protected / private / 默认包级
来源：http://xt.huixinmuqiang.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://nt.shxzskj.cn

Ruby: public / protected / private
来源：http://xe.muxihuayi.cn

C#:   public / protected / private / internal
来源：http://lx.yuexingan06.cn

[G11] getter / setter
来源：http://zr.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://sa.gzmigu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://hk.yuntaijiaju.cn

JS:   get name() { return this._name; }
来源：http://ft.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://hy.gzmigu.cn

Java: public String getName() { return name; }
来源：http://jr.haigaiapp.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wb.jctech888.com.cn

Ruby: attr_accessor :name
来源：http://ff.szsharing.cn

C#:   public string Name { get; set; }
来源：http://pd.szsharing.cn

[G12] 对象转字符串
来源：http://gq.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://yk.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bg.panjiajie.cn

JS:   toString() { return this.name; }
来源：http://dw.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://xf.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://so.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://lt.colortex.cn

Ruby: def to_s; @name; end
来源：http://qx.jctech888.com.cn

C#:   public override string ToString() => Name;
来源：http://cp.shxzskj.cn

[G13] 判断对象类型
来源：http://ud.chemitech.net.cn

Py:   isinstance(u, User)
来源：http://eq.szxytkj.cn

PHP:  $u instanceof User
来源：http://th.9csxet.cn

JS:   u instanceof User
来源：http://rf.shtwfgs.cn

TS:   u instanceof User
来源：http://hg.huixiangedu.cn

Java: u instanceof User
来源：http://gh.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ze.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://jm.hahajie.cn

C#:   u is User
来源：http://mf.huanxung.cn


<!-- 参考信息 -->