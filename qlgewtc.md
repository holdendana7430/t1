代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://nz.chemitech.net.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xc.shtwfgs.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://tj.nszjky.cn

Ruby: s.bytesize;  s.length
来源：http://xn.jianghongdianzi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://uf.wgjwhj.cn

================================================================================
来源：http://kx.jctech888.com.cn

F. 文件与目录
来源：http://qp.chemitech.net.cn

================================================================================
来源：http://db.hnjuh.cn

[F01] 读取整个文件
来源：http://on.hahajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://tw.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://ap.gzmigu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hc.shxzskj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wy.shxzskj.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://up.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://nc.lnxyls.cn

Ruby: File.read("a.txt")
来源：http://vz.szsharing.cn

C#:   File.ReadAllText("a.txt");
来源：http://my.jctech888.com.cn

[F02] 逐行读取文件
来源：http://us.huixiangedu.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://zz.wgjwhj.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://fx.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jp.hnjuh.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ss.jianghongdianzi.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://sf.wgjwhj.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://lj.huixinmuqiang.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://of.shxzskj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://au.521024.cn

[F03] 写入文件（覆盖）
来源：http://pp.chemitech.net.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://qm.muxihuayi.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://uz.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qq.jianghongdianzi.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ki.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ys.lnxyls.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wh.colortex.cn

Ruby: File.write("a.txt", "hi")
来源：http://ho.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://vk.wgjwhj.cn

[F04] 追加写入文件
来源：http://eb.huanxung.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ka.nszjky.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://zm.bookmarksfly.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gn.panjiajie.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ou.hahajie.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://og.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://eo.huanxung.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wf.gzmigu.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wj.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://ub.huixinmuqiang.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jf.muxihuayi.cn

PHP:  file_exists("a.txt");
来源：http://bp.shxzukj.cn

JS:   fs.existsSync("a.txt")
来源：http://kn.shxzukj.cn

TS:   fs.existsSync("a.txt")
来源：http://vm.yuntaijiaju.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://qr.jianghongdianzi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://cl.hahajie.cn

Ruby: File.exist?("a.txt")
来源：http://kq.szxytkj.cn

C#:   File.Exists("a.txt")
来源：http://hl.yuntaijiaju.cn

[F06] 删除文件
来源：http://ol.bookmarksfly.cn

Py:   os.remove("a.txt")
来源：http://ec.shtwfgs.cn

PHP:  unlink("a.txt");
来源：http://gp.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://oq.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ix.yuexingan06.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mt.hnjuh.cn

Go:   os.Remove("a.txt")
来源：http://aa.hahajie.cn

Ruby: File.delete("a.txt")
来源：http://my.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://ft.huanxung.cn

[F07] 创建目录（含多级）
来源：http://bn.haigaiapp.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ra.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://lk.newstarts.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://dt.bjjhwx.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://rq.bjjhwx.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://id.shxzskj.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://nv.colortex.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rc.9csxet.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://dc.szsharing.cn

[F08] 遍历目录
来源：http://vy.colortex.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ea.521024.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ge.bookmarksfly.cn

JS:   fs.readdirSync("dir")
来源：http://vn.bookmarksfly.cn

TS:   fs.readdirSync("dir")
来源：http://ss.hnjuh.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://of.muxihuayi.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://bz.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://nr.nicolike.cn

C#:   Directory.GetFiles("dir")
来源：http://cd.hnjuh.cn

[F09] 获取文件大小
来源：http://fd.szxytkj.cn

Py:   os.path.getsize("a.txt")
来源：http://no.newstarts.cn

PHP:  filesize("a.txt");
来源：http://nz.nszjky.cn

JS:   fs.statSync("a.txt").size
来源：http://gx.panjiajie.cn

TS:   fs.statSync("a.txt").size
来源：http://pa.shxzukj.cn

Java: Files.size(Path.of("a.txt"))
来源：http://je.huixiangedu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://pl.panjiajie.cn

Ruby: File.size("a.txt")
来源：http://xw.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://nz.bjjhwx.cn

[F10] 取文件扩展名 / 文件名
来源：http://zh.hahajie.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://ih.shtwfgs.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wh.bjjhwx.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ju.colortex.cn

TS:   path.extname("a.txt")
来源：http://uo.hahajie.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://vm.nicolike.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ud.chemitech.net.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://ww.huixiangedu.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mw.nszjky.cn

[F11] 复制与移动文件
来源：http://al.muxihuayi.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ui.jctech888.com.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ko.521024.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://bp.shxzukj.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://gx.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ox.jctech888.com.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ih.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://oe.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://re.nicolike.cn

[F12] CSV 读写
来源：http://kp.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://eo.asd995.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://lb.shtwfgs.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ui.chemitech.net.cn

TS:   // 同上
来源：http://rf.lnxyls.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://do.szxytkj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://sl.521024.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://lv.asd995.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://up.muxihuayi.cn

================================================================================
来源：http://iv.jctech888.com.cn

G. 面向对象
来源：http://ad.gzmigu.cn

================================================================================
来源：http://if.shxzukj.cn

