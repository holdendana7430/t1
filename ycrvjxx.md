代发 wailian999

Go:   if s == "" {}
来源：http://df.shxzskj.cn

Ruby: if s.empty?
来源：http://bo.jianghongdianzi.cn

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wa.jctech888.com.cn

[E21] 超长截断加省略号
来源：http://no.chemitech.net.cn

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://aj.9csxet.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://zq.szsharing.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://le.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://ss.nszjky.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wz.shtwfgs.cn

Go:   // 按 rune 判断长度后截断
来源：http://fl.szxytkj.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wi.asd995.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://ng.asd995.cn

[E22] 字节长度与字符长度
来源：http://gj.9csxet.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://jo.yuntaijiaju.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://ib.colortex.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://xs.lnxyls.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uu.9csxet.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dc.shxzukj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://ce.muxihuayi.cn

Ruby: s.bytesize;  s.length
来源：http://kp.wgjwhj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://kd.huanxung.cn

================================================================================
来源：http://qf.huixiangedu.cn

F. 文件与目录
来源：http://ad.hnjuh.cn

================================================================================
来源：http://gy.yuntaijiaju.cn

[F01] 读取整个文件
来源：http://om.shxzskj.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://uh.asd995.cn

PHP:  file_get_contents("a.txt");
来源：http://gg.bookmarksfly.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://zb.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iv.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://xw.gzmigu.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://dm.bookmarksfly.cn

Ruby: File.read("a.txt")
来源：http://cv.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://wi.shxzskj.cn

[F02] 逐行读取文件
来源：http://fa.521024.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://fy.shxzskj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://lw.huanxung.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://lu.gzmigu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://az.521024.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ey.muxihuayi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://cj.9csxet.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://pc.huixiangedu.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://dh.shxzskj.cn

[F03] 写入文件（覆盖）
来源：http://ba.521024.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oz.szxytkj.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://on.colortex.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://og.gzmigu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ou.szsharing.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tz.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://py.shtwfgs.cn

Ruby: File.write("a.txt", "hi")
来源：http://pd.huanxung.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ib.lnxyls.cn

[F04] 追加写入文件
来源：http://xx.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wo.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://qi.bjjhwx.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://os.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://qr.bookmarksfly.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://dx.bjjhwx.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://gu.huixiangedu.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://qt.huixiangedu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ll.szsharing.cn

[F05] 判断文件或目录是否存在
来源：http://rs.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://gx.panjiajie.cn

PHP:  file_exists("a.txt");
来源：http://rf.jctech888.com.cn

JS:   fs.existsSync("a.txt")
来源：http://rj.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://st.huixinmuqiang.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://rk.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://sg.asd995.cn

Ruby: File.exist?("a.txt")
来源：http://vp.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://ou.lnxyls.cn

[F06] 删除文件
来源：http://nz.bjjhwx.cn

Py:   os.remove("a.txt")
来源：http://uq.chemitech.net.cn

PHP:  unlink("a.txt");
来源：http://wf.nicolike.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zt.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://uf.szxytkj.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fy.hahajie.cn

Go:   os.Remove("a.txt")
来源：http://eb.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://me.jctech888.com.cn

C#:   File.Delete("a.txt");
来源：http://zk.lnxyls.cn

[F07] 创建目录（含多级）
来源：http://qa.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://px.yuntaijiaju.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://zt.colortex.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zr.huixinmuqiang.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rx.haigaiapp.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://jk.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://kp.shtwfgs.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ub.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://na.muxihuayi.cn

[F08] 遍历目录
来源：http://md.gzmigu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fp.gzmigu.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ce.nszjky.cn

JS:   fs.readdirSync("dir")
来源：http://xo.bjjhwx.cn

TS:   fs.readdirSync("dir")
来源：http://lc.hahajie.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fh.521024.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ih.shxzukj.cn

Ruby: Dir.children("dir")
来源：http://kh.chemitech.net.cn

C#:   Directory.GetFiles("dir")
来源：http://rv.hahajie.cn

[F09] 获取文件大小
来源：http://ij.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://jl.gzmigu.cn

PHP:  filesize("a.txt");
来源：http://qb.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://qm.jianghongdianzi.cn

TS:   fs.statSync("a.txt").size
来源：http://gg.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hr.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pr.gzmigu.cn

Ruby: File.size("a.txt")
来源：http://qt.colortex.cn

C#:   new FileInfo("a.txt").Length
来源：http://ck.bookmarksfly.cn

[F10] 取文件扩展名 / 文件名
来源：http://wq.hnjuh.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ut.jianghongdianzi.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://th.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qw.colortex.cn

TS:   path.extname("a.txt")
来源：http://wf.wgjwhj.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ou.asd995.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://pd.hahajie.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ee.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sr.shxzukj.cn

[F11] 复制与移动文件
来源：http://or.lnxyls.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ie.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://pf.wgjwhj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://jy.szxytkj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://do.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ot.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cc.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ww.huixiangedu.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://so.panjiajie.cn

