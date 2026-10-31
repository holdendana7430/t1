代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://tw.jianghongdianzi.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://de.gzmigu.cn

[E16] 数字千分位
来源：http://in.szxytkj.cn

Py:   f"{1234567:,}"
来源：http://bi.szxytkj.cn

PHP:  number_format(1234567);
来源：http://fy.newstarts.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://qn.bjjhwx.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://sl.yuntaijiaju.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://lo.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://lj.521024.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://vs.lnxyls.cn

C#:   1234567.ToString("N0")
来源：http://wa.521024.cn

[E17] 首字母大写
来源：http://rt.9csxet.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://yl.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ve.9csxet.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ij.lnxyls.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://zq.yuntaijiaju.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wq.bookmarksfly.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mq.bjjhwx.cn

Ruby: s.capitalize
来源：http://ie.shxzukj.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://xt.asd995.cn

[E18] 模板占位符替换
来源：http://pg.gzmigu.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://tk.szxytkj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://yb.bookmarksfly.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ja.nicolike.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://jy.yuntaijiaju.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://kl.lnxyls.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://yp.nicolike.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://du.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://am.haigaiapp.cn

[E19] 多行文本按行拆分
来源：http://hb.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://mu.huixiangedu.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://xc.huixiangedu.cn

JS:   s.split(/\r?\n/)
来源：http://eb.9csxet.cn

TS:   s.split(/\r?\n/)
来源：http://dy.gzmigu.cn

Java: s.lines().toList()
来源：http://jv.yuexingan06.cn

Go:   strings.Split(s, "\n")
来源：http://pn.521024.cn

Ruby: s.lines
来源：http://gq.muxihuayi.cn

C#:   s.Split('\n')
来源：http://cb.muxihuayi.cn

[E20] 判断字符串是否为空
来源：http://jf.shxzukj.cn

Py:   if not s:
来源：http://vv.jianghongdianzi.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://yw.panjiajie.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://en.yuexingan06.cn

TS:   if (s === "") {}
来源：http://hc.panjiajie.cn

Java: if (s.isEmpty()) {}
来源：http://rp.szsharing.cn

Go:   if s == "" {}
来源：http://gi.huixiangedu.cn

Ruby: if s.empty?
来源：http://sa.wgjwhj.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://cv.huixiangedu.cn

[E21] 超长截断加省略号
来源：http://gy.szxytkj.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://jw.shxzukj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://eq.huanxung.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://us.haigaiapp.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mb.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://xv.haigaiapp.cn

Go:   // 按 rune 判断长度后截断
来源：http://qe.gzmigu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://cd.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wi.newstarts.cn

[E22] 字节长度与字符长度
来源：http://ic.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://qm.huixiangedu.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://pp.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://tf.nszjky.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yf.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://qy.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://sj.asd995.cn

Ruby: s.bytesize;  s.length
来源：http://cy.haigaiapp.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://gq.huixinmuqiang.cn

================================================================================
来源：http://gl.bookmarksfly.cn

F. 文件与目录
来源：http://hz.shxzskj.cn

================================================================================
来源：http://mp.hahajie.cn

[F01] 读取整个文件
来源：http://jf.521024.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wg.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://gf.lnxyls.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://dh.muxihuayi.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://vh.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fr.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://tr.muxihuayi.cn

Ruby: File.read("a.txt")
来源：http://ar.9csxet.cn

C#:   File.ReadAllText("a.txt");
来源：http://vn.huixiangedu.cn

[F02] 逐行读取文件
来源：http://pu.wgjwhj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://of.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hv.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://zm.lnxyls.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://dr.bookmarksfly.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wg.huixinmuqiang.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://yr.asd995.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://rn.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://js.chemitech.net.cn

[F03] 写入文件（覆盖）
来源：http://yi.lnxyls.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://nq.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ws.yuexingan06.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iv.asd995.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ds.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wg.shxzskj.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pi.panjiajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://hv.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oo.9csxet.cn

[F04] 追加写入文件
来源：http://ib.haigaiapp.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zr.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vy.huixinmuqiang.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://tj.9csxet.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wd.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://kd.chemitech.net.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://io.lnxyls.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wc.hahajie.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ph.panjiajie.cn

[F05] 判断文件或目录是否存在
来源：http://rz.lnxyls.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://am.colortex.cn

PHP:  file_exists("a.txt");
来源：http://iy.colortex.cn

JS:   fs.existsSync("a.txt")
来源：http://lo.lnxyls.cn

TS:   fs.existsSync("a.txt")
来源：http://rm.panjiajie.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ng.yuexingan06.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://gy.yuexingan06.cn

Ruby: File.exist?("a.txt")
来源：http://zc.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://cv.jctech888.com.cn

