代发 wailian999

PHP:  number_format(1234567);
来源：http://zi.chemitech.net.cn

JS:   (1234567).toLocaleString("en-US")
来源：http://fl.huanxung.cn

TS:   (1234567).toLocaleString("en-US")
来源：http://kg.nszjky.cn

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mr.newstarts.cn

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://ll.gzmigu.cn

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://xv.jctech888.com.cn

C#:   1234567.ToString("N0")
来源：http://np.newstarts.cn

[E17] 首字母大写
来源：http://ic.szxytkj.cn

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://dc.panjiajie.cn

PHP:  ucfirst($s);  ucwords($s);
来源：http://rn.huanxung.cn

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ui.huixiangedu.cn

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://ci.panjiajie.cn

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://tf.chemitech.net.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://sa.panjiajie.cn

Ruby: s.capitalize
来源：http://es.huanxung.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://em.szsharing.cn

[E18] 模板占位符替换
来源：http://od.yuntaijiaju.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://cy.wgjwhj.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://il.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://ul.chemitech.net.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://bf.hnjuh.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://xu.bookmarksfly.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://dh.muxihuayi.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://nm.9csxet.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://ov.szsharing.cn

[E19] 多行文本按行拆分
来源：http://ot.yuntaijiaju.cn

Py:   s.splitlines()
来源：http://le.haigaiapp.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://ui.bookmarksfly.cn

JS:   s.split(/\r?\n/)
来源：http://ia.bookmarksfly.cn

TS:   s.split(/\r?\n/)
来源：http://fb.yuexingan06.cn

Java: s.lines().toList()
来源：http://nd.colortex.cn

Go:   strings.Split(s, "\n")
来源：http://yk.nicolike.cn

Ruby: s.lines
来源：http://qk.9csxet.cn

C#:   s.Split('\n')
来源：http://oa.panjiajie.cn

[E20] 判断字符串是否为空
来源：http://eu.szxytkj.cn

Py:   if not s:
来源：http://yd.huixinmuqiang.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://uu.haigaiapp.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://dm.wgjwhj.cn

TS:   if (s === "") {}
来源：http://mt.jianghongdianzi.cn

Java: if (s.isEmpty()) {}
来源：http://ec.haigaiapp.cn

Go:   if s == "" {}
来源：http://mv.shtwfgs.cn

Ruby: if s.empty?
来源：http://mx.yuexingan06.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://st.521024.cn

[E21] 超长截断加省略号
来源：http://ha.huixiangedu.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://eg.521024.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://pt.haigaiapp.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ej.yuntaijiaju.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wh.yuexingan06.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://nm.hnjuh.cn

Go:   // 按 rune 判断长度后截断
来源：http://nn.huixiangedu.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mc.bookmarksfly.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://do.jianghongdianzi.cn

[E22] 字节长度与字符长度
来源：http://qp.shxzukj.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://uz.newstarts.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://uq.nicolike.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ao.szxytkj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tf.nszjky.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://nc.szxytkj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://vi.bookmarksfly.cn

Ruby: s.bytesize;  s.length
来源：http://fa.nszjky.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://pj.huanxung.cn

================================================================================
来源：http://gx.huixinmuqiang.cn

F. 文件与目录
来源：http://oz.haigaiapp.cn

================================================================================
来源：http://bn.nicolike.cn

[F01] 读取整个文件
来源：http://mg.9csxet.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://un.shxzskj.cn

PHP:  file_get_contents("a.txt");
来源：http://so.nszjky.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mr.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://jb.szxytkj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://im.jctech888.com.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ab.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://sm.521024.cn

C#:   File.ReadAllText("a.txt");
来源：http://qc.newstarts.cn

[F02] 逐行读取文件
来源：http://rp.shtwfgs.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://jh.bookmarksfly.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://jd.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://xk.newstarts.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://od.yuexingan06.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://fj.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://vj.jctech888.com.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mc.jianghongdianzi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://kd.asd995.cn

[F03] 写入文件（覆盖）
来源：http://qh.shxzskj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pl.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hk.asd995.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ll.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://vc.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mq.jctech888.com.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gm.muxihuayi.cn

Ruby: File.write("a.txt", "hi")
来源：http://ch.hahajie.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://oj.asd995.cn

[F04] 追加写入文件
来源：http://yp.shxzukj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://fi.jianghongdianzi.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rk.shxzskj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://pr.huixiangedu.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://la.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://nc.hahajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xt.jctech888.com.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://as.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ch.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://uy.shtwfgs.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fj.haigaiapp.cn

PHP:  file_exists("a.txt");
来源：http://lj.gzmigu.cn

JS:   fs.existsSync("a.txt")
来源：http://us.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://ab.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://iw.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://qd.colortex.cn

Ruby: File.exist?("a.txt")
来源：http://jw.hnjuh.cn

C#:   File.Exists("a.txt")
来源：http://dw.jctech888.com.cn

[F06] 删除文件
来源：http://wm.nicolike.cn

Py:   os.remove("a.txt")
来源：http://oq.huanxung.cn

