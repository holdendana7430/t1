代发 wailian999

[E22] 字节长度与字符长度
来源：http://ix.huanxung.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hh.muxihuayi.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cu.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://jo.chemitech.net.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://vu.jianghongdianzi.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ob.huanxung.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://oy.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://bn.colortex.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hf.hahajie.cn

================================================================================
来源：http://gl.huixinmuqiang.cn

F. 文件与目录
来源：http://ai.chemitech.net.cn

================================================================================
来源：http://pr.hnjuh.cn

[F01] 读取整个文件
来源：http://zc.panjiajie.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://el.bjjhwx.cn

PHP:  file_get_contents("a.txt");
来源：http://rr.9csxet.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://qv.bjjhwx.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://gr.huanxung.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dx.hahajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://de.huixiangedu.cn

Ruby: File.read("a.txt")
来源：http://dv.shxzskj.cn

C#:   File.ReadAllText("a.txt");
来源：http://pn.nicolike.cn

[F02] 逐行读取文件
来源：http://bo.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://bp.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tc.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://gp.muxihuayi.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://cd.gzmigu.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://cm.haigaiapp.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ht.gzmigu.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://jx.hnjuh.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ec.yuntaijiaju.cn

[F03] 写入文件（覆盖）
来源：http://ej.yuexingan06.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://cb.9csxet.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://hv.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://bv.9csxet.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://yk.bjjhwx.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://la.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://cj.hnjuh.cn

Ruby: File.write("a.txt", "hi")
来源：http://wi.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hk.lnxyls.cn

[F04] 追加写入文件
来源：http://wo.521024.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://kv.shxzukj.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://cx.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://au.asd995.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://kq.chemitech.net.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://jz.panjiajie.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://fn.yuexingan06.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://nf.yuntaijiaju.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ch.bjjhwx.cn

[F05] 判断文件或目录是否存在
来源：http://qr.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://lc.9csxet.cn

PHP:  file_exists("a.txt");
来源：http://qn.hahajie.cn

JS:   fs.existsSync("a.txt")
来源：http://ek.nicolike.cn

TS:   fs.existsSync("a.txt")
来源：http://fu.nicolike.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dk.panjiajie.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mp.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://nq.chemitech.net.cn

C#:   File.Exists("a.txt")
来源：http://vn.nszjky.cn

[F06] 删除文件
来源：http://eg.szsharing.cn

Py:   os.remove("a.txt")
来源：http://fv.9csxet.cn

PHP:  unlink("a.txt");
来源：http://en.bookmarksfly.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xx.nicolike.cn

TS:   fs.unlinkSync("a.txt")
来源：http://pl.jianghongdianzi.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://tk.gzmigu.cn

Go:   os.Remove("a.txt")
来源：http://dt.yuexingan06.cn

Ruby: File.delete("a.txt")
来源：http://wq.yuexingan06.cn

C#:   File.Delete("a.txt");
来源：http://mb.muxihuayi.cn

[F07] 创建目录（含多级）
来源：http://ny.shxzukj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wj.chemitech.net.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://rz.wgjwhj.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gn.chemitech.net.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ax.shtwfgs.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tw.yuexingan06.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://gh.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://jg.huixinmuqiang.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://xu.bjjhwx.cn

[F08] 遍历目录
来源：http://wm.hnjuh.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://fi.shxzukj.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ij.shxzskj.cn

JS:   fs.readdirSync("dir")
来源：http://mh.gzmigu.cn

TS:   fs.readdirSync("dir")
来源：http://ax.shxzskj.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://li.chemitech.net.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://wp.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://wd.lnxyls.cn

C#:   Directory.GetFiles("dir")
来源：http://wl.shtwfgs.cn

[F09] 获取文件大小
来源：http://rh.yuntaijiaju.cn

Py:   os.path.getsize("a.txt")
来源：http://ci.9csxet.cn

PHP:  filesize("a.txt");
来源：http://zb.shtwfgs.cn

JS:   fs.statSync("a.txt").size
来源：http://lv.bjjhwx.cn

