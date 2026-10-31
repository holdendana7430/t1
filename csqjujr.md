代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://qc.asd995.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://st.newstarts.cn

[E16] 数字千分位
来源：http://ia.bjjhwx.cn

Py:   f"{1234567:,}"
来源：http://zz.nszjky.cn

PHP:  number_format(1234567);
来源：http://ju.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://oj.chemitech.net.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://ia.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://gq.szsharing.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://yz.nicolike.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://ct.nicolike.cn

C#:   1234567.ToString("N0")
来源：http://sh.szsharing.cn

[E17] 首字母大写
来源：http://fs.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hi.huanxung.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://mj.hahajie.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://yk.bookmarksfly.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zo.jctech888.com.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://ys.colortex.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://bz.colortex.cn

Ruby: s.capitalize
来源：http://nr.hnjuh.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://nk.huixiangedu.cn

[E18] 模板占位符替换
来源：http://br.521024.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://aj.9csxet.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://na.huixinmuqiang.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://wp.asd995.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hx.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://vn.szsharing.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://vj.huanxung.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://ep.chemitech.net.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://gw.nszjky.cn

[E19] 多行文本按行拆分
来源：http://xd.huixiangedu.cn

Py:   s.splitlines()
来源：http://hx.asd995.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://dx.jctech888.com.cn

JS:   s.split(/\r?\n/)
来源：http://tn.jctech888.com.cn

TS:   s.split(/\r?\n/)
来源：http://qh.huanxung.cn

Java: s.lines().toList()
来源：http://kh.szsharing.cn

Go:   strings.Split(s, "\n")
来源：http://kt.yuexingan06.cn

Ruby: s.lines
来源：http://uf.lnxyls.cn

C#:   s.Split('\n')
来源：http://yr.szsharing.cn

[E20] 判断字符串是否为空
来源：http://mt.hnjuh.cn

Py:   if not s:
来源：http://ig.hnjuh.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://xu.yuntaijiaju.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ub.jctech888.com.cn

TS:   if (s === "") {}
来源：http://hb.huanxung.cn

Java: if (s.isEmpty()) {}
来源：http://ye.haigaiapp.cn

Go:   if s == "" {}
来源：http://hm.chemitech.net.cn

Ruby: if s.empty?
来源：http://fc.szxytkj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://qw.newstarts.cn

[E21] 超长截断加省略号
来源：http://pv.colortex.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://od.hnjuh.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://sp.asd995.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://gz.hahajie.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://si.shtwfgs.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://bl.huixiangedu.cn

Go:   // 按 rune 判断长度后截断
来源：http://nb.wgjwhj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hn.chemitech.net.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pa.huixinmuqiang.cn

[E22] 字节长度与字符长度
来源：http://iq.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xd.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://os.yuntaijiaju.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://nb.521024.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://zz.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pa.panjiajie.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://kt.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://dx.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mx.haigaiapp.cn

================================================================================
来源：http://iu.huixiangedu.cn

F. 文件与目录
来源：http://sh.szsharing.cn

================================================================================
来源：http://wr.muxihuayi.cn

[F01] 读取整个文件
来源：http://xq.nszjky.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://kw.lnxyls.cn

PHP:  file_get_contents("a.txt");
来源：http://pn.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://pd.huixiangedu.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wx.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://km.huanxung.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://an.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://fx.bookmarksfly.cn

C#:   File.ReadAllText("a.txt");
来源：http://pg.szsharing.cn

[F02] 逐行读取文件
来源：http://kh.shxzukj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ji.shxzukj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://zd.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ry.chemitech.net.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zz.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://lk.bookmarksfly.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://oe.haigaiapp.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://uf.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://pt.gzmigu.cn

[F03] 写入文件（覆盖）
来源：http://bv.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ro.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://lr.newstarts.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://he.nicolike.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xw.muxihuayi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://av.asd995.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://lu.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://qr.jianghongdianzi.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://jc.huanxung.cn

[F04] 追加写入文件
来源：http://uo.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://tr.chemitech.net.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://yt.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nk.szsharing.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://eu.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mr.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://jb.9csxet.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qk.wgjwhj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://cb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://gp.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://au.wgjwhj.cn

PHP:  file_exists("a.txt");
来源：http://sr.szxytkj.cn

JS:   fs.existsSync("a.txt")
来源：http://ns.szxytkj.cn

TS:   fs.existsSync("a.txt")
来源：http://fl.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://xt.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://tw.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://bi.bookmarksfly.cn

C#:   File.Exists("a.txt")
来源：http://ih.chemitech.net.cn

[F06] 删除文件
来源：http://fm.asd995.cn

