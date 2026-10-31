代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://sr.nicolike.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://ao.yuexingan06.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://vj.yuntaijiaju.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://vh.yuntaijiaju.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://xg.bjjhwx.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://zo.gzmigu.cn

[E16] 数字千分位
来源：http://rx.shxzukj.cn

Py:   f"{1234567:,}"
来源：http://jn.shxzskj.cn

PHP:  number_format(1234567);
来源：http://qg.9csxet.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://bu.colortex.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://zn.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://ki.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yo.hnjuh.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://oi.asd995.cn

C#:   1234567.ToString("N0")
来源：http://xt.muxihuayi.cn

[E17] 首字母大写
来源：http://id.huixinmuqiang.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://qx.asd995.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://en.yuntaijiaju.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xe.chemitech.net.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://fz.asd995.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ku.yuntaijiaju.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://gp.lnxyls.cn

Ruby: s.capitalize
来源：http://ye.9csxet.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hh.huixiangedu.cn

[E18] 模板占位符替换
来源：http://ro.szsharing.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://bb.muxihuayi.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://pj.nszjky.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://jd.gzmigu.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://wz.muxihuayi.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://pr.shtwfgs.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zb.newstarts.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wv.asd995.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://nf.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://dc.nicolike.cn

Py:   s.splitlines()
来源：http://wh.yuexingan06.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hq.asd995.cn

JS:   s.split(/\r?\n/)
来源：http://dl.wgjwhj.cn

TS:   s.split(/\r?\n/)
来源：http://zy.hahajie.cn

Java: s.lines().toList()
来源：http://lo.szxytkj.cn

Go:   strings.Split(s, "\n")
来源：http://zz.shxzukj.cn

Ruby: s.lines
来源：http://fy.newstarts.cn

C#:   s.Split('\n')
来源：http://mo.yuexingan06.cn

[E20] 判断字符串是否为空
来源：http://of.jctech888.com.cn

Py:   if not s:
来源：http://id.colortex.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://kc.shxzukj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ap.9csxet.cn

TS:   if (s === "") {}
来源：http://qo.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://yz.nszjky.cn

Go:   if s == "" {}
来源：http://dw.nszjky.cn

Ruby: if s.empty?
来源：http://lw.haigaiapp.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://xl.chemitech.net.cn

[E21] 超长截断加省略号
来源：http://bz.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://qe.bjjhwx.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://jr.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://dx.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gv.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xx.9csxet.cn

Go:   // 按 rune 判断长度后截断
来源：http://fg.nszjky.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://ua.shxzskj.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hk.haigaiapp.cn

[E22] 字节长度与字符长度
来源：http://ht.yuexingan06.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xd.gzmigu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ei.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://pt.huixiangedu.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xi.hahajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ms.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ef.colortex.cn

Ruby: s.bytesize;  s.length
来源：http://ga.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sq.shtwfgs.cn

================================================================================
来源：http://dt.szxytkj.cn

F. 文件与目录
来源：http://hx.hahajie.cn

================================================================================
来源：http://hh.jianghongdianzi.cn

[F01] 读取整个文件
来源：http://ek.wgjwhj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uo.huanxung.cn

PHP:  file_get_contents("a.txt");
来源：http://ek.jctech888.com.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://se.newstarts.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://uv.9csxet.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ns.chemitech.net.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ay.szsharing.cn

Ruby: File.read("a.txt")
来源：http://zu.colortex.cn

C#:   File.ReadAllText("a.txt");
来源：http://zo.shxzukj.cn

[F02] 逐行读取文件
来源：http://nf.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ja.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ra.huixiangedu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sh.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://th.szsharing.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zg.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://pg.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://gp.haigaiapp.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wg.szxytkj.cn

[F03] 写入文件（覆盖）
来源：http://dh.shtwfgs.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://og.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ly.521024.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://be.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vo.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://zy.haigaiapp.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://co.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://mh.szsharing.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mh.shxzskj.cn

[F04] 追加写入文件
来源：http://oj.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ww.hahajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://se.jianghongdianzi.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://iv.szxytkj.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qf.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ul.shxzukj.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://lz.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://we.shxzukj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ds.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://yf.jianghongdianzi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lx.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://ft.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://rb.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://jl.szsharing.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ip.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://me.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://yj.colortex.cn

C#:   File.Exists("a.txt")
来源：http://df.huanxung.cn

[F06] 删除文件
来源：http://cr.panjiajie.cn