TS:   fs.statSync("a.txt").size
来源：http://zt.jctech888.com.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ml.wgjwhj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://yg.yuntaijiaju.cn

Ruby: File.size("a.txt")
来源：http://ow.huixinmuqiang.cn

C#:   new FileInfo("a.txt").Length
来源：http://qo.chemitech.net.cn

[F10] 取文件扩展名 / 文件名
来源：http://ar.nszjky.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://db.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://rx.huixiangedu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://oa.asd995.cn

TS:   path.extname("a.txt")
来源：http://dp.nszjky.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://cg.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zx.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jz.muxihuayi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://gf.yuexingan06.cn

[F11] 复制与移动文件
来源：http://oj.bookmarksfly.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://fc.hahajie.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://sd.szsharing.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://zv.bookmarksfly.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ri.jianghongdianzi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://io.panjiajie.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://kx.shxzukj.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://er.huixinmuqiang.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://kb.nszjky.cn

[F12] CSV 读写
来源：http://tz.newstarts.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jl.huanxung.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ub.colortex.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ii.muxihuayi.cn

TS:   // 同上
来源：http://ts.nicolike.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://ud.wgjwhj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://dc.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ur.shtwfgs.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://sd.szsharing.cn

================================================================================
来源：http://cz.jianghongdianzi.cn

G. 面向对象
来源：http://ed.shxzskj.cn

================================================================================
来源：http://jr.szxytkj.cn

[G01] 定义类
来源：http://rw.shtwfgs.cn

Py:   class User: pass
来源：http://wa.huanxung.cn

PHP:  class User {}
来源：http://fd.hahajie.cn

JS:   class User {}
来源：http://jv.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://lc.nszjky.cn

Java: class User {}
来源：http://om.panjiajie.cn

Go:   type User struct { Name string }
来源：http://rj.shtwfgs.cn

Ruby: class User; end
来源：http://ez.colortex.cn

C#:   class User {}
来源：http://sj.jctech888.com.cn

[G02] 构造函数
来源：http://lg.shtwfgs.cn

Py:   def __init__(self, name): self.name = name
来源：http://eq.chemitech.net.cn

PHP:  public function __construct(public string $name) {}
来源：http://vv.wgjwhj.cn

JS:   constructor(name) { this.name = name; }
来源：http://bb.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://ji.shxzskj.cn

Java: User(String name) { this.name = name; }
来源：http://vu.asd995.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://tf.bookmarksfly.cn

Ruby: def initialize(name); @name = name; end
来源：http://sn.bjjhwx.cn

C#:   public User(string name) { Name = name; }
来源：http://hj.asd995.cn

[G03] 实例属性
来源：http://mj.hahajie.cn

Py:   self.name = "x"
来源：http://db.muxihuayi.cn

PHP:  public string $name = "x";
来源：http://mf.szsharing.cn

JS:   this.name = "x";
来源：http://wg.muxihuayi.cn

TS:   name: string = "x";
来源：http://nq.shtwfgs.cn

Java: private String name;
来源：http://sb.huixinmuqiang.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://xp.huixinmuqiang.cn

Ruby: @name = "x"
来源：http://rj.chemitech.net.cn

C#:   public string Name { get; set; } = "x";
来源：http://ml.huanxung.cn

[G04] 定义方法
来源：http://kb.szxytkj.cn

Py:   def greet(self): return self.name
来源：http://rt.wgjwhj.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bw.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://pk.haigaiapp.cn

TS:   greet(): string { return this.name; }
来源：http://wh.jianghongdianzi.cn

Java: String greet() { return name; }
来源：http://wp.gzmigu.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://se.yuexingan06.cn

Ruby: def greet; @name; end
来源：http://vi.chemitech.net.cn

C#:   public string Greet() => Name;
来源：http://cg.jianghongdianzi.cn

[G05] 继承
来源：http://ls.shxzukj.cn

Py:   class Admin(User): pass
来源：http://ph.asd995.cn

PHP:  class Admin extends User {}
来源：http://yg.huanxung.cn