Py:   os.remove("a.txt")
来源：http://zd.nicolike.cn

PHP:  unlink("a.txt");
来源：http://xe.yuntaijiaju.cn

JS:   fs.unlinkSync("a.txt")
来源：http://nc.szsharing.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sv.newstarts.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ay.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://rb.muxihuayi.cn

Ruby: File.delete("a.txt")
来源：http://rw.newstarts.cn

C#:   File.Delete("a.txt");
来源：http://wv.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://ym.szxytkj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://jm.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ag.shtwfgs.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rw.nszjky.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xz.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ad.gzmigu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jh.bjjhwx.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://so.shtwfgs.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sh.colortex.cn

[F08] 遍历目录
来源：http://in.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://zr.wgjwhj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://qo.9csxet.cn

JS:   fs.readdirSync("dir")
来源：http://rd.huixiangedu.cn

TS:   fs.readdirSync("dir")
来源：http://vq.asd995.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://sr.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ni.asd995.cn

Ruby: Dir.children("dir")
来源：http://lj.shxzukj.cn

C#:   Directory.GetFiles("dir")
来源：http://ej.huixiangedu.cn

[F09] 获取文件大小
来源：http://ia.bjjhwx.cn

Py:   os.path.getsize("a.txt")
来源：http://ri.yuntaijiaju.cn

PHP:  filesize("a.txt");
来源：http://kr.hahajie.cn

JS:   fs.statSync("a.txt").size
来源：http://yp.szsharing.cn

TS:   fs.statSync("a.txt").size
来源：http://pz.shxzskj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lf.9csxet.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://za.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://cb.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://vy.wgjwhj.cn

[F10] 取文件扩展名 / 文件名
来源：http://lq.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ib.shxzukj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rn.bookmarksfly.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wy.szsharing.cn

TS:   path.extname("a.txt")
来源：http://ya.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://sc.haigaiapp.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://aj.szxytkj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dz.colortex.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://lx.newstarts.cn

[F11] 复制与移动文件
来源：http://df.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://jv.jianghongdianzi.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://jm.jctech888.com.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hh.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://yd.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://so.shxzskj.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://jd.bookmarksfly.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://uk.jctech888.com.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://os.wgjwhj.cn

[F12] CSV 读写
来源：http://fd.huixinmuqiang.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hw.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://br.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://fc.bookmarksfly.cn

TS:   // 同上
来源：http://eu.gzmigu.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://oj.hnjuh.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://gs.yuexingan06.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://km.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qc.bjjhwx.cn

================================================================================
来源：http://mg.bookmarksfly.cn

G. 面向对象
来源：http://yz.huanxung.cn

================================================================================
来源：http://sk.huanxung.cn

[G01] 定义类
来源：http://rw.nicolike.cn

Py:   class User: pass
来源：http://kp.jianghongdianzi.cn

PHP:  class User {}
来源：http://nf.nszjky.cn

JS:   class User {}
来源：http://qp.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://wb.hahajie.cn

Java: class User {}
来源：http://nm.panjiajie.cn

Go:   type User struct { Name string }
来源：http://hr.lnxyls.cn

Ruby: class User; end
来源：http://eg.asd995.cn

C#:   class User {}
来源：http://lc.jctech888.com.cn

[G02] 构造函数
来源：http://ub.panjiajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://hd.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://jp.jctech888.com.cn

JS:   constructor(name) { this.name = name; }
来源：http://hd.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://hc.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://uy.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://he.shtwfgs.cn

Ruby: def initialize(name); @name = name; end
来源：http://hl.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://jp.szsharing.cn

[G03] 实例属性
来源：http://tr.chemitech.net.cn

Py:   self.name = "x"
来源：http://up.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://nt.shxzskj.cn

JS:   this.name = "x";
来源：http://oy.nszjky.cn

TS:   name: string = "x";
来源：http://ph.muxihuayi.cn

Java: private String name;
来源：http://hp.asd995.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wh.huixiangedu.cn

Ruby: @name = "x"
来源：http://pc.asd995.cn

C#:   public string Name { get; set; } = "x";
来源：http://fc.yuntaijiaju.cn

[G04] 定义方法
来源：http://kb.newstarts.cn

Py:   def greet(self): return self.name
来源：http://ax.521024.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ak.yuntaijiaju.cn

JS:   greet() { return this.name; }
来源：http://pr.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://tl.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://zc.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://cj.muxihuayi.cn

Ruby: def greet; @name; end
来源：http://tr.jianghongdianzi.cn

C#:   public string Greet() => Name;
来源：http://fl.haigaiapp.cn

[G05] 继承
来源：http://vx.lnxyls.cn

