代发 wailian999

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://qd.haigaiapp.cn

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://le.muxihuayi.cn

Ruby: s.capitalize
来源：http://ch.gzmigu.cn

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://zp.muxihuayi.cn

[E18] 模板占位符替换
来源：http://es.haigaiapp.cn

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://li.huanxung.cn

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://cf.huanxung.cn

JS:   tpl.replaceAll("{name}", name)
来源：http://zh.bjjhwx.cn

TS:   tpl.replaceAll("{name}", name)
来源：http://rt.bjjhwx.cn

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://md.bjjhwx.cn

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://zb.huixiangedu.cn

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://zs.huixiangedu.cn

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wv.shtwfgs.cn

[E19] 多行文本按行拆分
来源：http://yb.shtwfgs.cn

Py:   s.splitlines()
来源：http://qu.huanxung.cn

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://sw.521024.cn

JS:   s.split(/\r?\n/)
来源：http://iq.shxzukj.cn

TS:   s.split(/\r?\n/)
来源：http://ua.521024.cn

Java: s.lines().toList()
来源：http://dq.shxzskj.cn

Go:   strings.Split(s, "\n")
来源：http://ox.huanxung.cn

Ruby: s.lines
来源：http://qx.nszjky.cn

C#:   s.Split('\n')
来源：http://ij.hnjuh.cn

[E20] 判断字符串是否为空
来源：http://qo.panjiajie.cn

Py:   if not s:
来源：http://tq.bjjhwx.cn

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://ml.yuexingan06.cn

JS:   if (s === "") {} 或 if (!s) {}
来源：http://fw.shxzskj.cn

TS:   if (s === "") {}
来源：http://st.colortex.cn

Java: if (s.isEmpty()) {}
来源：http://sm.shxzskj.cn

Go:   if s == "" {}
来源：http://kz.gzmigu.cn

Ruby: if s.empty?
来源：http://rr.521024.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://ok.shxzskj.cn

[E21] 超长截断加省略号
来源：http://ep.asd995.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://nl.shxzskj.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://tc.panjiajie.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://rk.jianghongdianzi.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://zg.huixiangedu.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://oe.wgjwhj.cn

Go:   // 按 rune 判断长度后截断
来源：http://oi.chemitech.net.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://pj.huanxung.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://cm.hnjuh.cn

[E22] 字节长度与字符长度
来源：http://cp.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ls.asd995.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://sn.bjjhwx.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hw.hahajie.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xf.huixiangedu.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://eg.huixiangedu.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://yr.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://vt.huixiangedu.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://un.szsharing.cn

================================================================================
来源：http://xg.521024.cn

F. 文件与目录
来源：http://gg.lnxyls.cn

================================================================================
来源：http://yz.hahajie.cn

[F01] 读取整个文件
来源：http://yb.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ns.yuexingan06.cn

PHP:  file_get_contents("a.txt");
来源：http://fw.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zc.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://pu.521024.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lo.newstarts.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ee.nicolike.cn

Ruby: File.read("a.txt")
来源：http://ul.huixiangedu.cn

C#:   File.ReadAllText("a.txt");
来源：http://fk.nszjky.cn

[F02] 逐行读取文件
来源：http://ye.colortex.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fp.asd995.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://yn.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lw.jianghongdianzi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cs.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://at.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://qw.yuntaijiaju.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zh.bjjhwx.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ih.lnxyls.cn

[F03] 写入文件（覆盖）
来源：http://ft.hnjuh.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://we.bookmarksfly.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://da.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://by.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ag.shtwfgs.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://aq.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://vf.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://nq.shtwfgs.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ur.bookmarksfly.cn

[F04] 追加写入文件
来源：http://rf.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hr.panjiajie.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qs.yuexingan06.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qv.yuntaijiaju.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://vw.huanxung.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jx.yuexingan06.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wc.nicolike.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://xd.shxzskj.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://yl.huanxung.cn

[F05] 判断文件或目录是否存在
来源：http://wo.colortex.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://pn.szsharing.cn

PHP:  file_exists("a.txt");
来源：http://tk.muxihuayi.cn

JS:   fs.existsSync("a.txt")
来源：http://ht.shtwfgs.cn

TS:   fs.existsSync("a.txt")
来源：http://dj.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://pq.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://to.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://ii.huanxung.cn

C#:   File.Exists("a.txt")
来源：http://yy.jctech888.com.cn

[F06] 删除文件
来源：http://sd.colortex.cn

Py:   os.remove("a.txt")
来源：http://se.bookmarksfly.cn

PHP:  unlink("a.txt");
来源：http://jm.jctech888.com.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ol.hahajie.cn

TS:   fs.unlinkSync("a.txt")
来源：http://dm.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://zd.colortex.cn

Go:   os.Remove("a.txt")
来源：http://lp.shtwfgs.cn

Ruby: File.delete("a.txt")
来源：http://hf.huixinmuqiang.cn