PHP:  unlink("a.txt");
来源：http://eg.asd995.cn

JS:   fs.unlinkSync("a.txt")
来源：http://vs.bookmarksfly.cn

TS:   fs.unlinkSync("a.txt")
来源：http://sp.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://vb.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://mq.huixinmuqiang.cn

Ruby: File.delete("a.txt")
来源：http://bz.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://xf.huixiangedu.cn

[F07] 创建目录（含多级）
来源：http://jx.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://zy.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://sq.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://lh.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://pa.newstarts.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://yt.huixiangedu.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://sh.shxzukj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ih.hahajie.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://sy.shxzukj.cn

[F08] 遍历目录
来源：http://pi.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://tv.hnjuh.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://cz.lnxyls.cn

JS:   fs.readdirSync("dir")
来源：http://wa.colortex.cn

TS:   fs.readdirSync("dir")
来源：http://cw.jctech888.com.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fn.shtwfgs.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://lt.newstarts.cn

Ruby: Dir.children("dir")
来源：http://ec.yuexingan06.cn

C#:   Directory.GetFiles("dir")
来源：http://zh.huixinmuqiang.cn

[F09] 获取文件大小
来源：http://hs.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://zo.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://vz.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://zw.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://hc.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ie.521024.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yd.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://fq.huanxung.cn

C#:   new FileInfo("a.txt").Length
来源：http://ii.hnjuh.cn

[F10] 取文件扩展名 / 文件名
来源：http://uu.shxzskj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://zn.haigaiapp.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rb.nicolike.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ez.haigaiapp.cn

TS:   path.extname("a.txt")
来源：http://ld.521024.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://qx.jctech888.com.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://xn.gzmigu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://eo.szxytkj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wg.gzmigu.cn

[F11] 复制与移动文件
来源：http://aj.newstarts.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wu.shtwfgs.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cs.muxihuayi.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vg.jianghongdianzi.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nq.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nj.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nc.lnxyls.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hv.huanxung.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://bb.nicolike.cn

[F12] CSV 读写
来源：http://xo.shtwfgs.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://nv.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://sf.panjiajie.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bi.szxytkj.cn

TS:   // 同上
来源：http://ac.szsharing.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://yu.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://py.jctech888.com.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://up.nicolike.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://dw.newstarts.cn

================================================================================
来源：http://nn.shxzukj.cn

G. 面向对象
来源：http://zt.bookmarksfly.cn

================================================================================
来源：http://pl.nszjky.cn

[G01] 定义类
来源：http://xu.colortex.cn

Py:   class User: pass
来源：http://tb.9csxet.cn

PHP:  class User {}
来源：http://la.jctech888.com.cn

JS:   class User {}
来源：http://cg.asd995.cn

TS:   class User { name: string = ""; }
来源：http://fy.panjiajie.cn

Java: class User {}
来源：http://yd.bookmarksfly.cn

Go:   type User struct { Name string }
来源：http://nc.yuexingan06.cn

Ruby: class User; end
来源：http://br.huanxung.cn

C#:   class User {}
来源：http://ar.shtwfgs.cn

[G02] 构造函数
来源：http://nb.bookmarksfly.cn

Py:   def __init__(self, name): self.name = name
来源：http://af.haigaiapp.cn

PHP:  public function __construct(public string $name) {}
来源：http://ln.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://qt.gzmigu.cn

TS:   constructor(public name: string) {}
来源：http://hw.huixiangedu.cn

Java: User(String name) { this.name = name; }
来源：http://as.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ew.asd995.cn

Ruby: def initialize(name); @name = name; end
来源：http://xv.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://kz.shxzukj.cn

[G03] 实例属性
来源：http://mb.yuexingan06.cn

Py:   self.name = "x"
来源：http://pj.wgjwhj.cn

PHP:  public string $name = "x";
来源：http://xj.lnxyls.cn

JS:   this.name = "x";
来源：http://kn.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://lz.asd995.cn

Java: private String name;
来源：http://wh.shxzukj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://lb.muxihuayi.cn

Ruby: @name = "x"
来源：http://xn.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://ds.asd995.cn

[G04] 定义方法
来源：http://tm.szsharing.cn

Py:   def greet(self): return self.name
来源：http://zl.muxihuayi.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://uc.haigaiapp.cn

JS:   greet() { return this.name; }
来源：http://ym.lnxyls.cn

TS:   greet(): string { return this.name; }
来源：http://re.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://gn.jctech888.com.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://fb.newstarts.cn

Ruby: def greet; @name; end
来源：http://eb.nicolike.cn

C#:   public string Greet() => Name;
来源：http://lw.panjiajie.cn

[G05] 继承
来源：http://gb.muxihuayi.cn

Py:   class Admin(User): pass
来源：http://wc.shxzukj.cn

PHP:  class Admin extends User {}
来源：http://jr.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://la.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://ym.nszjky.cn

Java: class Admin extends User {}
来源：http://op.hahajie.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ki.huixiangedu.cn