JS:   class Admin extends User {}
来源：http://ba.nicolike.cn

TS:   class Admin extends User {}
来源：http://zc.jianghongdianzi.cn

Java: class Admin extends User {}
来源：http://pi.jctech888.com.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mj.521024.cn

Ruby: class Admin < User; end
来源：http://lj.muxihuayi.cn

C#:   class Admin : User {}
来源：http://ju.newstarts.cn

[G06] 重写方法
来源：http://fv.shxzskj.cn

Py:   def greet(self): return "admin"
来源：http://yg.shxzskj.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://zk.bookmarksfly.cn

JS:   greet() { return "admin"; }
来源：http://vy.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://cw.jianghongdianzi.cn

Java: @Override String greet() { return "admin"; }
来源：http://qw.nszjky.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yf.chemitech.net.cn

Ruby: def greet; "admin"; end
来源：http://xw.bookmarksfly.cn

C#:   public override string Greet() => "admin";
来源：http://do.hahajie.cn

[G07] 调用父类方法
来源：http://ju.yuexingan06.cn

Py:   super().greet()
来源：http://qq.shxzskj.cn

PHP:  parent::greet();
来源：http://xi.nicolike.cn

JS:   super.greet();
来源：http://md.yuntaijiaju.cn

TS:   super.greet();
来源：http://py.szxytkj.cn

Java: super.greet();
来源：http://le.huixinmuqiang.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gx.wgjwhj.cn

Ruby: super
来源：http://pm.521024.cn

C#:   base.Greet();
来源：http://eu.521024.cn

[G08] 静态方法与属性
来源：http://ku.shxzukj.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://pa.hahajie.cn

PHP:  public static function f() {}
来源：http://kj.bookmarksfly.cn

JS:   static f() {}
来源：http://zj.wgjwhj.cn

TS:   static f(): void {}
来源：http://tx.gzmigu.cn

Java: static void f() {}
来源：http://cx.asd995.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://xr.muxihuayi.cn

Ruby: def self.f; end
来源：http://mm.nszjky.cn

C#:   public static void F() {}
来源：http://og.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://tq.panjiajie.cn

Py:   from abc import ABC, abstractmethod
来源：http://kp.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://zj.szxytkj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://qy.yuntaijiaju.cn

TS:   interface Shape { area(): number; }
来源：http://ye.szsharing.cn

Java: interface Shape { double area(); }
来源：http://od.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://hm.521024.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://yg.nszjky.cn

C#:   interface IShape { double Area(); }
来源：http://ap.jianghongdianzi.cn

[G10] 访问控制
来源：http://cu.shtwfgs.cn

Py:   约定 _protected / __private（不强制）
来源：http://jr.szsharing.cn

PHP:  public / protected / private
来源：http://yr.gzmigu.cn

JS:   #private 字段；其余公开
来源：http://iz.shxzukj.cn

TS:   public / protected / private
来源：http://zm.yuntaijiaju.cn

Java: public / protected / private / 默认包级
来源：http://fj.szxytkj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://dz.lnxyls.cn

Ruby: public / protected / private
来源：http://zn.bookmarksfly.cn

C#:   public / protected / private / internal
来源：http://ae.jianghongdianzi.cn

[G11] getter / setter
来源：http://zj.lnxyls.cn

Py:   @property 与 @x.setter
来源：http://tu.lnxyls.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://uk.9csxet.cn

JS:   get name() { return this._name; }
来源：http://qz.szsharing.cn

TS:   get name(): string { return this._name; }
来源：http://wh.szsharing.cn

Java: public String getName() { return name; }
来源：http://rd.yuexingan06.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://ra.shxzukj.cn

Ruby: attr_accessor :name
来源：http://yc.shtwfgs.cn

C#:   public string Name { get; set; }
来源：http://ah.yuntaijiaju.cn

[G12] 对象转字符串
来源：http://kw.yuexingan06.cn

Py:   def __str__(self): return self.name
来源：http://zs.gzmigu.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wj.szsharing.cn