C#:   File.Delete("a.txt");
来源：http://ye.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://lj.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ob.haigaiapp.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://eb.nszjky.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://cz.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vk.9csxet.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fr.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://pn.szxytkj.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zr.szxytkj.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://pb.szxytkj.cn

[F08] 遍历目录
来源：http://ue.huixinmuqiang.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://jo.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://xw.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://kg.jianghongdianzi.cn

TS:   fs.readdirSync("dir")
来源：http://lc.colortex.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mw.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fe.jctech888.com.cn

Ruby: Dir.children("dir")
来源：http://rb.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://se.yuntaijiaju.cn

[F09] 获取文件大小
来源：http://nf.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://cx.yuexingan06.cn

PHP:  filesize("a.txt");
来源：http://su.shxzskj.cn

JS:   fs.statSync("a.txt").size
来源：http://ys.huixiangedu.cn

TS:   fs.statSync("a.txt").size
来源：http://qc.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://om.huixinmuqiang.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://aq.hahajie.cn

Ruby: File.size("a.txt")
来源：http://ml.yuntaijiaju.cn

C#:   new FileInfo("a.txt").Length
来源：http://ga.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://cn.nicolike.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://li.chemitech.net.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://np.hnjuh.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://yu.bookmarksfly.cn

TS:   path.extname("a.txt")
来源：http://ad.haigaiapp.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ya.9csxet.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mw.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://sz.shxzskj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hk.nszjky.cn

[F11] 复制与移动文件
来源：http://zr.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://dx.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://dr.9csxet.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ek.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://dh.nicolike.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://oj.nicolike.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://bz.521024.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://gc.yuntaijiaju.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://cy.newstarts.cn

[F12] CSV 读写
来源：http://et.huixiangedu.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://al.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ol.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ha.muxihuayi.cn

TS:   // 同上
来源：http://ff.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ld.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://yw.huixinmuqiang.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://eg.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://wa.shxzskj.cn

================================================================================
来源：http://ub.hnjuh.cn

G. 面向对象
来源：http://de.huixinmuqiang.cn

================================================================================
来源：http://dm.jianghongdianzi.cn

[G01] 定义类
来源：http://et.hnjuh.cn

Py:   class User: pass
来源：http://pn.huixiangedu.cn

PHP:  class User {}
来源：http://tf.hnjuh.cn

JS:   class User {}
来源：http://bt.hahajie.cn

TS:   class User { name: string = ""; }
来源：http://qh.muxihuayi.cn

Java: class User {}
来源：http://is.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://qi.bookmarksfly.cn

Ruby: class User; end
来源：http://ys.haigaiapp.cn

C#:   class User {}
来源：http://iw.jianghongdianzi.cn

[G02] 构造函数
来源：http://us.haigaiapp.cn

Py:   def __init__(self, name): self.name = name
来源：http://vs.newstarts.cn

PHP:  public function __construct(public string $name) {}
来源：http://yl.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://bn.shtwfgs.cn

TS:   constructor(public name: string) {}
来源：http://pr.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://rd.521024.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://iy.yuexingan06.cn

Ruby: def initialize(name); @name = name; end
来源：http://te.huanxung.cn

C#:   public User(string name) { Name = name; }
来源：http://fc.huanxung.cn

[G03] 实例属性
来源：http://lg.9csxet.cn

Py:   self.name = "x"
来源：http://ey.nszjky.cn

PHP:  public string $name = "x";
来源：http://by.panjiajie.cn

JS:   this.name = "x";
来源：http://kx.nszjky.cn

TS:   name: string = "x";
来源：http://zf.hahajie.cn

Java: private String name;
来源：http://fl.hnjuh.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://af.yuexingan06.cn

Ruby: @name = "x"
来源：http://pv.yuexingan06.cn

C#:   public string Name { get; set; } = "x";
来源：http://sx.nszjky.cn

[G04] 定义方法
来源：http://nm.nszjky.cn

Py:   def greet(self): return self.name
来源：http://uk.huixinmuqiang.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ci.asd995.cn

JS:   greet() { return this.name; }
来源：http://rm.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://xm.chemitech.net.cn

Java: String greet() { return name; }
来源：http://nd.huixinmuqiang.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://nz.shtwfgs.cn

Ruby: def greet; @name; end
来源：http://bg.muxihuayi.cn

C#:   public string Greet() => Name;
来源：http://rz.chemitech.net.cn

[G05] 继承
来源：http://go.wgjwhj.cn

Py:   class Admin(User): pass
来源：http://pa.chemitech.net.cn

PHP:  class Admin extends User {}
来源：http://bv.colortex.cn

JS:   class Admin extends User {}
来源：http://eo.lnxyls.cn

TS:   class Admin extends User {}
来源：http://kq.bjjhwx.cn

Java: class Admin extends User {}
来源：http://da.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://fh.colortex.cn

Ruby: class Admin < User; end
来源：http://zm.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://mf.panjiajie.cn

[G06] 重写方法
来源：http://yg.shxzukj.cn

Py:   def greet(self): return "admin"
来源：http://xd.chemitech.net.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://yi.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://ea.wgjwhj.cn