Py:   os.remove("a.txt")
来源：http://ji.bjjhwx.cn

PHP:  unlink("a.txt");
来源：http://et.newstarts.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ye.bjjhwx.cn

TS:   fs.unlinkSync("a.txt")
来源：http://io.szsharing.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://dq.chemitech.net.cn

Go:   os.Remove("a.txt")
来源：http://rt.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://fs.colortex.cn

C#:   File.Delete("a.txt");
来源：http://rd.bookmarksfly.cn

[F07] 创建目录（含多级）
来源：http://pj.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fl.yuexingan06.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://oj.hahajie.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yk.huanxung.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zw.shxzskj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rz.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://dx.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ov.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pk.szxytkj.cn

[F08] 遍历目录
来源：http://gw.bookmarksfly.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xf.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://yx.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://dg.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://ix.jianghongdianzi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hw.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://xc.panjiajie.cn

Ruby: Dir.children("dir")
来源：http://zr.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://ok.szxytkj.cn

[F09] 获取文件大小
来源：http://zv.chemitech.net.cn

Py:   os.path.getsize("a.txt")
来源：http://tk.szsharing.cn

PHP:  filesize("a.txt");
来源：http://tg.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://um.521024.cn

TS:   fs.statSync("a.txt").size
来源：http://yh.chemitech.net.cn

Java: Files.size(Path.of("a.txt"))
来源：http://bi.jctech888.com.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://lu.wgjwhj.cn

Ruby: File.size("a.txt")
来源：http://oj.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://nc.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://nq.huanxung.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ot.huixinmuqiang.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://tu.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://lg.521024.cn

TS:   path.extname("a.txt")
来源：http://dw.jianghongdianzi.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sf.hnjuh.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ub.521024.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://nc.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://vi.lnxyls.cn

[F11] 复制与移动文件
来源：http://jg.szxytkj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ty.haigaiapp.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://tr.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://aq.muxihuayi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.9csxet.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://qh.nszjky.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wu.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vm.jianghongdianzi.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mt.huixinmuqiang.cn

[F12] CSV 读写
来源：http://gi.nicolike.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://yw.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://br.bjjhwx.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://qe.shxzukj.cn

TS:   // 同上
来源：http://xf.muxihuayi.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://de.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://eo.asd995.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://na.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wy.jctech888.com.cn

================================================================================
来源：http://ty.yuntaijiaju.cn

G. 面向对象
来源：http://zc.bookmarksfly.cn

================================================================================
来源：http://ue.jianghongdianzi.cn

[G01] 定义类
来源：http://tp.bookmarksfly.cn

Py:   class User: pass
来源：http://il.yuntaijiaju.cn

PHP:  class User {}
来源：http://mm.521024.cn

JS:   class User {}
来源：http://ai.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://un.bjjhwx.cn

Java: class User {}
来源：http://jm.newstarts.cn

Go:   type User struct { Name string }
来源：http://ej.shxzukj.cn

Ruby: class User; end
来源：http://wm.colortex.cn

C#:   class User {}
来源：http://rd.lnxyls.cn

[G02] 构造函数
来源：http://ed.wgjwhj.cn

Py:   def __init__(self, name): self.name = name
来源：http://kk.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://rq.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://xh.yuexingan06.cn

TS:   constructor(public name: string) {}
来源：http://jk.gzmigu.cn

Java: User(String name) { this.name = name; }
来源：http://wc.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://to.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://lq.521024.cn

C#:   public User(string name) { Name = name; }
来源：http://bi.huixinmuqiang.cn

[G03] 实例属性
来源：http://tn.newstarts.cn

Py:   self.name = "x"
来源：http://pu.9csxet.cn

PHP:  public string $name = "x";
来源：http://bl.lnxyls.cn

JS:   this.name = "x";
来源：http://tp.panjiajie.cn

TS:   name: string = "x";
来源：http://hh.yuntaijiaju.cn

Java: private String name;
来源：http://kn.yuntaijiaju.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kl.gzmigu.cn

Ruby: @name = "x"
来源：http://gr.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://vr.jianghongdianzi.cn

[G04] 定义方法
来源：http://jg.huixinmuqiang.cn

Py:   def greet(self): return self.name
来源：http://wd.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://vg.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://vv.hnjuh.cn

TS:   greet(): string { return this.name; }
来源：http://kx.shxzskj.cn

Java: String greet() { return name; }
来源：http://zy.panjiajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ze.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://tw.nszjky.cn

C#:   public string Greet() => Name;
来源：http://we.shxzskj.cn

