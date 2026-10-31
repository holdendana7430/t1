代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://ir.szsharing.cn

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hy.panjiajie.cn

[E16] 数字千分位
来源：http://uk.jctech888.com.cn

Py:   f"{1234567:,}"
来源：http://pa.haigaiapp.cn

PHP:  number_format(1234567);
来源：http://al.haigaiapp.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://il.szsharing.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://qn.muxihuayi.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://io.haigaiapp.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://rq.lnxyls.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://we.bjjhwx.cn

C#:   1234567.ToString("N0")
来源：http://iy.9csxet.cn

[E17] 首字母大写
来源：http://tv.muxihuayi.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://pc.muxihuayi.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://ie.gzmigu.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://xj.szxytkj.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://qa.yuexingan06.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://zi.huanxung.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://ru.huixinmuqiang.cn

Ruby: s.capitalize
来源：http://xn.huixiangedu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wf.bookmarksfly.cn

[E18] 模板占位符替换
来源：http://jh.asd995.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://fw.shtwfgs.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://bs.yuntaijiaju.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://av.szxytkj.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://hs.panjiajie.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://sz.shxzukj.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zd.asd995.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nl.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://pw.asd995.cn

[E19] 多行文本按行拆分
来源：http://nb.bjjhwx.cn

Py:   s.splitlines()
来源：http://gy.muxihuayi.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://md.nicolike.cn

JS:   s.split(/\r?\n/)
来源：http://wt.hahajie.cn

TS:   s.split(/\r?\n/)
来源：http://hk.haigaiapp.cn

Java: s.lines().toList()
来源：http://eg.haigaiapp.cn

Go:   strings.Split(s, "\n")
来源：http://zl.haigaiapp.cn

Ruby: s.lines
来源：http://sm.shxzukj.cn

C#:   s.Split('\n')
来源：http://ro.szxytkj.cn

[E20] 判断字符串是否为空
来源：http://iz.szsharing.cn

Py:   if not s:
来源：http://aq.szsharing.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hw.shxzskj.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://ph.shxzukj.cn

TS:   if (s === "") {}
来源：http://yx.szsharing.cn

Java: if (s.isEmpty()) {}
来源：http://uz.huixiangedu.cn

Go:   if s == "" {}
来源：http://qi.haigaiapp.cn

Ruby: if s.empty?
来源：http://cw.huixiangedu.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://fq.9csxet.cn

[E21] 超长截断加省略号
来源：http://hz.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://np.szxytkj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://bw.huixinmuqiang.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zz.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ng.chemitech.net.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://po.newstarts.cn

Go:   // 按 rune 判断长度后截断
来源：http://td.jctech888.com.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://gv.bjjhwx.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://gh.521024.cn

[E22] 字节长度与字符长度
来源：http://qm.huixiangedu.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://if.haigaiapp.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://gf.hahajie.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://rj.asd995.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yi.huanxung.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://pt.shxzskj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://li.haigaiapp.cn

Ruby: s.bytesize;  s.length
来源：http://sg.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pg.bookmarksfly.cn

================================================================================
来源：http://dp.huixinmuqiang.cn

F. 文件与目录
来源：http://yk.lnxyls.cn

================================================================================
来源：http://gb.shxzskj.cn

[F01] 读取整个文件
来源：http://mw.huanxung.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://am.szsharing.cn

PHP:  file_get_contents("a.txt");
来源：http://ja.shxzukj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://nh.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://si.huixiangedu.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ed.yuexingan06.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ji.szsharing.cn

Ruby: File.read("a.txt")
来源：http://ng.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://du.lnxyls.cn

[F02] 逐行读取文件
来源：http://rd.yuexingan06.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tw.szxytkj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pm.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ob.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yh.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ld.colortex.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qz.521024.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bb.hahajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://rb.szsharing.cn

[F03] 写入文件（覆盖）
来源：http://ox.shxzukj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uw.chemitech.net.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://sg.panjiajie.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sx.huanxung.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tc.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://cp.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mc.huixinmuqiang.cn

Ruby: File.write("a.txt", "hi")
来源：http://hs.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qx.panjiajie.cn

[F04] 追加写入文件
来源：http://dv.panjiajie.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://jy.colortex.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ne.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://cv.lnxyls.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vl.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ae.muxihuayi.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fv.521024.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dq.asd995.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://tp.yuexingan06.cn

[F05] 判断文件或目录是否存在
来源：http://pp.gzmigu.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://sb.nicolike.cn

PHP:  file_exists("a.txt");
来源：http://ct.521024.cn

JS:   fs.existsSync("a.txt")
来源：http://ia.colortex.cn

TS:   fs.existsSync("a.txt")
来源：http://fq.jianghongdianzi.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://gb.huanxung.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ow.lnxyls.cn

Ruby: File.exist?("a.txt")
来源：http://bg.colortex.cn