[F06] 删除文件
来源：http://ls.nszjky.cn

Py:   os.remove("a.txt")
来源：http://lz.lnxyls.cn

PHP:  unlink("a.txt");
来源：http://oq.521024.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zt.colortex.cn

TS:   fs.unlinkSync("a.txt")
来源：http://jx.bjjhwx.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://lg.asd995.cn

Go:   os.Remove("a.txt")
来源：http://ap.haigaiapp.cn

Ruby: File.delete("a.txt")
来源：http://yg.hahajie.cn

C#:   File.Delete("a.txt");
来源：http://cc.nszjky.cn

[F07] 创建目录（含多级）
来源：http://lb.asd995.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://pq.nicolike.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xq.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yn.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://og.wgjwhj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tn.newstarts.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://xh.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ny.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ui.9csxet.cn

[F08] 遍历目录
来源：http://ru.haigaiapp.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ja.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://dm.chemitech.net.cn

JS:   fs.readdirSync("dir")
来源：http://pe.huixinmuqiang.cn

TS:   fs.readdirSync("dir")
来源：http://zj.muxihuayi.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://if.newstarts.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://qc.asd995.cn

Ruby: Dir.children("dir")
来源：http://pg.bookmarksfly.cn

C#:   Directory.GetFiles("dir")
来源：http://gi.nszjky.cn

[F09] 获取文件大小
来源：http://me.huixinmuqiang.cn

Py:   os.path.getsize("a.txt")
来源：http://ud.9csxet.cn

PHP:  filesize("a.txt");
来源：http://tp.9csxet.cn

JS:   fs.statSync("a.txt").size
来源：http://ya.newstarts.cn

TS:   fs.statSync("a.txt").size
来源：http://ao.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gk.szsharing.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://my.chemitech.net.cn

Ruby: File.size("a.txt")
来源：http://sw.hahajie.cn

C#:   new FileInfo("a.txt").Length
来源：http://cs.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://sk.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mo.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://zc.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://gd.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://br.jctech888.com.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ik.muxihuayi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xn.9csxet.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ij.9csxet.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xb.szsharing.cn

[F11] 复制与移动文件
来源：http://qs.asd995.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dn.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://nn.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://sc.lnxyls.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://is.panjiajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://vv.yuntaijiaju.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://fo.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mi.hnjuh.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kz.szxytkj.cn

[F12] CSV 读写
来源：http://mt.yuexingan06.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sa.521024.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://em.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://cv.huixiangedu.cn

TS:   // 同上
来源：http://lw.shxzskj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fx.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sd.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ft.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://qv.wgjwhj.cn

================================================================================
来源：http://wa.bookmarksfly.cn

G. 面向对象
来源：http://iu.chemitech.net.cn

================================================================================
来源：http://vr.asd995.cn

[G01] 定义类
来源：http://mx.chemitech.net.cn

Py:   class User: pass
来源：http://vw.hahajie.cn

PHP:  class User {}
来源：http://cb.9csxet.cn

JS:   class User {}
来源：http://ns.shxzskj.cn

TS:   class User { name: string = ""; }
来源：http://id.yuntaijiaju.cn

Java: class User {}
来源：http://ed.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://ro.yuexingan06.cn

Ruby: class User; end
来源：http://oq.huixiangedu.cn

C#:   class User {}
来源：http://tg.bjjhwx.cn

[G02] 构造函数
来源：http://yp.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://pm.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://gp.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://mz.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://bh.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://td.muxihuayi.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wy.panjiajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://jk.jctech888.com.cn

C#:   public User(string name) { Name = name; }
来源：http://vd.hnjuh.cn

[G03] 实例属性
来源：http://so.nszjky.cn

Py:   self.name = "x"
来源：http://se.huanxung.cn

PHP:  public string $name = "x";
来源：http://hm.hahajie.cn

JS:   this.name = "x";
来源：http://kc.shtwfgs.cn

TS:   name: string = "x";
来源：http://az.chemitech.net.cn

Java: private String name;
来源：http://xj.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rz.panjiajie.cn

Ruby: @name = "x"
来源：http://vo.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://iy.nszjky.cn

[G04] 定义方法
来源：http://ia.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://wg.lnxyls.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://pc.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://gx.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://hn.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://kk.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://eu.gzmigu.cn

Ruby: def greet; @name; end
来源：http://ny.shxzukj.cn

C#:   public string Greet() => Name;
来源：http://sd.hnjuh.cn

[G05] 继承
来源：http://jv.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://sz.hahajie.cn

PHP:  class Admin extends User {}
来源：http://fe.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://nv.gzmigu.cn

