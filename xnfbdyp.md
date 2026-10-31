代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://st.huixiangedu.cn

TS:   // 同上，务必做 XSS 过滤
来源：http://yq.nszjky.cn

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mv.haigaiapp.cn

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://do.nszjky.cn

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ye.huixinmuqiang.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://ol.shtwfgs.cn

[E16] 数字千分位
来源：http://cb.bookmarksfly.cn

Py:   f"{1234567:,}"
来源：http://nz.yuntaijiaju.cn

PHP:  number_format(1234567);
来源：http://wd.panjiajie.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://ty.yuexingan06.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://iw.hahajie.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://vb.nicolike.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://qg.shtwfgs.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xl.9csxet.cn

C#:   1234567.ToString("N0")
来源：http://ko.huanxung.cn

[E17] 首字母大写
来源：http://gf.521024.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://ik.colortex.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://qw.shtwfgs.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ue.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://tb.9csxet.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://gy.shxzskj.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://xh.asd995.cn

Ruby: s.capitalize
来源：http://zq.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zi.hnjuh.cn

[E18] 模板占位符替换
来源：http://sp.newstarts.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://ir.shxzskj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://jw.jctech888.com.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://pb.lnxyls.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://yy.bookmarksfly.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mp.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://od.gzmigu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hm.hnjuh.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://aw.9csxet.cn

[E19] 多行文本按行拆分
来源：http://mw.bjjhwx.cn

Py:   s.splitlines()
来源：http://qf.nszjky.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ml.panjiajie.cn

JS:   s.split(/\r?\n/)
来源：http://wi.521024.cn

TS:   s.split(/\r?\n/)
来源：http://nt.shxzukj.cn

Java: s.lines().toList()
来源：http://rp.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://bj.huanxung.cn

Ruby: s.lines
来源：http://xb.gzmigu.cn

C#:   s.Split('\n')
来源：http://vf.huanxung.cn

[E20] 判断字符串是否为空
来源：http://jq.hahajie.cn

Py:   if not s:
来源：http://fe.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://oa.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://qt.szxytkj.cn

TS:   if (s === "") {}
来源：http://zd.521024.cn

Java: if (s.isEmpty()) {}
来源：http://xq.asd995.cn

Go:   if s == "" {}
来源：http://cc.huixiangedu.cn

Ruby: if s.empty?
来源：http://qh.bookmarksfly.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ti.wgjwhj.cn

[E21] 超长截断加省略号
来源：http://ma.shxzukj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://ft.nszjky.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://za.wgjwhj.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://no.huanxung.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://or.szxytkj.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oo.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://si.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://fe.jianghongdianzi.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://dj.newstarts.cn

[E22] 字节长度与字符长度
来源：http://ge.jianghongdianzi.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ay.szsharing.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sf.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jy.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ys.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://yp.jianghongdianzi.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wk.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://yi.shtwfgs.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ja.lnxyls.cn

================================================================================
来源：http://zq.gzmigu.cn

F. 文件与目录
来源：http://yz.shxzukj.cn

================================================================================
来源：http://mi.panjiajie.cn

[F01] 读取整个文件
来源：http://mm.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://le.nicolike.cn

PHP:  file_get_contents("a.txt");
来源：http://lk.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pe.nszjky.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://qx.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://jd.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ms.shtwfgs.cn

Ruby: File.read("a.txt")
来源：http://iw.shtwfgs.cn

C#:   File.ReadAllText("a.txt");
来源：http://oy.yuntaijiaju.cn

[F02] 逐行读取文件
来源：http://fq.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qz.panjiajie.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://ey.yuexingan06.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sx.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://bk.szxytkj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://js.jctech888.com.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wq.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ko.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://tx.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://jo.szsharing.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://yt.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://tl.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rz.panjiajie.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pj.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://fx.huixinmuqiang.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fi.yuexingan06.cn

Ruby: File.write("a.txt", "hi")
来源：http://yx.gzmigu.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://sz.shxzukj.cn

[F04] 追加写入文件
来源：http://hv.newstarts.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zq.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://is.hahajie.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zh.huanxung.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://jq.yuexingan06.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://qh.huixinmuqiang.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ft.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://do.bookmarksfly.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://oa.lnxyls.cn

[F05] 判断文件或目录是否存在
来源：http://ho.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://id.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://lk.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://kh.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://dm.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ed.nszjky.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://rb.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://zh.colortex.cn

C#:   File.Exists("a.txt")
来源：http://lr.wgjwhj.cn

[F06] 删除文件
来源：http://td.gzmigu.cn

Py:   os.remove("a.txt")
来源：http://ql.huixinmuqiang.cn

