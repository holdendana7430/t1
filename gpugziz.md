代发 wailian999

[E22] 字节长度与字符长度
来源：http://ci.chemitech.net.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://dt.bookmarksfly.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mr.huixinmuqiang.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://uo.yuexingan06.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ou.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://iq.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://gv.huanxung.cn

Ruby: s.bytesize;  s.length
来源：http://bb.shxzukj.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://ee.newstarts.cn

================================================================================
来源：http://rk.shtwfgs.cn

F. 文件与目录
来源：http://yk.nicolike.cn

================================================================================
来源：http://zv.colortex.cn

[F01] 读取整个文件
来源：http://pv.jctech888.com.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://sn.gzmigu.cn

PHP:  file_get_contents("a.txt");
来源：http://gs.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://aq.yuexingan06.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://av.szsharing.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://fp.9csxet.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://ad.shxzskj.cn

Ruby: File.read("a.txt")
来源：http://yc.panjiajie.cn

C#:   File.ReadAllText("a.txt");
来源：http://as.szsharing.cn

[F02] 逐行读取文件
来源：http://hv.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://um.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://rh.gzmigu.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mj.huixiangedu.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jy.shtwfgs.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://ls.szsharing.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://sx.jianghongdianzi.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://bb.chemitech.net.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://gk.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://wh.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://xa.hahajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hl.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://sg.shxzskj.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ba.521024.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lo.huanxung.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ge.yuntaijiaju.cn

Ruby: File.write("a.txt", "hi")
来源：http://nn.shxzskj.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://ly.jctech888.com.cn

[F04] 追加写入文件
来源：http://xl.9csxet.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://zv.newstarts.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ad.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ks.jianghongdianzi.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://lx.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cl.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://bo.huixinmuqiang.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://le.hnjuh.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rm.nszjky.cn

[F05] 判断文件或目录是否存在
来源：http://fr.bookmarksfly.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://bu.521024.cn

PHP:  file_exists("a.txt");
来源：http://jk.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://dc.haigaiapp.cn

TS:   fs.existsSync("a.txt")
来源：http://cp.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://aj.bjjhwx.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://fe.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://cz.yuexingan06.cn

C#:   File.Exists("a.txt")
来源：http://xt.newstarts.cn

[F06] 删除文件
来源：http://en.huanxung.cn

Py:   os.remove("a.txt")
来源：http://sn.muxihuayi.cn

PHP:  unlink("a.txt");
来源：http://kp.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://qk.wgjwhj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://xk.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://qf.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://jw.newstarts.cn

Ruby: File.delete("a.txt")
来源：http://lf.huixiangedu.cn

C#:   File.Delete("a.txt");
来源：http://oq.nszjky.cn

[F07] 创建目录（含多级）
来源：http://ec.bjjhwx.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://nj.huixinmuqiang.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://es.huanxung.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ah.huixiangedu.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://iy.jianghongdianzi.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://xm.szxytkj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://qp.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ss.colortex.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://vf.nszjky.cn

[F08] 遍历目录
来源：http://aa.shtwfgs.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://of.shtwfgs.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://np.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://gl.nicolike.cn

TS:   fs.readdirSync("dir")
来源：http://hb.huixiangedu.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mh.szxytkj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://fa.bookmarksfly.cn

Ruby: Dir.children("dir")
来源：http://ks.bjjhwx.cn

C#:   Directory.GetFiles("dir")
来源：http://up.shxzukj.cn

[F09] 获取文件大小
来源：http://ne.yuexingan06.cn

Py:   os.path.getsize("a.txt")
来源：http://aw.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://gf.szsharing.cn

JS:   fs.statSync("a.txt").size
来源：http://ch.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://zy.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://pl.nszjky.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hw.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://tr.newstarts.cn

C#:   new FileInfo("a.txt").Length
来源：http://hk.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://uy.gzmigu.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://qs.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://ng.chemitech.net.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://iz.asd995.cn

TS:   path.extname("a.txt")
来源：http://fm.yuexingan06.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ej.yuntaijiaju.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://es.jianghongdianzi.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://dm.nicolike.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://iq.gzmigu.cn

[F11] 复制与移动文件
来源：http://pn.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uh.shxzskj.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ve.lnxyls.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ep.jctech888.com.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://su.chemitech.net.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://rc.muxihuayi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://po.huixinmuqiang.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hw.lnxyls.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://jy.jctech888.com.cn

[F12] CSV 读写
来源：http://zx.bookmarksfly.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://qx.haigaiapp.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ye.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://nl.yuexingan06.cn

TS:   // 同上
来源：http://bw.521024.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rd.shxzskj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://ti.bjjhwx.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://uj.jianghongdianzi.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fl.nszjky.cn

================================================================================
来源：http://ud.bjjhwx.cn

G. 面向对象
来源：http://pb.wgjwhj.cn

================================================================================
来源：http://yt.jctech888.com.cn

[G01] 定义类
来源：http://wk.shxzukj.cn