C#:   File.Exists("a.txt")
来源：http://nf.jctech888.com.cn

[F06] 删除文件
来源：http://ic.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://dk.jctech888.com.cn

PHP:  unlink("a.txt");
来源：http://fx.muxihuayi.cn

JS:   fs.unlinkSync("a.txt")
来源：http://sv.shxzukj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ca.asd995.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ry.9csxet.cn

Go:   os.Remove("a.txt")
来源：http://fg.shxzukj.cn

Ruby: File.delete("a.txt")
来源：http://wi.bjjhwx.cn

C#:   File.Delete("a.txt");
来源：http://ty.yuntaijiaju.cn

[F07] 创建目录（含多级）
来源：http://wa.newstarts.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://fj.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lf.szxytkj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://yx.shxzskj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ft.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mr.colortex.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://za.nszjky.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://dg.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xg.huanxung.cn

[F08] 遍历目录
来源：http://fv.wgjwhj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jk.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://oy.521024.cn

JS:   fs.readdirSync("dir")
来源：http://th.haigaiapp.cn

TS:   fs.readdirSync("dir")
来源：http://ec.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://lw.jianghongdianzi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://mr.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://rb.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://kz.nicolike.cn

[F09] 获取文件大小
来源：http://mn.panjiajie.cn

Py:   os.path.getsize("a.txt")
来源：http://wd.colortex.cn

PHP:  filesize("a.txt");
来源：http://ml.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://bc.asd995.cn

TS:   fs.statSync("a.txt").size
来源：http://vy.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://gh.lnxyls.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://kg.huanxung.cn

Ruby: File.size("a.txt")
来源：http://qo.nszjky.cn

C#:   new FileInfo("a.txt").Length
来源：http://ny.asd995.cn

[F10] 取文件扩展名 / 文件名
来源：http://zp.shxzukj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://oa.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ly.szxytkj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ui.jctech888.com.cn

TS:   path.extname("a.txt")
来源：http://or.9csxet.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://xn.huanxung.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ug.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ch.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pl.szxytkj.cn

[F11] 复制与移动文件
来源：http://xg.wgjwhj.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://he.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ip.gzmigu.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://fc.nicolike.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gm.gzmigu.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://lq.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://vc.colortex.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ik.shxzskj.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://il.hnjuh.cn

[F12] CSV 读写
来源：http://or.hahajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://xm.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kw.hahajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bb.lnxyls.cn

TS:   // 同上
来源：http://cn.hnjuh.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hp.gzmigu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pa.hnjuh.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://xi.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ds.bookmarksfly.cn

================================================================================
来源：http://gp.jctech888.com.cn

G. 面向对象
来源：http://fk.colortex.cn

================================================================================
来源：http://fg.nszjky.cn

[G01] 定义类
来源：http://at.wgjwhj.cn

Py:   class User: pass
来源：http://gl.chemitech.net.cn

PHP:  class User {}
来源：http://uo.yuexingan06.cn

JS:   class User {}
来源：http://yw.shtwfgs.cn

TS:   class User { name: string = ""; }
来源：http://ho.nszjky.cn

Java: class User {}
来源：http://bw.huixiangedu.cn

Go:   type User struct { Name string }
来源：http://uz.shxzskj.cn

Ruby: class User; end
来源：http://ml.shxzskj.cn

C#:   class User {}
来源：http://mw.colortex.cn

[G02] 构造函数
来源：http://vd.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://db.hnjuh.cn

PHP:  public function __construct(public string $name) {}
来源：http://sb.nszjky.cn

JS:   constructor(name) { this.name = name; }
来源：http://ds.lnxyls.cn

TS:   constructor(public name: string) {}
来源：http://kc.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://da.panjiajie.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ay.wgjwhj.cn

Ruby: def initialize(name); @name = name; end
来源：http://us.colortex.cn

C#:   public User(string name) { Name = name; }
来源：http://rp.wgjwhj.cn

[G03] 实例属性
来源：http://oi.huixinmuqiang.cn

Py:   self.name = "x"
来源：http://rl.szsharing.cn

PHP:  public string $name = "x";
来源：http://tn.bookmarksfly.cn

JS:   this.name = "x";
来源：http://gq.newstarts.cn

TS:   name: string = "x";
来源：http://gs.szxytkj.cn

Java: private String name;
来源：http://bh.521024.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://ye.shtwfgs.cn

Ruby: @name = "x"
来源：http://uy.jianghongdianzi.cn

C#:   public string Name { get; set; } = "x";
来源：http://qg.bookmarksfly.cn

[G04] 定义方法
来源：http://wo.bjjhwx.cn

Py:   def greet(self): return self.name
来源：http://le.haigaiapp.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://in.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://jc.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://bh.colortex.cn

Java: String greet() { return name; }
来源：http://eb.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://jq.yuntaijiaju.cn

Ruby: def greet; @name; end
来源：http://ik.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://xz.yuexingan06.cn