Py:   class Admin(User): pass
来源：http://oa.nszjky.cn

PHP:  class Admin extends User {}
来源：http://sa.yuntaijiaju.cn

JS:   class Admin extends User {}
来源：http://ts.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://it.521024.cn

Java: class Admin extends User {}
来源：http://ik.bookmarksfly.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ne.jianghongdianzi.cn

Ruby: class Admin < User; end
来源：http://ft.jctech888.com.cn

C#:   class Admin : User {}
来源：http://sx.yuexingan06.cn

[G06] 重写方法
来源：http://lf.asd995.cn

Py:   def greet(self): return "admin"
来源：http://mk.szxytkj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://tn.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://du.panjiajie.cn

TS:   greet(): string { return "admin"; }
来源：http://jy.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://gf.nicolike.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://fe.jianghongdianzi.cn

Ruby: def greet; "admin"; end
来源：http://zj.shxzskj.cn

C#:   public override string Greet() => "admin";
来源：http://qk.nszjky.cn

[G07] 调用父类方法
来源：http://jv.hahajie.cn

Py:   super().greet()
来源：http://bu.nszjky.cn

PHP:  parent::greet();
来源：http://le.newstarts.cn

JS:   super.greet();
来源：http://vo.panjiajie.cn

TS:   super.greet();
来源：http://zz.lnxyls.cn

Java: super.greet();
来源：http://ks.hahajie.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://fn.lnxyls.cn

Ruby: super
来源：http://os.colortex.cn

C#:   base.Greet();
来源：http://cy.huanxung.cn

[G08] 静态方法与属性
来源：http://hd.521024.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fz.bjjhwx.cn

PHP:  public static function f() {}
来源：http://pl.colortex.cn

JS:   static f() {}
来源：http://vf.wgjwhj.cn

TS:   static f(): void {}
来源：http://fg.hahajie.cn

Java: static void f() {}
来源：http://vh.jctech888.com.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://un.jianghongdianzi.cn

Ruby: def self.f; end
来源：http://jn.gzmigu.cn

C#:   public static void F() {}
来源：http://jp.521024.cn

[G09] 接口 / 抽象类
来源：http://xn.bjjhwx.cn

Py:   from abc import ABC, abstractmethod
来源：http://xp.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://lu.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://uz.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://jm.9csxet.cn

Java: interface Shape { double area(); }
来源：http://te.hnjuh.cn

Go:   type Shape interface { Area() float64 }
来源：http://zl.szsharing.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gs.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://ri.panjiajie.cn

[G10] 访问控制
来源：http://mw.shxzukj.cn

Py:   约定 _protected / __private（不强制）
来源：http://ac.szxytkj.cn

PHP:  public / protected / private
来源：http://jj.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://hd.muxihuayi.cn

TS:   public / protected / private
来源：http://aa.jianghongdianzi.cn

Java: public / protected / private / 默认包级
来源：http://dw.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://ws.yuntaijiaju.cn

Ruby: public / protected / private
来源：http://vj.gzmigu.cn

C#:   public / protected / private / internal
来源：http://vk.yuexingan06.cn

[G11] getter / setter
来源：http://ts.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://dm.huixiangedu.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://fw.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://fg.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://rw.huixinmuqiang.cn

Java: public String getName() { return name; }
来源：http://ns.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hb.huanxung.cn

Ruby: attr_accessor :name
来源：http://et.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://zg.nszjky.cn

[G12] 对象转字符串
来源：http://wg.hnjuh.cn

Py:   def __str__(self): return self.name
来源：http://le.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://vr.nicolike.cn

JS:   toString() { return this.name; }
来源：http://kd.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://uv.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://gy.huanxung.cn

Go:   func (u User) String() string { return u.Name }
来源：http://gs.colortex.cn

Ruby: def to_s; @name; end
来源：http://yq.yuexingan06.cn

C#:   public override string ToString() => Name;
来源：http://ai.521024.cn

[G13] 判断对象类型
来源：http://he.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://ms.colortex.cn

PHP:  $u instanceof User
来源：http://sd.chemitech.net.cn

JS:   u instanceof User
来源：http://se.yuntaijiaju.cn

TS:   u instanceof User
来源：http://jo.shxzukj.cn

Java: u instanceof User
来源：http://xu.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://is.bookmarksfly.cn

Ruby: u.is_a?(User)
来源：http://ss.yuexingan06.cn

C#:   u is User
来源：http://nf.jianghongdianzi.cn

[G14] 数据类 / record
来源：http://py.wgjwhj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nc.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://gw.bjjhwx.cn

JS:   // 无内置：普通类或对象字面量
来源：http://mo.szsharing.cn


<!-- 参考信息 -->