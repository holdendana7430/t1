代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://co.muxihuayi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://jt.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://pk.shtwfgs.cn

Ruby: s.bytesize;  s.length
来源：http://tx.lnxyls.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://df.hahajie.cn

================================================================================
来源：http://iu.bookmarksfly.cn

F. 文件与目录
来源：http://le.lnxyls.cn

================================================================================
来源：http://eu.bookmarksfly.cn

[F01] 读取整个文件
来源：http://hk.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://py.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://ip.shxzskj.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://om.shxzukj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ny.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dn.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ug.nicolike.cn

Ruby: File.read("a.txt")
来源：http://iu.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://nw.huixinmuqiang.cn

[F02] 逐行读取文件
来源：http://wu.shxzskj.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://qf.muxihuayi.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://md.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://se.bjjhwx.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://vk.huixiangedu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://de.jianghongdianzi.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ts.wgjwhj.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fg.yuexingan06.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://zp.wgjwhj.cn

[F03] 写入文件（覆盖）
来源：http://jv.hahajie.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jj.yuexingan06.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://qg.muxihuayi.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://pw.yuexingan06.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://rb.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tm.huixiangedu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qf.newstarts.cn

Ruby: File.write("a.txt", "hi")
来源：http://mk.521024.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://he.huixiangedu.cn

[F04] 追加写入文件
来源：http://fg.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bj.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://td.szsharing.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wb.colortex.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://be.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://xy.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://sl.shxzskj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://zd.huanxung.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://pa.jctech888.com.cn

[F05] 判断文件或目录是否存在
来源：http://rc.nicolike.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://fa.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://wo.9csxet.cn

JS:   fs.existsSync("a.txt")
来源：http://dj.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://ix.bookmarksfly.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://sh.hnjuh.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://at.wgjwhj.cn

Ruby: File.exist?("a.txt")
来源：http://uw.jctech888.com.cn

C#:   File.Exists("a.txt")
来源：http://ei.yuntaijiaju.cn

[F06] 删除文件
来源：http://md.hnjuh.cn

Py:   os.remove("a.txt")
来源：http://df.szxytkj.cn

PHP:  unlink("a.txt");
来源：http://tl.shtwfgs.cn

JS:   fs.unlinkSync("a.txt")
来源：http://go.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://gv.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://cn.bookmarksfly.cn

Go:   os.Remove("a.txt")
来源：http://nn.gzmigu.cn

Ruby: File.delete("a.txt")
来源：http://bc.panjiajie.cn

C#:   File.Delete("a.txt");
来源：http://ah.hnjuh.cn

[F07] 创建目录（含多级）
来源：http://en.szsharing.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mv.asd995.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://nd.muxihuayi.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ab.wgjwhj.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://tt.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://em.lnxyls.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://io.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://vg.bookmarksfly.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://bd.haigaiapp.cn

[F08] 遍历目录
来源：http://yl.szxytkj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://um.bookmarksfly.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ky.shtwfgs.cn

JS:   fs.readdirSync("dir")
来源：http://tb.newstarts.cn

TS:   fs.readdirSync("dir")
来源：http://ko.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://qg.yuexingan06.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fv.wgjwhj.cn

Ruby: Dir.children("dir")
来源：http://sc.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://rx.szsharing.cn

[F09] 获取文件大小
来源：http://xh.hnjuh.cn

Py:   os.path.getsize("a.txt")
来源：http://cr.hahajie.cn

PHP:  filesize("a.txt");
来源：http://gq.asd995.cn

JS:   fs.statSync("a.txt").size
来源：http://eb.bookmarksfly.cn

TS:   fs.statSync("a.txt").size
来源：http://oy.lnxyls.cn

Java: Files.size(Path.of("a.txt"))
来源：http://lo.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://im.szxytkj.cn

Ruby: File.size("a.txt")
来源：http://sy.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://me.nicolike.cn

[F10] 取文件扩展名 / 文件名
来源：http://pp.muxihuayi.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://dw.hnjuh.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://nh.hahajie.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ll.newstarts.cn

TS:   path.extname("a.txt")
来源：http://ss.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://fi.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://lb.wgjwhj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mc.gzmigu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://yk.bjjhwx.cn

[F11] 复制与移动文件
来源：http://eo.huanxung.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hb.nszjky.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yl.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://lr.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bq.hahajie.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ki.lnxyls.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ra.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://vr.panjiajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ju.chemitech.net.cn

[F12] CSV 读写
来源：http://do.asd995.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://lr.yuexingan06.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ni.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hh.huixiangedu.cn

TS:   // 同上
来源：http://du.panjiajie.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://jd.nicolike.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ob.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bz.9csxet.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://ui.yuexingan06.cn

================================================================================
来源：http://jr.jctech888.com.cn

G. 面向对象
来源：http://hq.wgjwhj.cn

================================================================================
来源：http://ug.haigaiapp.cn

[G01] 定义类
来源：http://xf.szsharing.cn

Py:   class User: pass
来源：http://vl.bjjhwx.cn