PHP:  unlink("a.txt");
来源：http://zu.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nu.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://af.9csxet.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lx.nszjky.cn

Go:   os.Remove("a.txt")
来源：http://uz.yuntaijiaju.cn

Ruby: File.delete("a.txt")
来源：http://ag.hnjuh.cn

C#:   File.Delete("a.txt");
来源：http://jt.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://sd.lnxyls.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://js.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://cn.bjjhwx.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hc.colortex.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xx.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://gg.nicolike.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kx.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ps.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://kp.521024.cn

[F08] 遍历目录
来源：http://mv.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vs.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ez.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://bh.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://ab.huanxung.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://aq.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://vd.yuexingan06.cn

Ruby: Dir.children("dir")
来源：http://aa.hahajie.cn

C#:   Directory.GetFiles("dir")
来源：http://ms.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://df.shtwfgs.cn

Py:   os.path.getsize("a.txt")
来源：http://dv.shxzukj.cn

PHP:  filesize("a.txt");
来源：http://uk.newstarts.cn

JS:   fs.statSync("a.txt").size
来源：http://fa.huanxung.cn

TS:   fs.statSync("a.txt").size
来源：http://xa.bjjhwx.cn

Java: Files.size(Path.of("a.txt"))
来源：http://fb.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://dq.huanxung.cn

Ruby: File.size("a.txt")
来源：http://el.szsharing.cn

C#:   new FileInfo("a.txt").Length
来源：http://rx.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://jj.bjjhwx.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nk.hahajie.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nk.jctech888.com.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ey.yuntaijiaju.cn

TS:   path.extname("a.txt")
来源：http://ze.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sd.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://gk.huanxung.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://pr.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wi.panjiajie.cn

[F11] 复制与移动文件
来源：http://rd.gzmigu.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ky.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sv.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ji.nszjky.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ya.wgjwhj.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bd.yuexingan06.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nj.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://zr.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mi.hahajie.cn

[F12] CSV 读写
来源：http://tm.haigaiapp.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://vv.jctech888.com.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://qf.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mw.shxzskj.cn

TS:   // 同上
来源：http://mj.yuexingan06.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://vo.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bf.9csxet.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wv.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://rg.gzmigu.cn

================================================================================
来源：http://lu.muxihuayi.cn

G. 面向对象
来源：http://ad.lnxyls.cn

================================================================================
来源：http://ti.nicolike.cn

[G01] 定义类
来源：http://nf.bjjhwx.cn

Py:   class User: pass
来源：http://sp.521024.cn

PHP:  class User {}
来源：http://it.hahajie.cn

JS:   class User {}
来源：http://af.yuexingan06.cn

TS:   class User { name: string = ""; }
来源：http://wh.hnjuh.cn

Java: class User {}
来源：http://te.huixinmuqiang.cn

Go:   type User struct { Name string }
来源：http://ki.521024.cn

Ruby: class User; end
来源：http://yd.hahajie.cn

C#:   class User {}
来源：http://xy.huixinmuqiang.cn

[G02] 构造函数
来源：http://yo.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://ki.yuntaijiaju.cn

PHP:  public function __construct(public string $name) {}
来源：http://dk.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://wd.jianghongdianzi.cn

TS:   constructor(public name: string) {}
来源：http://ol.521024.cn

Java: User(String name) { this.name = name; }
来源：http://sw.hahajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ij.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://fa.hnjuh.cn

C#:   public User(string name) { Name = name; }
来源：http://jz.bjjhwx.cn

[G03] 实例属性
来源：http://fa.yuntaijiaju.cn

Py:   self.name = "x"
来源：http://sw.haigaiapp.cn

PHP:  public string $name = "x";
来源：http://rb.panjiajie.cn

JS:   this.name = "x";
来源：http://ob.huixiangedu.cn

TS:   name: string = "x";
来源：http://of.asd995.cn

Java: private String name;
来源：http://fn.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://sp.haigaiapp.cn

Ruby: @name = "x"
来源：http://fc.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://hh.huixinmuqiang.cn

[G04] 定义方法
来源：http://rh.bookmarksfly.cn

Py:   def greet(self): return self.name
来源：http://zc.colortex.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qc.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://pf.muxihuayi.cn

TS:   greet(): string { return this.name; }
来源：http://wn.huixinmuqiang.cn

Java: String greet() { return name; }
来源：http://rd.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mc.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://zp.szsharing.cn

C#:   public string Greet() => Name;
来源：http://vj.szsharing.cn

[G05] 继承
来源：http://xi.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://fk.9csxet.cn

PHP:  class Admin extends User {}
来源：http://xx.colortex.cn

JS:   class Admin extends User {}
来源：http://ud.nszjky.cn