Ruby: class Admin < User; end
来源：http://it.9csxet.cn

C#:   class Admin : User {}
来源：http://oi.szxytkj.cn

[G06] 重写方法
来源：http://mr.hnjuh.cn

Py:   def greet(self): return "admin"
来源：http://sk.bjjhwx.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://sz.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://mj.huixinmuqiang.cn

TS:   greet(): string { return "admin"; }
来源：http://ty.lnxyls.cn

Java: @Override String greet() { return "admin"; }
来源：http://wb.bookmarksfly.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://xc.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://mw.jianghongdianzi.cn

C#:   public override string Greet() => "admin";
来源：http://fa.hahajie.cn

[G07] 调用父类方法
来源：http://rr.szxytkj.cn

Py:   super().greet()
来源：http://wp.huixiangedu.cn

PHP:  parent::greet();
来源：http://xi.newstarts.cn

JS:   super.greet();
来源：http://mo.chemitech.net.cn

TS:   super.greet();
来源：http://ow.521024.cn

Java: super.greet();
来源：http://wp.bjjhwx.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gk.colortex.cn

Ruby: super
来源：http://ub.shxzskj.cn

C#:   base.Greet();
来源：http://fg.colortex.cn

[G08] 静态方法与属性
来源：http://nr.nicolike.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://kx.bjjhwx.cn

PHP:  public static function f() {}
来源：http://wy.huixiangedu.cn

JS:   static f() {}
来源：http://il.gzmigu.cn

TS:   static f(): void {}
来源：http://pp.521024.cn

Java: static void f() {}
来源：http://jf.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ea.9csxet.cn

Ruby: def self.f; end
来源：http://uv.huixinmuqiang.cn

C#:   public static void F() {}
来源：http://ms.jianghongdianzi.cn

[G09] 接口 / 抽象类
来源：http://qo.yuexingan06.cn

Py:   from abc import ABC, abstractmethod
来源：http://ic.hnjuh.cn

PHP:  interface Shape { public function area(): float; }
来源：http://do.hnjuh.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xi.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://vu.yuntaijiaju.cn

Java: interface Shape { double area(); }
来源：http://sx.huanxung.cn

Go:   type Shape interface { Area() float64 }
来源：http://wu.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://nx.bookmarksfly.cn

C#:   interface IShape { double Area(); }
来源：http://ra.bjjhwx.cn

[G10] 访问控制
来源：http://xt.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://hp.nszjky.cn

PHP:  public / protected / private
来源：http://gm.9csxet.cn

JS:   #private 字段；其余公开
来源：http://jn.hahajie.cn

TS:   public / protected / private
来源：http://ep.nicolike.cn

Java: public / protected / private / 默认包级
来源：http://tk.gzmigu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yh.shtwfgs.cn

Ruby: public / protected / private
来源：http://ws.shxzukj.cn

C#:   public / protected / private / internal
来源：http://ix.chemitech.net.cn

[G11] getter / setter
来源：http://bx.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://au.szsharing.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://je.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://cj.yuexingan06.cn

TS:   get name(): string { return this._name; }
来源：http://bq.lnxyls.cn

Java: public String getName() { return name; }
来源：http://fq.shxzskj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://iu.shxzukj.cn

Ruby: attr_accessor :name
来源：http://tm.chemitech.net.cn

C#:   public string Name { get; set; }
来源：http://ki.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://xd.shxzskj.cn

Py:   def __str__(self): return self.name
来源：http://sp.panjiajie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rp.yuntaijiaju.cn

JS:   toString() { return this.name; }
来源：http://al.szxytkj.cn

TS:   toString(): string { return this.name; }
来源：http://mk.wgjwhj.cn

Java: @Override public String toString() { return name; }
来源：http://gs.muxihuayi.cn

Go:   func (u User) String() string { return u.Name }
来源：http://xd.lnxyls.cn

Ruby: def to_s; @name; end
来源：http://lj.panjiajie.cn

C#:   public override string ToString() => Name;
来源：http://bh.muxihuayi.cn

[G13] 判断对象类型
来源：http://es.panjiajie.cn

Py:   isinstance(u, User)
来源：http://kj.jianghongdianzi.cn

PHP:  $u instanceof User
来源：http://oy.asd995.cn

JS:   u instanceof User
来源：http://kt.chemitech.net.cn

TS:   u instanceof User
来源：http://nr.huanxung.cn

Java: u instanceof User
来源：http://zv.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://kn.asd995.cn

Ruby: u.is_a?(User)
来源：http://ll.shxzukj.cn

C#:   u is User
来源：http://il.bookmarksfly.cn

[G14] 数据类 / record
来源：http://vk.szsharing.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://fr.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://gi.shxzskj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ln.jianghongdianzi.cn

TS:   type User = { name: string; age: number };
来源：http://iy.bjjhwx.cn

Java: record User(String name, int age) {}
来源：http://jj.jianghongdianzi.cn

Go:   type User struct { Name string; Age int }
来源：http://xs.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://dw.szsharing.cn


<!-- 参考信息 -->