[G05] 继承
来源：http://ek.szsharing.cn

Py:   class Admin(User): pass
来源：http://qr.shxzskj.cn

PHP:  class Admin extends User {}
来源：http://lu.nicolike.cn

JS:   class Admin extends User {}
来源：http://uv.haigaiapp.cn

TS:   class Admin extends User {}
来源：http://ej.nicolike.cn

Java: class Admin extends User {}
来源：http://za.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rq.shtwfgs.cn

Ruby: class Admin < User; end
来源：http://mg.gzmigu.cn

C#:   class Admin : User {}
来源：http://mq.yuntaijiaju.cn

[G06] 重写方法
来源：http://nf.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://ga.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ki.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ab.shtwfgs.cn

TS:   greet(): string { return "admin"; }
来源：http://wk.jctech888.com.cn

Java: @Override String greet() { return "admin"; }
来源：http://jk.haigaiapp.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://vo.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://oh.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://vx.521024.cn

[G07] 调用父类方法
来源：http://qp.huixiangedu.cn

Py:   super().greet()
来源：http://fl.lnxyls.cn

PHP:  parent::greet();
来源：http://le.bjjhwx.cn

JS:   super.greet();
来源：http://ua.hnjuh.cn

TS:   super.greet();
来源：http://pk.shxzukj.cn

Java: super.greet();
来源：http://jo.lnxyls.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://iv.huanxung.cn

Ruby: super
来源：http://ra.szxytkj.cn

C#:   base.Greet();
来源：http://gu.9csxet.cn

[G08] 静态方法与属性
来源：http://ss.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ut.bookmarksfly.cn

PHP:  public static function f() {}
来源：http://bn.chemitech.net.cn

JS:   static f() {}
来源：http://dq.gzmigu.cn

TS:   static f(): void {}
来源：http://fr.huixiangedu.cn

Java: static void f() {}
来源：http://uv.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ol.newstarts.cn

Ruby: def self.f; end
来源：http://jy.szsharing.cn

C#:   public static void F() {}
来源：http://or.hahajie.cn

[G09] 接口 / 抽象类
来源：http://wd.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://kz.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ss.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ud.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://ms.shtwfgs.cn

Java: interface Shape { double area(); }
来源：http://ge.hahajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://xo.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://lh.huixiangedu.cn

C#:   interface IShape { double Area(); }
来源：http://bs.colortex.cn

[G10] 访问控制
来源：http://gt.521024.cn

Py:   约定 _protected / __private（不强制）
来源：http://as.muxihuayi.cn

PHP:  public / protected / private
来源：http://wt.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://yt.newstarts.cn

TS:   public / protected / private
来源：http://hx.bjjhwx.cn

Java: public / protected / private / 默认包级
来源：http://wd.jianghongdianzi.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://mi.szsharing.cn

Ruby: public / protected / private
来源：http://ly.szxytkj.cn

C#:   public / protected / private / internal
来源：http://ul.hahajie.cn

[G11] getter / setter
来源：http://tp.colortex.cn

Py:   @property 与 @x.setter
来源：http://wp.yuexingan06.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xv.huixinmuqiang.cn

JS:   get name() { return this._name; }
来源：http://vd.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://if.shxzukj.cn

Java: public String getName() { return name; }
来源：http://rl.asd995.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mc.panjiajie.cn

Ruby: attr_accessor :name
来源：http://yd.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://sl.shxzskj.cn

[G12] 对象转字符串
来源：http://rq.gzmigu.cn

Py:   def __str__(self): return self.name
来源：http://dn.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://to.nicolike.cn

JS:   toString() { return this.name; }
来源：http://ne.colortex.cn

TS:   toString(): string { return this.name; }
来源：http://rt.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://dv.newstarts.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vl.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://rc.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://oc.huixinmuqiang.cn

[G13] 判断对象类型
来源：http://ci.wgjwhj.cn

Py:   isinstance(u, User)
来源：http://ba.szsharing.cn

PHP:  $u instanceof User
来源：http://bt.huixinmuqiang.cn

JS:   u instanceof User
来源：http://wf.colortex.cn

TS:   u instanceof User
来源：http://rn.chemitech.net.cn

Java: u instanceof User
来源：http://vf.chemitech.net.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ea.colortex.cn

Ruby: u.is_a?(User)
来源：http://ep.hnjuh.cn

C#:   u is User
来源：http://zz.szsharing.cn


<!-- 参考信息 -->