TS:   greet(): string { return "admin"; }
来源：http://wt.hahajie.cn

Java: @Override String greet() { return "admin"; }
来源：http://qt.huixiangedu.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://rl.nicolike.cn

Ruby: def greet; "admin"; end
来源：http://pc.panjiajie.cn

C#:   public override string Greet() => "admin";
来源：http://qi.huanxung.cn

[G07] 调用父类方法
来源：http://wz.jianghongdianzi.cn

Py:   super().greet()
来源：http://yv.huixinmuqiang.cn

PHP:  parent::greet();
来源：http://ne.newstarts.cn

JS:   super.greet();
来源：http://oc.gzmigu.cn

TS:   super.greet();
来源：http://qv.521024.cn

Java: super.greet();
来源：http://gc.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://bx.521024.cn

Ruby: super
来源：http://tq.hahajie.cn

C#:   base.Greet();
来源：http://ng.szsharing.cn

[G08] 静态方法与属性
来源：http://bu.shxzskj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lc.huixiangedu.cn

PHP:  public static function f() {}
来源：http://oi.bookmarksfly.cn

JS:   static f() {}
来源：http://xf.shxzskj.cn

TS:   static f(): void {}
来源：http://wu.9csxet.cn

Java: static void f() {}
来源：http://gy.yuntaijiaju.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ct.yuntaijiaju.cn

Ruby: def self.f; end
来源：http://wk.szxytkj.cn

C#:   public static void F() {}
来源：http://bz.bjjhwx.cn

[G09] 接口 / 抽象类
来源：http://zl.szxytkj.cn

Py:   from abc import ABC, abstractmethod
来源：http://tk.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://hh.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ae.jianghongdianzi.cn

TS:   interface Shape { area(): number; }
来源：http://ea.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://vz.nszjky.cn

Go:   type Shape interface { Area() float64 }
来源：http://uz.szxytkj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yi.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://pt.9csxet.cn

[G10] 访问控制
来源：http://ur.huanxung.cn

Py:   约定 _protected / __private（不强制）
来源：http://xy.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://bn.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://zd.yuexingan06.cn

TS:   public / protected / private
来源：http://yr.yuexingan06.cn

Java: public / protected / private / 默认包级
来源：http://lu.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dg.bjjhwx.cn

Ruby: public / protected / private
来源：http://gi.521024.cn

C#:   public / protected / private / internal
来源：http://ed.haigaiapp.cn

[G11] getter / setter
来源：http://sz.bjjhwx.cn

Py:   @property 与 @x.setter
来源：http://ss.hahajie.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://je.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://as.colortex.cn

TS:   get name(): string { return this._name; }
来源：http://pa.bookmarksfly.cn

Java: public String getName() { return name; }
来源：http://se.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yr.huixiangedu.cn

Ruby: attr_accessor :name
来源：http://se.jctech888.com.cn

C#:   public string Name { get; set; }
来源：http://mt.newstarts.cn

[G12] 对象转字符串
来源：http://xn.colortex.cn

Py:   def __str__(self): return self.name
来源：http://rh.nicolike.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://sk.9csxet.cn

JS:   toString() { return this.name; }
来源：http://gf.huixiangedu.cn

TS:   toString(): string { return this.name; }
来源：http://eq.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://gz.szxytkj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://km.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://yg.huixinmuqiang.cn

C#:   public override string ToString() => Name;
来源：http://xr.bookmarksfly.cn

[G13] 判断对象类型
来源：http://ya.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://ak.huanxung.cn

PHP:  $u instanceof User
来源：http://sp.asd995.cn

JS:   u instanceof User
来源：http://bc.szsharing.cn

TS:   u instanceof User
来源：http://jn.shtwfgs.cn

Java: u instanceof User
来源：http://gi.asd995.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://su.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://fo.hahajie.cn

C#:   u is User
来源：http://ks.szsharing.cn

[G14] 数据类 / record
来源：http://sx.yuexingan06.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vk.shxzskj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ki.gzmigu.cn

JS:   // 无内置：普通类或对象字面量
来源：http://xv.shxzukj.cn

TS:   type User = { name: string; age: number };
来源：http://ir.yuntaijiaju.cn

Java: record User(String name, int age) {}
来源：http://ee.nicolike.cn

Go:   type User struct { Name string; Age int }
来源：http://wo.lnxyls.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gs.huixinmuqiang.cn

C#:   record User(string Name, int Age);
来源：http://yw.bookmarksfly.cn

[G15] 枚举
来源：http://yt.yuexingan06.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xl.shtwfgs.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rs.chemitech.net.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://gm.521024.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lk.bookmarksfly.cn

Java: enum Color { RED, GREEN }
来源：http://gx.muxihuayi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ol.szsharing.cn

Ruby: Color = %i[red green].freeze
来源：http://lj.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hg.haigaiapp.cn

[G16] 对象转数组 / 字典
来源：http://mu.shtwfgs.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zi.shtwfgs.cn


<!-- 参考信息 -->