[F12] CSV 读写
来源：http://zo.muxihuayi.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sx.szxytkj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://om.muxihuayi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://we.shtwfgs.cn

TS:   // 同上
来源：http://fh.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fc.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://bv.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://zg.panjiajie.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://zg.bookmarksfly.cn

================================================================================
来源：http://kt.hnjuh.cn

G. 面向对象
来源：http://jl.gzmigu.cn

================================================================================
来源：http://tp.lnxyls.cn

[G01] 定义类
来源：http://od.muxihuayi.cn

Py:   class User: pass
来源：http://yl.hahajie.cn

PHP:  class User {}
来源：http://mv.shtwfgs.cn

JS:   class User {}
来源：http://zd.jianghongdianzi.cn

TS:   class User { name: string = ""; }
来源：http://dv.haigaiapp.cn

Java: class User {}
来源：http://wj.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://un.huanxung.cn

Ruby: class User; end
来源：http://od.szsharing.cn

C#:   class User {}
来源：http://fq.hahajie.cn

[G02] 构造函数
来源：http://wn.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://io.huixinmuqiang.cn

PHP:  public function __construct(public string $name) {}
来源：http://jj.yuexingan06.cn

JS:   constructor(name) { this.name = name; }
来源：http://fk.wgjwhj.cn

TS:   constructor(public name: string) {}
来源：http://zl.huanxung.cn

Java: User(String name) { this.name = name; }
来源：http://fq.jctech888.com.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://nx.szxytkj.cn

Ruby: def initialize(name); @name = name; end
来源：http://be.wgjwhj.cn

C#:   public User(string name) { Name = name; }
来源：http://rt.521024.cn

[G03] 实例属性
来源：http://ni.muxihuayi.cn

Py:   self.name = "x"
来源：http://lo.newstarts.cn

PHP:  public string $name = "x";
来源：http://ks.nicolike.cn

JS:   this.name = "x";
来源：http://bo.hahajie.cn

TS:   name: string = "x";
来源：http://cs.shxzukj.cn

Java: private String name;
来源：http://de.shxzskj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kw.bjjhwx.cn

Ruby: @name = "x"
来源：http://gj.huanxung.cn

C#:   public string Name { get; set; } = "x";
来源：http://lt.newstarts.cn

[G04] 定义方法
来源：http://is.jctech888.com.cn

Py:   def greet(self): return self.name
来源：http://ff.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fy.wgjwhj.cn

JS:   greet() { return this.name; }
来源：http://ay.huixiangedu.cn

TS:   greet(): string { return this.name; }
来源：http://iz.haigaiapp.cn

Java: String greet() { return name; }
来源：http://ko.hahajie.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ky.nicolike.cn

Ruby: def greet; @name; end
来源：http://mh.huanxung.cn

C#:   public string Greet() => Name;
来源：http://ne.haigaiapp.cn

[G05] 继承
来源：http://ju.bookmarksfly.cn

Py:   class Admin(User): pass
来源：http://lk.hnjuh.cn

PHP:  class Admin extends User {}
来源：http://rj.huixinmuqiang.cn

JS:   class Admin extends User {}
来源：http://jv.szsharing.cn

TS:   class Admin extends User {}
来源：http://sj.szxytkj.cn

Java: class Admin extends User {}
来源：http://ud.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://tr.chemitech.net.cn

Ruby: class Admin < User; end
来源：http://yj.asd995.cn

C#:   class Admin : User {}
来源：http://tn.jctech888.com.cn

[G06] 重写方法
来源：http://xg.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://pa.newstarts.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://xt.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://sz.jctech888.com.cn

TS:   greet(): string { return "admin"; }
来源：http://nk.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ic.yuntaijiaju.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hy.panjiajie.cn

Ruby: def greet; "admin"; end
来源：http://ie.bjjhwx.cn

C#:   public override string Greet() => "admin";
来源：http://lu.wgjwhj.cn

[G07] 调用父类方法
来源：http://yl.bookmarksfly.cn

Py:   super().greet()
来源：http://xm.lnxyls.cn

PHP:  parent::greet();
来源：http://td.huanxung.cn

JS:   super.greet();
来源：http://qm.yuexingan06.cn

TS:   super.greet();
来源：http://vq.shxzukj.cn

Java: super.greet();
来源：http://by.shxzskj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://da.wgjwhj.cn

Ruby: super
来源：http://ae.hahajie.cn

C#:   base.Greet();
来源：http://ij.huanxung.cn

[G08] 静态方法与属性
来源：http://wu.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ut.9csxet.cn

PHP:  public static function f() {}
来源：http://wf.nszjky.cn

JS:   static f() {}
来源：http://cz.jctech888.com.cn

TS:   static f(): void {}
来源：http://ud.shxzukj.cn