[G01] 定义类
来源：http://fd.gzmigu.cn

Py:   class User: pass
来源：http://rb.huanxung.cn

PHP:  class User {}
来源：http://vq.huixiangedu.cn

JS:   class User {}
来源：http://ux.9csxet.cn

TS:   class User { name: string = ""; }
来源：http://sr.muxihuayi.cn

Java: class User {}
来源：http://du.panjiajie.cn

Go:   type User struct { Name string }
来源：http://dc.bjjhwx.cn

Ruby: class User; end
来源：http://fk.chemitech.net.cn

C#:   class User {}
来源：http://lq.haigaiapp.cn

[G02] 构造函数
来源：http://vq.jianghongdianzi.cn

Py:   def __init__(self, name): self.name = name
来源：http://kx.panjiajie.cn

PHP:  public function __construct(public string $name) {}
来源：http://ci.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://qb.bjjhwx.cn

TS:   constructor(public name: string) {}
来源：http://si.chemitech.net.cn

Java: User(String name) { this.name = name; }
来源：http://vn.szxytkj.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://lq.newstarts.cn

Ruby: def initialize(name); @name = name; end
来源：http://zl.shxzskj.cn

C#:   public User(string name) { Name = name; }
来源：http://gi.nicolike.cn

[G03] 实例属性
来源：http://xp.panjiajie.cn

Py:   self.name = "x"
来源：http://bt.521024.cn

PHP:  public string $name = "x";
来源：http://mg.wgjwhj.cn

JS:   this.name = "x";
来源：http://er.lnxyls.cn

TS:   name: string = "x";
来源：http://wo.asd995.cn

Java: private String name;
来源：http://bj.bookmarksfly.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://rw.huixiangedu.cn

Ruby: @name = "x"
来源：http://mu.hnjuh.cn

C#:   public string Name { get; set; } = "x";
来源：http://vq.panjiajie.cn

[G04] 定义方法
来源：http://fz.haigaiapp.cn

Py:   def greet(self): return self.name
来源：http://nr.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://dm.jianghongdianzi.cn

JS:   greet() { return this.name; }
来源：http://ua.bookmarksfly.cn

TS:   greet(): string { return this.name; }
来源：http://ec.nszjky.cn

Java: String greet() { return name; }
来源：http://fl.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://hv.chemitech.net.cn

Ruby: def greet; @name; end
来源：http://dq.hahajie.cn

C#:   public string Greet() => Name;
来源：http://tr.huanxung.cn

[G05] 继承
来源：http://rz.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://gi.panjiajie.cn

PHP:  class Admin extends User {}
来源：http://ic.9csxet.cn

JS:   class Admin extends User {}
来源：http://lh.szxytkj.cn

TS:   class Admin extends User {}
来源：http://al.wgjwhj.cn

Java: class Admin extends User {}
来源：http://jq.shxzskj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://ip.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://lm.jctech888.com.cn

C#:   class Admin : User {}
来源：http://em.bjjhwx.cn

[G06] 重写方法
来源：http://gb.lnxyls.cn

Py:   def greet(self): return "admin"
来源：http://fc.shtwfgs.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dt.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ip.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://sl.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://ov.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://je.hnjuh.cn

Ruby: def greet; "admin"; end
来源：http://lr.huixinmuqiang.cn

C#:   public override string Greet() => "admin";
来源：http://ur.shtwfgs.cn

[G07] 调用父类方法
来源：http://oe.panjiajie.cn

Py:   super().greet()
来源：http://ma.gzmigu.cn

PHP:  parent::greet();
来源：http://dc.nicolike.cn

JS:   super.greet();
来源：http://un.muxihuayi.cn

TS:   super.greet();
来源：http://vg.wgjwhj.cn

Java: super.greet();
来源：http://xe.haigaiapp.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://yk.521024.cn

Ruby: super
来源：http://og.muxihuayi.cn

C#:   base.Greet();
来源：http://cv.nicolike.cn

[G08] 静态方法与属性
来源：http://pg.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://lf.shxzukj.cn

PHP:  public static function f() {}
来源：http://aa.hahajie.cn

JS:   static f() {}
来源：http://xr.yuexingan06.cn

TS:   static f(): void {}
来源：http://dt.bookmarksfly.cn

Java: static void f() {}
来源：http://jt.panjiajie.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://ks.newstarts.cn

Ruby: def self.f; end
来源：http://cw.szsharing.cn

C#:   public static void F() {}
来源：http://le.521024.cn

[G09] 接口 / 抽象类
来源：http://yx.nicolike.cn

Py:   from abc import ABC, abstractmethod
来源：http://gv.szsharing.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ym.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://eg.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://wu.shxzukj.cn

Java: interface Shape { double area(); }
来源：http://iw.colortex.cn

Go:   type Shape interface { Area() float64 }
来源：http://dc.muxihuayi.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ww.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://bg.shxzukj.cn

[G10] 访问控制
来源：http://hu.huixinmuqiang.cn

Py:   约定 _protected / __private（不强制）
来源：http://xv.gzmigu.cn

PHP:  public / protected / private
来源：http://zs.huixinmuqiang.cn