TS:   class Admin extends User {}
来源：http://dv.shtwfgs.cn

Java: class Admin extends User {}
来源：http://vs.nszjky.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://yk.jctech888.com.cn

Ruby: class Admin < User; end
来源：http://rx.nicolike.cn

C#:   class Admin : User {}
来源：http://ei.hahajie.cn

[G06] 重写方法
来源：http://pl.newstarts.cn

Py:   def greet(self): return "admin"
来源：http://dv.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cb.shtwfgs.cn

JS:   greet() { return "admin"; }
来源：http://wv.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://bg.huixinmuqiang.cn

Java: @Override String greet() { return "admin"; }
来源：http://ft.wgjwhj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hy.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://yy.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://xk.shxzskj.cn

[G07] 调用父类方法
来源：http://if.nszjky.cn

Py:   super().greet()
来源：http://wh.521024.cn

PHP:  parent::greet();
来源：http://vj.haigaiapp.cn

JS:   super.greet();
来源：http://qf.yuntaijiaju.cn

TS:   super.greet();
来源：http://th.lnxyls.cn

Java: super.greet();
来源：http://vm.asd995.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://at.huanxung.cn

Ruby: super
来源：http://bg.521024.cn

C#:   base.Greet();
来源：http://oz.jctech888.com.cn

[G08] 静态方法与属性
来源：http://dy.yuexingan06.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://xn.gzmigu.cn

PHP:  public static function f() {}
来源：http://ad.shxzukj.cn

JS:   static f() {}
来源：http://jz.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://rn.hnjuh.cn

Java: static void f() {}
来源：http://yb.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://px.gzmigu.cn

Ruby: def self.f; end
来源：http://yn.hnjuh.cn

C#:   public static void F() {}
来源：http://rz.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://oq.szsharing.cn

Py:   from abc import ABC, abstractmethod
来源：http://zi.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://al.jianghongdianzi.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dn.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://og.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://ye.panjiajie.cn

Go:   type Shape interface { Area() float64 }
来源：http://mb.hahajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ea.hnjuh.cn

C#:   interface IShape { double Area(); }
来源：http://xp.lnxyls.cn

[G10] 访问控制
来源：http://pj.nicolike.cn

Py:   约定 _protected / __private（不强制）
来源：http://es.jianghongdianzi.cn

PHP:  public / protected / private
来源：http://hj.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://nq.chemitech.net.cn

TS:   public / protected / private
来源：http://ae.colortex.cn

Java: public / protected / private / 默认包级
来源：http://lf.521024.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://px.hahajie.cn

Ruby: public / protected / private
来源：http://mw.yuexingan06.cn

C#:   public / protected / private / internal
来源：http://kl.9csxet.cn

[G11] getter / setter
来源：http://ir.9csxet.cn

Py:   @property 与 @x.setter
来源：http://hq.bookmarksfly.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ne.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://xd.muxihuayi.cn

TS:   get name(): string { return this._name; }
来源：http://ju.9csxet.cn

Java: public String getName() { return name; }
来源：http://mh.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ar.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://yk.newstarts.cn

C#:   public string Name { get; set; }
来源：http://aj.colortex.cn

[G12] 对象转字符串
来源：http://ro.szxytkj.cn

Py:   def __str__(self): return self.name
来源：http://xq.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://mm.nicolike.cn

JS:   toString() { return this.name; }
来源：http://pk.bookmarksfly.cn

TS:   toString(): string { return this.name; }
来源：http://nd.yuntaijiaju.cn

Java: @Override public String toString() { return name; }
来源：http://gg.huixinmuqiang.cn

Go:   func (u User) String() string { return u.Name }
来源：http://iw.shtwfgs.cn

Ruby: def to_s; @name; end
来源：http://bh.wgjwhj.cn

C#:   public override string ToString() => Name;
来源：http://xt.shxzskj.cn

[G13] 判断对象类型
来源：http://ag.521024.cn

Py:   isinstance(u, User)
来源：http://nj.shtwfgs.cn

PHP:  $u instanceof User
来源：http://ga.nszjky.cn

JS:   u instanceof User
来源：http://ha.9csxet.cn

TS:   u instanceof User
来源：http://tn.shtwfgs.cn

Java: u instanceof User
来源：http://zm.shxzukj.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://bf.huanxung.cn

Ruby: u.is_a?(User)
来源：http://xr.huixinmuqiang.cn

C#:   u is User
来源：http://rm.szxytkj.cn

[G14] 数据类 / record
来源：http://hq.hnjuh.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://nm.9csxet.cn

PHP:  // 用 readonly 属性模拟
来源：http://fq.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://pe.bookmarksfly.cn


<!-- 参考信息 -->