JS:   toString() { return this.name; }
来源：http://fz.muxihuayi.cn

TS:   toString(): string { return this.name; }
来源：http://hk.521024.cn

Java: @Override public String toString() { return name; }
来源：http://qo.colortex.cn

Go:   func (u User) String() string { return u.Name }
来源：http://fj.shxzukj.cn

Ruby: def to_s; @name; end
来源：http://zi.yuntaijiaju.cn

C#:   public override string ToString() => Name;
来源：http://mx.bookmarksfly.cn

[G13] 判断对象类型
来源：http://du.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://hs.muxihuayi.cn

PHP:  $u instanceof User
来源：http://ti.shxzskj.cn

JS:   u instanceof User
来源：http://cb.colortex.cn

TS:   u instanceof User
来源：http://sb.asd995.cn

Java: u instanceof User
来源：http://re.lnxyls.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://lk.bjjhwx.cn

Ruby: u.is_a?(User)
来源：http://qv.lnxyls.cn

C#:   u is User
来源：http://pj.hahajie.cn

[G14] 数据类 / record
来源：http://im.yuntaijiaju.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ho.lnxyls.cn

PHP:  // 用 readonly 属性模拟
来源：http://ip.shtwfgs.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ts.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://jg.jctech888.com.cn

Java: record User(String name, int age) {}
来源：http://aj.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://fc.huixiangedu.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fr.shxzskj.cn

C#:   record User(string Name, int Age);
来源：http://pe.haigaiapp.cn

[G15] 枚举
来源：http://ee.asd995.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://xt.yuexingan06.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lk.muxihuayi.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://tc.shtwfgs.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://di.panjiajie.cn

Java: enum Color { RED, GREEN }
来源：http://ux.jianghongdianzi.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ie.panjiajie.cn

Ruby: Color = %i[red green].freeze
来源：http://av.gzmigu.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://bf.yuexingan06.cn

[G16] 对象转数组 / 字典
来源：http://xc.shxzukj.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ij.szxytkj.cn

PHP:  get_object_vars($obj);
来源：http://gx.haigaiapp.cn

JS:   Object.entries(obj)
来源：http://ut.hahajie.cn

TS:   Object.entries(obj)
来源：http://gs.szxytkj.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://cj.shxzukj.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://hs.jianghongdianzi.cn

Ruby: obj.instance_variables
来源：http://zh.hahajie.cn

C#:   // 用反射或 System.Text.Json
来源：http://gx.szsharing.cn

================================================================================
来源：http://pr.chemitech.net.cn

H. 异常与错误处理
来源：http://zz.bookmarksfly.cn

================================================================================
来源：http://uw.szsharing.cn

[H01] try / catch 基础
来源：http://bc.shxzskj.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://gd.bjjhwx.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://if.shxzskj.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://lo.nicolike.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://xs.hnjuh.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qr.huanxung.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://uy.shtwfgs.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://vy.huixiangedu.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://np.haigaiapp.cn

[H02] finally / ensure 收尾
来源：http://el.jianghongdianzi.cn

Py:   try: f()⏎finally: cleanup()
来源：http://eu.huixinmuqiang.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://nz.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yr.gzmigu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ux.nszjky.cn

Java: try { f(); } finally { cleanup(); }
来源：http://bn.newstarts.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://us.huanxung.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://on.asd995.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://zp.szxytkj.cn

[H03] 主动抛出异常
来源：http://zj.nszjky.cn

Py:   raise ValueError("错误信息")
来源：http://rc.hnjuh.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://vf.szsharing.cn

JS:   throw new Error("错误信息");
来源：http://me.chemitech.net.cn

TS:   throw new Error("错误信息");
来源：http://pq.hahajie.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://rw.shxzskj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cg.gzmigu.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://dc.muxihuayi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rf.szsharing.cn

[H04] 自定义异常类型
来源：http://hg.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://co.jctech888.com.cn

PHP:  class MyError extends RuntimeException {}
来源：http://eq.szxytkj.cn


<!-- 参考信息 -->