[G05] 继承
来源：http://sy.jianghongdianzi.cn

Py:   class Admin(User): pass
来源：http://cp.muxihuayi.cn

PHP:  class Admin extends User {}
来源：http://yi.nicolike.cn

JS:   class Admin extends User {}
来源：http://jb.hnjuh.cn

TS:   class Admin extends User {}
来源：http://jn.hahajie.cn

Java: class Admin extends User {}
来源：http://zs.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ms.newstarts.cn

Ruby: class Admin < User; end
来源：http://zj.bjjhwx.cn

C#:   class Admin : User {}
来源：http://ay.shxzskj.cn

[G06] 重写方法
来源：http://ok.jianghongdianzi.cn

Py:   def greet(self): return "admin"
来源：http://tt.yuntaijiaju.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://mk.chemitech.net.cn

JS:   greet() { return "admin"; }
来源：http://lo.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://bp.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://of.chemitech.net.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://uw.asd995.cn

Ruby: def greet; "admin"; end
来源：http://ln.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://rm.shxzukj.cn

[G07] 调用父类方法
来源：http://ae.nicolike.cn

Py:   super().greet()
来源：http://zt.jianghongdianzi.cn

PHP:  parent::greet();
来源：http://fk.jianghongdianzi.cn

JS:   super.greet();
来源：http://mr.shxzskj.cn

TS:   super.greet();
来源：http://mv.gzmigu.cn

Java: super.greet();
来源：http://xm.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mo.colortex.cn

Ruby: super
来源：http://dn.newstarts.cn

C#:   base.Greet();
来源：http://yy.nicolike.cn

[G08] 静态方法与属性
来源：http://uw.shtwfgs.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mb.gzmigu.cn

PHP:  public static function f() {}
来源：http://zf.lnxyls.cn

JS:   static f() {}
来源：http://gj.yuntaijiaju.cn

TS:   static f(): void {}
来源：http://km.jctech888.com.cn

Java: static void f() {}
来源：http://gt.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ce.huixinmuqiang.cn

Ruby: def self.f; end
来源：http://di.jctech888.com.cn

C#:   public static void F() {}
来源：http://sn.yuexingan06.cn

[G09] 接口 / 抽象类
来源：http://fr.hahajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://uk.muxihuayi.cn

PHP:  interface Shape { public function area(): float; }
来源：http://pf.shxzukj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://tb.shxzukj.cn

TS:   interface Shape { area(): number; }
来源：http://em.huixinmuqiang.cn

Java: interface Shape { double area(); }
来源：http://gp.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://qe.chemitech.net.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://to.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://ox.haigaiapp.cn

[G10] 访问控制
来源：http://ps.9csxet.cn

Py:   约定 _protected / __private（不强制）
来源：http://do.asd995.cn

PHP:  public / protected / private
来源：http://tx.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://os.muxihuayi.cn

TS:   public / protected / private
来源：http://ea.szsharing.cn

Java: public / protected / private / 默认包级
来源：http://wq.shtwfgs.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://qu.newstarts.cn

Ruby: public / protected / private
来源：http://ey.jctech888.com.cn

C#:   public / protected / private / internal
来源：http://ix.muxihuayi.cn

[G11] getter / setter
来源：http://fq.haigaiapp.cn

Py:   @property 与 @x.setter
来源：http://fb.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://et.huixiangedu.cn

JS:   get name() { return this._name; }
来源：http://ay.nicolike.cn

TS:   get name(): string { return this._name; }
来源：http://no.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://tv.wgjwhj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ne.szxytkj.cn

Ruby: attr_accessor :name
来源：http://et.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://jt.huanxung.cn

[G12] 对象转字符串
来源：http://pt.huanxung.cn

Py:   def __str__(self): return self.name
来源：http://ck.haigaiapp.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://ia.nszjky.cn

JS:   toString() { return this.name; }
来源：http://ee.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://yt.jctech888.com.cn

Java: @Override public String toString() { return name; }
来源：http://lv.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kj.521024.cn

Ruby: def to_s; @name; end
来源：http://pn.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://of.asd995.cn

[G13] 判断对象类型
来源：http://pd.521024.cn

Py:   isinstance(u, User)
来源：http://us.hahajie.cn

PHP:  $u instanceof User
来源：http://ag.newstarts.cn

JS:   u instanceof User
来源：http://pk.chemitech.net.cn

TS:   u instanceof User
来源：http://ya.panjiajie.cn

Java: u instanceof User
来源：http://dl.shtwfgs.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ho.huanxung.cn

Ruby: u.is_a?(User)
来源：http://zl.jianghongdianzi.cn

C#:   u is User
来源：http://tg.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://qy.asd995.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://to.nszjky.cn

PHP:  // 用 readonly 属性模拟
来源：http://sr.bookmarksfly.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wy.huixiangedu.cn


<!-- 参考信息 -->