JS:   #private 字段；其余公开
来源：http://bm.jianghongdianzi.cn

TS:   public / protected / private
来源：http://ml.bookmarksfly.cn

Java: public / protected / private / 默认包级
来源：http://tk.szsharing.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://uq.wgjwhj.cn

Ruby: public / protected / private
来源：http://mc.9csxet.cn

C#:   public / protected / private / internal
来源：http://qk.bjjhwx.cn

[G11] getter / setter
来源：http://jm.huixiangedu.cn

Py:   @property 与 @x.setter
来源：http://lw.jctech888.com.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ca.wgjwhj.cn

JS:   get name() { return this._name; }
来源：http://te.asd995.cn

TS:   get name(): string { return this._name; }
来源：http://vq.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://gt.shxzukj.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://qv.nszjky.cn

Ruby: attr_accessor :name
来源：http://gz.shxzskj.cn

C#:   public string Name { get; set; }
来源：http://yi.nszjky.cn

[G12] 对象转字符串
来源：http://eo.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://ft.521024.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://te.newstarts.cn

JS:   toString() { return this.name; }
来源：http://pk.wgjwhj.cn

TS:   toString(): string { return this.name; }
来源：http://cp.colortex.cn

Java: @Override public String toString() { return name; }
来源：http://ij.shxzukj.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ni.newstarts.cn

Ruby: def to_s; @name; end
来源：http://qf.haigaiapp.cn

C#:   public override string ToString() => Name;
来源：http://dy.muxihuayi.cn

[G13] 判断对象类型
来源：http://sj.bookmarksfly.cn

Py:   isinstance(u, User)
来源：http://id.nszjky.cn

PHP:  $u instanceof User
来源：http://iw.9csxet.cn

JS:   u instanceof User
来源：http://si.shxzskj.cn

TS:   u instanceof User
来源：http://nt.jianghongdianzi.cn

Java: u instanceof User
来源：http://pz.szsharing.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://xv.shxzukj.cn

Ruby: u.is_a?(User)
来源：http://yo.szxytkj.cn

C#:   u is User
来源：http://gt.yuntaijiaju.cn

[G14] 数据类 / record
来源：http://vu.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mx.521024.cn

PHP:  // 用 readonly 属性模拟
来源：http://kl.haigaiapp.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zg.panjiajie.cn

TS:   type User = { name: string; age: number };
来源：http://oz.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://cg.szsharing.cn

Go:   type User struct { Name string; Age int }
来源：http://ys.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://nl.9csxet.cn

C#:   record User(string Name, int Age);
来源：http://cg.muxihuayi.cn

[G15] 枚举
来源：http://jw.haigaiapp.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://ex.521024.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ki.bjjhwx.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sz.shxzukj.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://it.shxzukj.cn

Java: enum Color { RED, GREEN }
来源：http://di.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://tz.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://xo.huixiangedu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://oj.huixiangedu.cn

[G16] 对象转数组 / 字典
来源：http://zt.jianghongdianzi.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fw.bookmarksfly.cn

PHP:  get_object_vars($obj);
来源：http://xb.jianghongdianzi.cn

JS:   Object.entries(obj)
来源：http://rh.muxihuayi.cn

TS:   Object.entries(obj)
来源：http://vn.9csxet.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tu.shxzskj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cq.huixiangedu.cn

Ruby: obj.instance_variables
来源：http://nl.521024.cn

C#:   // 用反射或 System.Text.Json
来源：http://yi.jianghongdianzi.cn

================================================================================
来源：http://kj.yuexingan06.cn

H. 异常与错误处理
来源：http://de.shxzskj.cn

================================================================================
来源：http://jf.bookmarksfly.cn

[H01] try / catch 基础
来源：http://fl.colortex.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hk.haigaiapp.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://cp.nicolike.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ne.yuexingan06.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ar.shxzukj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xv.521024.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yu.bookmarksfly.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://nv.bookmarksfly.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jx.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ve.shxzukj.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ln.hahajie.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://ob.9csxet.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://px.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://js.jianghongdianzi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://xj.bjjhwx.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://om.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://qv.panjiajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://pt.szsharing.cn

[H03] 主动抛出异常
来源：http://jk.szsharing.cn

Py:   raise ValueError("错误信息")
来源：http://du.shxzukj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://ya.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://tt.hahajie.cn

TS:   throw new Error("错误信息");
来源：http://bd.nszjky.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://lp.yuntaijiaju.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ao.haigaiapp.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://wv.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ux.9csxet.cn

[H04] 自定义异常类型
来源：http://hm.bjjhwx.cn

Py:   class MyError(Exception): pass
来源：http://xy.haigaiapp.cn

PHP:  class MyError extends RuntimeException {}
来源：http://sc.muxihuayi.cn

JS:   class MyError extends Error {}
来源：http://px.bookmarksfly.cn

TS:   class MyError extends Error {}
来源：http://nk.hnjuh.cn

Java: class MyException extends RuntimeException {}
来源：http://vg.lnxyls.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://eb.asd995.cn


<!-- 参考信息 -->