PHP:  class User {}
来源：http://gt.hahajie.cn

JS:   class User {}
来源：http://to.gzmigu.cn

TS:   class User { name: string = ""; }
来源：http://vk.nszjky.cn

Java: class User {}
来源：http://wz.lnxyls.cn

Go:   type User struct { Name string }
来源：http://um.hahajie.cn

Ruby: class User; end
来源：http://dh.nicolike.cn

C#:   class User {}
来源：http://jm.haigaiapp.cn

[G02] 构造函数
来源：http://ib.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://ef.yuexingan06.cn

PHP:  public function __construct(public string $name) {}
来源：http://fh.haigaiapp.cn

JS:   constructor(name) { this.name = name; }
来源：http://ry.jctech888.com.cn

TS:   constructor(public name: string) {}
来源：http://le.haigaiapp.cn

Java: User(String name) { this.name = name; }
来源：http://kp.colortex.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lx.chemitech.net.cn

Ruby: def initialize(name); @name = name; end
来源：http://kl.bookmarksfly.cn

C#:   public User(string name) { Name = name; }
来源：http://wx.newstarts.cn

[G03] 实例属性
来源：http://aa.jianghongdianzi.cn

Py:   self.name = "x"
来源：http://dr.jianghongdianzi.cn

PHP:  public string $name = "x";
来源：http://ua.szxytkj.cn

JS:   this.name = "x";
来源：http://dg.jctech888.com.cn

TS:   name: string = "x";
来源：http://pp.szxytkj.cn

Java: private String name;
来源：http://pa.jianghongdianzi.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://js.hahajie.cn

Ruby: @name = "x"
来源：http://mq.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://jb.yuexingan06.cn

[G04] 定义方法
来源：http://nw.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://rh.shtwfgs.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ln.hahajie.cn

JS:   greet() { return this.name; }
来源：http://md.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://nd.yuntaijiaju.cn

Java: String greet() { return name; }
来源：http://la.chemitech.net.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://tl.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://wj.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://bw.newstarts.cn

[G05] 继承
来源：http://jh.hahajie.cn

Py:   class Admin(User): pass
来源：http://vm.jctech888.com.cn

PHP:  class Admin extends User {}
来源：http://wc.shxzukj.cn

JS:   class Admin extends User {}
来源：http://pf.hahajie.cn

TS:   class Admin extends User {}
来源：http://kh.lnxyls.cn

Java: class Admin extends User {}
来源：http://lk.haigaiapp.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ur.huanxung.cn

Ruby: class Admin < User; end
来源：http://wz.asd995.cn

C#:   class Admin : User {}
来源：http://gx.haigaiapp.cn

[G06] 重写方法
来源：http://js.huixiangedu.cn

Py:   def greet(self): return "admin"
来源：http://gb.asd995.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://fc.huanxung.cn

JS:   greet() { return "admin"; }
来源：http://io.nszjky.cn

TS:   greet(): string { return "admin"; }
来源：http://lb.haigaiapp.cn

Java: @Override String greet() { return "admin"; }
来源：http://nw.521024.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://he.haigaiapp.cn

Ruby: def greet; "admin"; end
来源：http://tj.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://sw.yuexingan06.cn

[G07] 调用父类方法
来源：http://kg.shxzskj.cn

Py:   super().greet()
来源：http://rh.szxytkj.cn

PHP:  parent::greet();
来源：http://mb.jianghongdianzi.cn

JS:   super.greet();
来源：http://vd.huixinmuqiang.cn

TS:   super.greet();
来源：http://iz.huixinmuqiang.cn

Java: super.greet();
来源：http://ia.chemitech.net.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yr.lnxyls.cn

Ruby: super
来源：http://zr.jctech888.com.cn

C#:   base.Greet();
来源：http://is.shtwfgs.cn

[G08] 静态方法与属性
来源：http://hx.lnxyls.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://zr.lnxyls.cn

PHP:  public static function f() {}
来源：http://ls.szxytkj.cn

JS:   static f() {}
来源：http://ta.wgjwhj.cn

TS:   static f(): void {}
来源：http://iq.yuntaijiaju.cn

Java: static void f() {}
来源：http://kk.hahajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ft.shxzskj.cn

Ruby: def self.f; end
来源：http://pw.wgjwhj.cn

C#:   public static void F() {}
来源：http://ux.panjiajie.cn

[G09] 接口 / 抽象类
来源：http://fi.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://lq.yuntaijiaju.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ut.nicolike.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://ht.shtwfgs.cn

TS:   interface Shape { area(): number; }
来源：http://mr.hahajie.cn

Java: interface Shape { double area(); }
来源：http://my.newstarts.cn

Go:   type Shape interface { Area() float64 }
来源：http://hd.hnjuh.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://uc.gzmigu.cn

C#:   interface IShape { double Area(); }
来源：http://dt.bjjhwx.cn

[G10] 访问控制
来源：http://yo.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://aj.lnxyls.cn

PHP:  public / protected / private
来源：http://nc.lnxyls.cn