TS:   class Admin extends User {}
来源：http://tu.bookmarksfly.cn

Java: class Admin extends User {}
来源：http://an.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xo.bjjhwx.cn

Ruby: class Admin < User; end
来源：http://bi.chemitech.net.cn

C#:   class Admin : User {}
来源：http://bc.huixinmuqiang.cn

[G06] 重写方法
来源：http://xy.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://su.nicolike.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://pf.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://gi.yuntaijiaju.cn

TS:   greet(): string { return "admin"; }
来源：http://zh.bjjhwx.cn

Java: @Override String greet() { return "admin"; }
来源：http://tg.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://an.yuexingan06.cn

Ruby: def greet; "admin"; end
来源：http://do.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://vi.521024.cn

[G07] 调用父类方法
来源：http://po.bjjhwx.cn

Py:   super().greet()
来源：http://sx.chemitech.net.cn

PHP:  parent::greet();
来源：http://sc.newstarts.cn

JS:   super.greet();
来源：http://bc.bjjhwx.cn

TS:   super.greet();
来源：http://op.yuntaijiaju.cn

Java: super.greet();
来源：http://zj.bookmarksfly.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://ct.bjjhwx.cn

Ruby: super
来源：http://pk.colortex.cn

C#:   base.Greet();
来源：http://wo.hahajie.cn

[G08] 静态方法与属性
来源：http://fb.jianghongdianzi.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://gi.huanxung.cn

PHP:  public static function f() {}
来源：http://mt.asd995.cn

JS:   static f() {}
来源：http://km.wgjwhj.cn

TS:   static f(): void {}
来源：http://ig.asd995.cn

Java: static void f() {}
来源：http://zz.shxzukj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://pj.szsharing.cn

Ruby: def self.f; end
来源：http://wn.shxzukj.cn

C#:   public static void F() {}
来源：http://pl.huixiangedu.cn

[G09] 接口 / 抽象类
来源：http://gd.colortex.cn

Py:   from abc import ABC, abstractmethod
来源：http://tp.haigaiapp.cn

PHP:  interface Shape { public function area(): float; }
来源：http://qf.yuexingan06.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dz.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://qo.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://ds.asd995.cn

Go:   type Shape interface { Area() float64 }
来源：http://ca.gzmigu.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://or.jctech888.com.cn

C#:   interface IShape { double Area(); }
来源：http://yi.haigaiapp.cn

[G10] 访问控制
来源：http://ek.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://fj.nszjky.cn

PHP:  public / protected / private
来源：http://ut.asd995.cn

JS:   #private 字段；其余公开
来源：http://ik.521024.cn

TS:   public / protected / private
来源：http://mq.shtwfgs.cn

Java: public / protected / private / 默认包级
来源：http://ag.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://fd.wgjwhj.cn

Ruby: public / protected / private
来源：http://si.hnjuh.cn

C#:   public / protected / private / internal
来源：http://wp.asd995.cn

[G11] getter / setter
来源：http://zc.colortex.cn

Py:   @property 与 @x.setter
来源：http://wq.chemitech.net.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://by.bookmarksfly.cn

JS:   get name() { return this._name; }
来源：http://ss.gzmigu.cn

TS:   get name(): string { return this._name; }
来源：http://nq.lnxyls.cn

Java: public String getName() { return name; }
来源：http://rw.panjiajie.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ns.hnjuh.cn

Ruby: attr_accessor :name
来源：http://cs.muxihuayi.cn

C#:   public string Name { get; set; }
来源：http://kv.9csxet.cn

[G12] 对象转字符串
来源：http://ne.hahajie.cn

Py:   def __str__(self): return self.name
来源：http://cs.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ap.hahajie.cn

JS:   toString() { return this.name; }
来源：http://mp.newstarts.cn

TS:   toString(): string { return this.name; }
来源：http://xj.panjiajie.cn

Java: @Override public String toString() { return name; }
来源：http://te.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ez.shxzskj.cn

Ruby: def to_s; @name; end
来源：http://uu.colortex.cn

C#:   public override string ToString() => Name;
来源：http://tn.panjiajie.cn

[G13] 判断对象类型
来源：http://dz.9csxet.cn

Py:   isinstance(u, User)
来源：http://cq.szsharing.cn

PHP:  $u instanceof User
来源：http://kj.gzmigu.cn

JS:   u instanceof User
来源：http://jr.521024.cn

TS:   u instanceof User
来源：http://kc.wgjwhj.cn

Java: u instanceof User
来源：http://zg.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://mk.colortex.cn

Ruby: u.is_a?(User)
来源：http://uq.huixinmuqiang.cn

C#:   u is User
来源：http://pi.muxihuayi.cn


<!-- 参考信息 -->