Java: static void f() {}
来源：http://vs.shtwfgs.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://po.gzmigu.cn

Ruby: def self.f; end
来源：http://we.gzmigu.cn

C#:   public static void F() {}
来源：http://rg.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://dk.asd995.cn

Py:   from abc import ABC, abstractmethod
来源：http://rc.colortex.cn

PHP:  interface Shape { public function area(): float; }
来源：http://oc.newstarts.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ra.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://gj.shxzskj.cn

Java: interface Shape { double area(); }
来源：http://iv.jianghongdianzi.cn

Go:   type Shape interface { Area() float64 }
来源：http://nm.shxzukj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://sn.asd995.cn

C#:   interface IShape { double Area(); }
来源：http://nd.nicolike.cn

[G10] 访问控制
来源：http://fb.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://vx.shtwfgs.cn

PHP:  public / protected / private
来源：http://ai.chemitech.net.cn

JS:   #private 字段；其余公开
来源：http://ar.gzmigu.cn

TS:   public / protected / private
来源：http://uj.shxzskj.cn

Java: public / protected / private / 默认包级
来源：http://ce.nicolike.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://le.haigaiapp.cn

Ruby: public / protected / private
来源：http://xo.shtwfgs.cn

C#:   public / protected / private / internal
来源：http://wp.yuntaijiaju.cn

[G11] getter / setter
来源：http://uz.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://de.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ku.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://fb.bookmarksfly.cn

TS:   get name(): string { return this._name; }
来源：http://zb.asd995.cn

Java: public String getName() { return name; }
来源：http://gx.szxytkj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://yi.shxzskj.cn

Ruby: attr_accessor :name
来源：http://eb.huixinmuqiang.cn

C#:   public string Name { get; set; }
来源：http://du.asd995.cn

[G12] 对象转字符串
来源：http://zt.521024.cn

Py:   def __str__(self): return self.name
来源：http://gs.huanxung.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://rz.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://ay.9csxet.cn

TS:   toString(): string { return this.name; }
来源：http://as.bjjhwx.cn

Java: @Override public String toString() { return name; }
来源：http://ot.panjiajie.cn

Go:   func (u User) String() string { return u.Name }
来源：http://vx.huixiangedu.cn

Ruby: def to_s; @name; end
来源：http://za.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://mr.9csxet.cn

[G13] 判断对象类型
来源：http://ox.jctech888.com.cn

Py:   isinstance(u, User)
来源：http://ti.shxzskj.cn

PHP:  $u instanceof User
来源：http://hz.shtwfgs.cn

JS:   u instanceof User
来源：http://jr.shxzukj.cn

TS:   u instanceof User
来源：http://dn.bookmarksfly.cn

Java: u instanceof User
来源：http://cm.muxihuayi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://wr.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://ek.wgjwhj.cn

C#:   u is User
来源：http://lz.nszjky.cn

[G14] 数据类 / record
来源：http://sd.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ji.asd995.cn

PHP:  // 用 readonly 属性模拟
来源：http://vp.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sl.gzmigu.cn

TS:   type User = { name: string; age: number };
来源：http://qp.shxzskj.cn

Java: record User(String name, int age) {}
来源：http://dy.jctech888.com.cn

Go:   type User struct { Name string; Age int }
来源：http://dk.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://vz.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://ob.huanxung.cn

[G15] 枚举
来源：http://nn.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://kw.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jd.szxytkj.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://jw.9csxet.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ad.chemitech.net.cn

Java: enum Color { RED, GREEN }
来源：http://kn.bjjhwx.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://eu.nicolike.cn

Ruby: Color = %i[red green].freeze
来源：http://mu.chemitech.net.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://tu.szxytkj.cn

[G16] 对象转数组 / 字典
来源：http://ty.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://zt.nszjky.cn

PHP:  get_object_vars($obj);
来源：http://wy.nszjky.cn

JS:   Object.entries(obj)
来源：http://jp.huixinmuqiang.cn

TS:   Object.entries(obj)
来源：http://wr.521024.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://gi.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://pn.521024.cn

Ruby: obj.instance_variables
来源：http://uc.chemitech.net.cn

C#:   // 用反射或 System.Text.Json
来源：http://uj.lnxyls.cn

================================================================================
来源：http://pn.bookmarksfly.cn

H. 异常与错误处理
来源：http://al.shtwfgs.cn

================================================================================
来源：http://wh.newstarts.cn

[H01] try / catch 基础
来源：http://gb.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://zo.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yf.huixinmuqiang.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://tn.yuntaijiaju.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://pr.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lo.gzmigu.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mn.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wy.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://pk.521024.cn

[H02] finally / ensure 收尾
来源：http://hs.yuntaijiaju.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ip.huanxung.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://os.yuntaijiaju.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://zp.panjiajie.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ad.lnxyls.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ky.9csxet.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://sl.wgjwhj.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://hu.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mm.nszjky.cn


<!-- 参考信息 -->