JS:   #private 字段；其余公开
来源：http://ny.chemitech.net.cn

TS:   public / protected / private
来源：http://ev.haigaiapp.cn

Java: public / protected / private / 默认包级
来源：http://of.huixiangedu.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cu.wgjwhj.cn

Ruby: public / protected / private
来源：http://oy.9csxet.cn

C#:   public / protected / private / internal
来源：http://qa.bjjhwx.cn

[G11] getter / setter
来源：http://ol.szxytkj.cn

Py:   @property 与 @x.setter
来源：http://ji.colortex.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://dk.yuexingan06.cn

JS:   get name() { return this._name; }
来源：http://lq.jianghongdianzi.cn

TS:   get name(): string { return this._name; }
来源：http://fw.nszjky.cn

Java: public String getName() { return name; }
来源：http://wm.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tq.shtwfgs.cn

Ruby: attr_accessor :name
来源：http://sp.jianghongdianzi.cn

C#:   public string Name { get; set; }
来源：http://fx.bjjhwx.cn

[G12] 对象转字符串
来源：http://wj.shxzukj.cn

Py:   def __str__(self): return self.name
来源：http://ou.lnxyls.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://dv.nicolike.cn

JS:   toString() { return this.name; }
来源：http://xc.shxzukj.cn

TS:   toString(): string { return this.name; }
来源：http://pg.hahajie.cn

Java: @Override public String toString() { return name; }
来源：http://pt.521024.cn

Go:   func (u User) String() string { return u.Name }
来源：http://dz.hahajie.cn

Ruby: def to_s; @name; end
来源：http://ua.lnxyls.cn

C#:   public override string ToString() => Name;
来源：http://ip.colortex.cn

[G13] 判断对象类型
来源：http://sr.hahajie.cn

Py:   isinstance(u, User)
来源：http://eb.jctech888.com.cn

PHP:  $u instanceof User
来源：http://xn.huixiangedu.cn

JS:   u instanceof User
来源：http://hx.asd995.cn

TS:   u instanceof User
来源：http://um.muxihuayi.cn

Java: u instanceof User
来源：http://pp.huixinmuqiang.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://gj.colortex.cn

Ruby: u.is_a?(User)
来源：http://jp.lnxyls.cn

C#:   u is User
来源：http://ui.bookmarksfly.cn

[G14] 数据类 / record
来源：http://iz.gzmigu.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://vk.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://ae.shxzukj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://az.hahajie.cn

TS:   type User = { name: string; age: number };
来源：http://sm.hahajie.cn

Java: record User(String name, int age) {}
来源：http://ll.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://be.yuntaijiaju.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://do.huixiangedu.cn

C#:   record User(string Name, int Age);
来源：http://cr.jctech888.com.cn

[G15] 枚举
来源：http://qc.gzmigu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://np.lnxyls.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://jr.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zm.yuexingan06.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cd.hnjuh.cn

Java: enum Color { RED, GREEN }
来源：http://zw.yuexingan06.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yo.bookmarksfly.cn

Ruby: Color = %i[red green].freeze
来源：http://tj.panjiajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://xs.colortex.cn

[G16] 对象转数组 / 字典
来源：http://tn.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://jh.521024.cn

PHP:  get_object_vars($obj);
来源：http://it.szxytkj.cn

JS:   Object.entries(obj)
来源：http://yo.szsharing.cn

TS:   Object.entries(obj)
来源：http://vl.shxzskj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://bx.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ql.huanxung.cn

Ruby: obj.instance_variables
来源：http://fw.panjiajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://er.bookmarksfly.cn

================================================================================
来源：http://to.haigaiapp.cn

H. 异常与错误处理
来源：http://gh.huanxung.cn

================================================================================
来源：http://uf.haigaiapp.cn

[H01] try / catch 基础
来源：http://kg.521024.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://dm.wgjwhj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://jt.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://oe.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://qn.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pd.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://vw.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://jn.hnjuh.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://sb.huixiangedu.cn

[H02] finally / ensure 收尾
来源：http://lk.nszjky.cn

Py:   try: f()⏎finally: cleanup()
来源：http://wn.bjjhwx.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://xc.haigaiapp.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://cm.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://qv.haigaiapp.cn

Java: try { f(); } finally { cleanup(); }
来源：http://kx.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zx.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://iw.shxzskj.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zc.hahajie.cn

[H03] 主动抛出异常
来源：http://rz.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://wv.yuntaijiaju.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://qd.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://uz.bookmarksfly.cn

TS:   throw new Error("错误信息");
来源：http://yr.chemitech.net.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cj.wgjwhj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://tt.huixiangedu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://br.jianghongdianzi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://nf.muxihuayi.cn

[H04] 自定义异常类型
来源：http://dg.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://kj.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://kk.hahajie.cn

JS:   class MyError extends Error {}
来源：http://af.jianghongdianzi.cn

TS:   class MyError extends Error {}
来源：http://rb.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://pi.nicolike.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://nx.hnjuh.cn


<!-- 参考信息 -->