Py:   class User: pass
来源：http://vl.yuntaijiaju.cn

PHP:  class User {}
来源：http://hm.shxzskj.cn

JS:   class User {}
来源：http://mn.bookmarksfly.cn

TS:   class User { name: string = ""; }
来源：http://ky.hnjuh.cn

Java: class User {}
来源：http://uc.bjjhwx.cn

Go:   type User struct { Name string }
来源：http://xm.huixiangedu.cn

Ruby: class User; end
来源：http://wv.szxytkj.cn

C#:   class User {}
来源：http://zr.shtwfgs.cn

[G02] 构造函数
来源：http://rc.shxzskj.cn

Py:   def __init__(self, name): self.name = name
来源：http://xr.wgjwhj.cn

PHP:  public function __construct(public string $name) {}
来源：http://vf.asd995.cn

JS:   constructor(name) { this.name = name; }
来源：http://kw.hahajie.cn

TS:   constructor(public name: string) {}
来源：http://tt.szxytkj.cn

Java: User(String name) { this.name = name; }
来源：http://vy.huixinmuqiang.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://ex.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://za.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://mj.shtwfgs.cn

[G03] 实例属性
来源：http://vc.jctech888.com.cn

Py:   self.name = "x"
来源：http://yx.hnjuh.cn

PHP:  public string $name = "x";
来源：http://ev.nicolike.cn

JS:   this.name = "x";
来源：http://pa.huixinmuqiang.cn

TS:   name: string = "x";
来源：http://xa.jctech888.com.cn

Java: private String name;
来源：http://ri.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://qj.jctech888.com.cn

Ruby: @name = "x"
来源：http://uj.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://rq.hahajie.cn

[G04] 定义方法
来源：http://bs.panjiajie.cn

Py:   def greet(self): return self.name
来源：http://vd.shxzukj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://wx.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://lg.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://wi.gzmigu.cn

Java: String greet() { return name; }
来源：http://xx.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ag.huixiangedu.cn

Ruby: def greet; @name; end
来源：http://ny.haigaiapp.cn

C#:   public string Greet() => Name;
来源：http://gl.yuexingan06.cn

[G05] 继承
来源：http://wy.yuntaijiaju.cn

Py:   class Admin(User): pass
来源：http://xx.szsharing.cn

PHP:  class Admin extends User {}
来源：http://yn.yuexingan06.cn

JS:   class Admin extends User {}
来源：http://bo.huixinmuqiang.cn

TS:   class Admin extends User {}
来源：http://ac.nszjky.cn

Java: class Admin extends User {}
来源：http://hk.shxzukj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://rn.newstarts.cn

Ruby: class Admin < User; end
来源：http://bk.jctech888.com.cn

C#:   class Admin : User {}
来源：http://us.521024.cn

[G06] 重写方法
来源：http://wr.szsharing.cn

Py:   def greet(self): return "admin"
来源：http://mj.nszjky.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cq.hahajie.cn

JS:   greet() { return "admin"; }
来源：http://ju.hnjuh.cn

TS:   greet(): string { return "admin"; }
来源：http://hs.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://cc.panjiajie.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yf.shxzukj.cn

Ruby: def greet; "admin"; end
来源：http://yk.szxytkj.cn

C#:   public override string Greet() => "admin";
来源：http://lz.521024.cn

[G07] 调用父类方法
来源：http://sn.panjiajie.cn

Py:   super().greet()
来源：http://td.nszjky.cn

PHP:  parent::greet();
来源：http://vn.yuexingan06.cn

JS:   super.greet();
来源：http://dv.huixiangedu.cn

TS:   super.greet();
来源：http://rs.gzmigu.cn

Java: super.greet();
来源：http://ro.muxihuayi.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://uu.jctech888.com.cn

Ruby: super
来源：http://ee.shxzukj.cn

C#:   base.Greet();
来源：http://ef.muxihuayi.cn

[G08] 静态方法与属性
来源：http://dt.hnjuh.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ec.jianghongdianzi.cn

PHP:  public static function f() {}
来源：http://pj.szxytkj.cn

JS:   static f() {}
来源：http://yq.lnxyls.cn

TS:   static f(): void {}
来源：http://yq.huixinmuqiang.cn

Java: static void f() {}
来源：http://us.nicolike.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sc.hahajie.cn

Ruby: def self.f; end
来源：http://kp.panjiajie.cn

C#:   public static void F() {}
来源：http://hm.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://ix.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://lm.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ob.huanxung.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://iz.newstarts.cn

TS:   interface Shape { area(): number; }
来源：http://nw.szxytkj.cn

Java: interface Shape { double area(); }
来源：http://mk.yuntaijiaju.cn

Go:   type Shape interface { Area() float64 }
来源：http://oi.shxzskj.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://pw.haigaiapp.cn

C#:   interface IShape { double Area(); }
来源：http://om.asd995.cn

[G10] 访问控制
来源：http://ki.hahajie.cn

Py:   约定 _protected / __private（不强制）
来源：http://ej.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://zy.asd995.cn

JS:   #private 字段；其余公开
来源：http://cd.jianghongdianzi.cn

TS:   public / protected / private
来源：http://ta.muxihuayi.cn

Java: public / protected / private / 默认包级
来源：http://dm.shxzskj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://oy.panjiajie.cn

Ruby: public / protected / private
来源：http://ww.huixiangedu.cn

C#:   public / protected / private / internal
来源：http://wh.nicolike.cn

[G11] getter / setter
来源：http://wh.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://lx.newstarts.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ik.szsharing.cn

JS:   get name() { return this._name; }
来源：http://am.bjjhwx.cn

TS:   get name(): string { return this._name; }
来源：http://gn.szxytkj.cn

Java: public String getName() { return name; }
来源：http://en.newstarts.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://xc.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://md.bookmarksfly.cn

C#:   public string Name { get; set; }
来源：http://qz.521024.cn

[G12] 对象转字符串
来源：http://qm.yuntaijiaju.cn

Py:   def __str__(self): return self.name
来源：http://rg.nszjky.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bn.bjjhwx.cn

JS:   toString() { return this.name; }
来源：http://yd.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://td.nszjky.cn

Java: @Override public String toString() { return name; }
来源：http://lh.9csxet.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kd.yuexingan06.cn

Ruby: def to_s; @name; end
来源：http://lo.9csxet.cn

C#:   public override string ToString() => Name;
来源：http://om.huanxung.cn

[G13] 判断对象类型
来源：http://iw.szxytkj.cn

Py:   isinstance(u, User)
来源：http://va.hahajie.cn

PHP:  $u instanceof User
来源：http://uz.huixiangedu.cn

JS:   u instanceof User
来源：http://ni.hahajie.cn

TS:   u instanceof User
来源：http://kg.lnxyls.cn

Java: u instanceof User
来源：http://dm.yuexingan06.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://be.szxytkj.cn

Ruby: u.is_a?(User)
来源：http://wu.yuntaijiaju.cn

C#:   u is User
来源：http://pz.521024.cn

[G14] 数据类 / record
来源：http://yb.jianghongdianzi.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ky.nicolike.cn

PHP:  // 用 readonly 属性模拟
来源：http://wh.asd995.cn

JS:   // 无内置：普通类或对象字面量
来源：http://wz.colortex.cn

TS:   type User = { name: string; age: number };
来源：http://bu.szsharing.cn

Java: record User(String name, int age) {}
来源：http://yq.colortex.cn

Go:   type User struct { Name string; Age int }
来源：http://me.colortex.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://pt.newstarts.cn

C#:   record User(string Name, int Age);
来源：http://nx.wgjwhj.cn

[G15] 枚举
来源：http://ip.lnxyls.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wc.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://rj.jianghongdianzi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lr.yuntaijiaju.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://cy.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://rk.nszjky.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://qz.chemitech.net.cn

Ruby: Color = %i[red green].freeze
来源：http://ez.hnjuh.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sy.newstarts.cn

[G16] 对象转数组 / 字典
来源：http://vn.szsharing.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://pi.chemitech.net.cn

PHP:  get_object_vars($obj);
来源：http://qz.asd995.cn

JS:   Object.entries(obj)
来源：http://wz.colortex.cn

TS:   Object.entries(obj)
来源：http://er.wgjwhj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://je.huixiangedu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://ph.lnxyls.cn

Ruby: obj.instance_variables
来源：http://ac.muxihuayi.cn

C#:   // 用反射或 System.Text.Json
来源：http://mj.jctech888.com.cn

================================================================================
来源：http://mc.jianghongdianzi.cn

H. 异常与错误处理
来源：http://so.szsharing.cn

================================================================================
来源：http://ms.bookmarksfly.cn

[H01] try / catch 基础
来源：http://kl.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ur.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://is.haigaiapp.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bv.chemitech.net.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vh.hahajie.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://yz.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://lh.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ad.panjiajie.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://le.shxzukj.cn

[H02] finally / ensure 收尾
来源：http://ko.9csxet.cn

Py:   try: f()⏎finally: cleanup()
来源：http://bz.9csxet.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://al.hnjuh.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://ci.jctech888.com.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ww.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ye.jctech888.com.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yy.panjiajie.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://wk.huixiangedu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://ao.hnjuh.cn

[H03] 主动抛出异常
来源：http://zd.yuntaijiaju.cn

Py:   raise ValueError("错误信息")
来源：http://lz.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ge.nszjky.cn

JS:   throw new Error("错误信息");
来源：http://og.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://zw.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://da.huixiangedu.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ty.yuexingan06.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://zz.huanxung.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zs.muxihuayi.cn

[H04] 自定义异常类型
来源：http://jc.chemitech.net.cn

Py:   class MyError(Exception): pass
来源：http://mq.huixiangedu.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gu.colortex.cn


<!-- 参考信息 -->