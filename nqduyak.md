代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://tl.panjiajie.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://xj.bjjhwx.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wz.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://hn.yuntaijiaju.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lz.yuexingan06.cn

================================================================================
来源：http://lb.chemitech.net.cn

F. 文件与目录
来源：http://of.yuexingan06.cn

================================================================================
来源：http://qr.yuexingan06.cn

[F01] 读取整个文件
来源：http://mn.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://ms.nszjky.cn

PHP:  file_get_contents("a.txt");
来源：http://vy.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ow.hnjuh.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bm.asd995.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://lb.szxytkj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://rm.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://wk.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://ki.shxzukj.cn

[F02] 逐行读取文件
来源：http://zu.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://gl.yuntaijiaju.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hg.nszjky.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://fd.colortex.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://sz.shxzskj.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://jm.gzmigu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ne.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://zb.9csxet.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ah.521024.cn

[F03] 写入文件（覆盖）
来源：http://oj.bookmarksfly.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://pf.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://em.hnjuh.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://xt.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://kq.newstarts.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://lk.chemitech.net.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://ce.wgjwhj.cn

Ruby: File.write("a.txt", "hi")
来源：http://eg.bookmarksfly.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://qa.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://dx.muxihuayi.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://nb.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://pp.newstarts.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zs.shtwfgs.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wk.haigaiapp.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ea.lnxyls.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://xb.panjiajie.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://io.lnxyls.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://rt.shtwfgs.cn

[F05] 判断文件或目录是否存在
来源：http://cg.yuexingan06.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://jt.huixinmuqiang.cn

PHP:  file_exists("a.txt");
来源：http://la.bookmarksfly.cn

JS:   fs.existsSync("a.txt")
来源：http://tc.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://wr.haigaiapp.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://dj.colortex.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://oh.huixinmuqiang.cn

Ruby: File.exist?("a.txt")
来源：http://vw.newstarts.cn

C#:   File.Exists("a.txt")
来源：http://de.szxytkj.cn

[F06] 删除文件
来源：http://nr.521024.cn

Py:   os.remove("a.txt")
来源：http://sn.yuntaijiaju.cn

PHP:  unlink("a.txt");
来源：http://sb.shxzukj.cn

JS:   fs.unlinkSync("a.txt")
来源：http://cl.shxzskj.cn

TS:   fs.unlinkSync("a.txt")
来源：http://cs.nicolike.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://sq.huanxung.cn

Go:   os.Remove("a.txt")
来源：http://ec.jctech888.com.cn

Ruby: File.delete("a.txt")
来源：http://to.gzmigu.cn

C#:   File.Delete("a.txt");
来源：http://uw.huixinmuqiang.cn

[F07] 创建目录（含多级）
来源：http://rk.9csxet.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://ov.newstarts.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://pz.gzmigu.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zf.shtwfgs.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://jn.shxzukj.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ju.huixinmuqiang.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hq.huixinmuqiang.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://rj.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://me.gzmigu.cn

[F08] 遍历目录
来源：http://oq.521024.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://ay.haigaiapp.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lh.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://jf.hahajie.cn

TS:   fs.readdirSync("dir")
来源：http://rt.szsharing.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://dh.szsharing.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://jd.bjjhwx.cn

Ruby: Dir.children("dir")
来源：http://vy.panjiajie.cn

C#:   Directory.GetFiles("dir")
来源：http://cf.colortex.cn

[F09] 获取文件大小
来源：http://sy.wgjwhj.cn

Py:   os.path.getsize("a.txt")
来源：http://vq.shxzskj.cn

PHP:  filesize("a.txt");
来源：http://fv.colortex.cn

JS:   fs.statSync("a.txt").size
来源：http://nr.shtwfgs.cn

TS:   fs.statSync("a.txt").size
来源：http://bg.asd995.cn

Java: Files.size(Path.of("a.txt"))
来源：http://nb.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://nh.jianghongdianzi.cn

Ruby: File.size("a.txt")
来源：http://rx.chemitech.net.cn

C#:   new FileInfo("a.txt").Length
来源：http://rc.lnxyls.cn

[F10] 取文件扩展名 / 文件名
来源：http://ku.szxytkj.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://vp.9csxet.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://gl.gzmigu.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://ei.huixiangedu.cn

TS:   path.extname("a.txt")
来源：http://bg.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ga.shtwfgs.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://ob.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://jm.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://zg.yuexingan06.cn

[F11] 复制与移动文件
来源：http://lp.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://uw.yuexingan06.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://yj.panjiajie.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://rv.yuntaijiaju.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://oq.huanxung.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://bm.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://yk.huixiangedu.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://io.newstarts.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ub.newstarts.cn

[F12] CSV 读写
来源：http://ck.jctech888.com.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://he.shxzukj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://es.nicolike.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://kq.haigaiapp.cn

TS:   // 同上
来源：http://gs.huanxung.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://tu.asd995.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wg.yuntaijiaju.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mo.colortex.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://pu.huanxung.cn

================================================================================
来源：http://yb.yuntaijiaju.cn

G. 面向对象
来源：http://bk.szsharing.cn

================================================================================
来源：http://zu.bjjhwx.cn

[G01] 定义类
来源：http://ct.lnxyls.cn

Py:   class User: pass
来源：http://og.bjjhwx.cn

PHP:  class User {}
来源：http://fe.colortex.cn

JS:   class User {}
来源：http://sp.haigaiapp.cn

TS:   class User { name: string = ""; }
来源：http://la.jianghongdianzi.cn

Java: class User {}
来源：http://cj.lnxyls.cn

Go:   type User struct { Name string }
来源：http://iu.gzmigu.cn

Ruby: class User; end
来源：http://jp.newstarts.cn

C#:   class User {}
来源：http://yf.chemitech.net.cn

[G02] 构造函数
来源：http://gj.nszjky.cn

Py:   def __init__(self, name): self.name = name
来源：http://yz.szxytkj.cn

PHP:  public function __construct(public string $name) {}
来源：http://za.colortex.cn

JS:   constructor(name) { this.name = name; }
来源：http://rx.panjiajie.cn

TS:   constructor(public name: string) {}
来源：http://fy.bookmarksfly.cn

Java: User(String name) { this.name = name; }
来源：http://fr.huanxung.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://pd.9csxet.cn

Ruby: def initialize(name); @name = name; end
来源：http://ha.hahajie.cn

C#:   public User(string name) { Name = name; }
来源：http://ih.huixinmuqiang.cn

[G03] 实例属性
来源：http://dr.chemitech.net.cn

Py:   self.name = "x"
来源：http://gf.yuntaijiaju.cn

PHP:  public string $name = "x";
来源：http://ic.yuexingan06.cn

JS:   this.name = "x";
来源：http://wp.gzmigu.cn

TS:   name: string = "x";
来源：http://xm.szsharing.cn

Java: private String name;
来源：http://if.wgjwhj.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://cq.521024.cn

Ruby: @name = "x"
来源：http://eg.huixinmuqiang.cn

C#:   public string Name { get; set; } = "x";
来源：http://ei.nszjky.cn

[G04] 定义方法
来源：http://oi.colortex.cn

Py:   def greet(self): return self.name
来源：http://gu.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://zr.chemitech.net.cn

JS:   greet() { return this.name; }
来源：http://fp.asd995.cn

TS:   greet(): string { return this.name; }
来源：http://iq.nicolike.cn

Java: String greet() { return name; }
来源：http://fg.bookmarksfly.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://mc.hnjuh.cn

Ruby: def greet; @name; end
来源：http://wo.hahajie.cn

C#:   public string Greet() => Name;
来源：http://dd.gzmigu.cn

[G05] 继承
来源：http://wt.yuexingan06.cn

Py:   class Admin(User): pass
来源：http://oi.shtwfgs.cn

PHP:  class Admin extends User {}
来源：http://gl.521024.cn

JS:   class Admin extends User {}
来源：http://hg.shxzukj.cn

TS:   class Admin extends User {}
来源：http://de.9csxet.cn

Java: class Admin extends User {}
来源：http://qx.szxytkj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://al.hahajie.cn

Ruby: class Admin < User; end
来源：http://ls.bjjhwx.cn

C#:   class Admin : User {}
来源：http://vc.szxytkj.cn

[G06] 重写方法
来源：http://wa.hahajie.cn

Py:   def greet(self): return "admin"
来源：http://ub.gzmigu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://jb.lnxyls.cn

JS:   greet() { return "admin"; }
来源：http://vz.hahajie.cn

TS:   greet(): string { return "admin"; }
来源：http://an.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://um.lnxyls.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://bx.huanxung.cn

Ruby: def greet; "admin"; end
来源：http://ve.huanxung.cn

C#:   public override string Greet() => "admin";
来源：http://qt.bookmarksfly.cn

[G07] 调用父类方法
来源：http://cy.jctech888.com.cn

Py:   super().greet()
来源：http://vb.lnxyls.cn

PHP:  parent::greet();
来源：http://le.shtwfgs.cn

JS:   super.greet();
来源：http://ak.shxzukj.cn

TS:   super.greet();
来源：http://sr.hnjuh.cn

Java: super.greet();
来源：http://cr.yuntaijiaju.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://pn.szsharing.cn

Ruby: super
来源：http://fo.chemitech.net.cn

C#:   base.Greet();
来源：http://ku.newstarts.cn

[G08] 静态方法与属性
来源：http://ab.bookmarksfly.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://eb.521024.cn

PHP:  public static function f() {}
来源：http://pv.nszjky.cn

JS:   static f() {}
来源：http://ad.jianghongdianzi.cn

TS:   static f(): void {}
来源：http://ud.yuexingan06.cn

Java: static void f() {}
来源：http://cg.muxihuayi.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://fo.huanxung.cn

Ruby: def self.f; end
来源：http://dg.huixiangedu.cn

C#:   public static void F() {}
来源：http://ie.wgjwhj.cn

[G09] 接口 / 抽象类
来源：http://gp.nszjky.cn

Py:   from abc import ABC, abstractmethod
来源：http://wh.bookmarksfly.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ei.haigaiapp.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://xi.hahajie.cn

TS:   interface Shape { area(): number; }
来源：http://ml.jianghongdianzi.cn

Java: interface Shape { double area(); }
来源：http://vy.chemitech.net.cn

Go:   type Shape interface { Area() float64 }
来源：http://kq.huanxung.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://bu.chemitech.net.cn

C#:   interface IShape { double Area(); }
来源：http://tl.haigaiapp.cn

[G10] 访问控制
来源：http://gc.haigaiapp.cn

Py:   约定 _protected / __private（不强制）
来源：http://zr.huixinmuqiang.cn

PHP:  public / protected / private
来源：http://vg.wgjwhj.cn

JS:   #private 字段；其余公开
来源：http://aj.521024.cn

TS:   public / protected / private
来源：http://th.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://tr.panjiajie.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://im.shxzskj.cn

Ruby: public / protected / private
来源：http://ix.newstarts.cn

C#:   public / protected / private / internal
来源：http://qa.jctech888.com.cn

[G11] getter / setter
来源：http://yd.yuexingan06.cn

Py:   @property 与 @x.setter
来源：http://sf.huixinmuqiang.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://nb.asd995.cn

JS:   get name() { return this._name; }
来源：http://vv.panjiajie.cn

TS:   get name(): string { return this._name; }
来源：http://jr.wgjwhj.cn

Java: public String getName() { return name; }
来源：http://gs.hnjuh.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://hg.bookmarksfly.cn

Ruby: attr_accessor :name
来源：http://hf.shxzukj.cn

C#:   public string Name { get; set; }
来源：http://qi.hnjuh.cn

[G12] 对象转字符串
来源：http://iz.521024.cn

Py:   def __str__(self): return self.name
来源：http://td.yuexingan06.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://yp.yuexingan06.cn

JS:   toString() { return this.name; }
来源：http://zg.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://ab.bookmarksfly.cn

Java: @Override public String toString() { return name; }
来源：http://hj.bjjhwx.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uu.bjjhwx.cn

Ruby: def to_s; @name; end
来源：http://lq.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://ag.huanxung.cn

[G13] 判断对象类型
来源：http://fp.shtwfgs.cn

Py:   isinstance(u, User)
来源：http://go.lnxyls.cn

PHP:  $u instanceof User
来源：http://mw.9csxet.cn

JS:   u instanceof User
来源：http://xx.yuexingan06.cn

TS:   u instanceof User
来源：http://ea.asd995.cn

Java: u instanceof User
来源：http://ts.yuntaijiaju.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://df.huixiangedu.cn

Ruby: u.is_a?(User)
来源：http://yj.chemitech.net.cn

C#:   u is User
来源：http://yr.gzmigu.cn

[G14] 数据类 / record
来源：http://gf.nszjky.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://sg.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://lj.lnxyls.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ga.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://ja.gzmigu.cn

Java: record User(String name, int age) {}
来源：http://qy.huixinmuqiang.cn

Go:   type User struct { Name string; Age int }
来源：http://xw.asd995.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://xu.shxzukj.cn

C#:   record User(string Name, int Age);
来源：http://hb.szsharing.cn

[G15] 枚举
来源：http://kh.huixiangedu.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://sw.panjiajie.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://th.nicolike.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://lu.bjjhwx.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://jc.newstarts.cn

Java: enum Color { RED, GREEN }
来源：http://bm.panjiajie.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://yv.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://qd.nicolike.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://sd.shxzukj.cn

[G16] 对象转数组 / 字典
来源：http://la.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fw.szsharing.cn

PHP:  get_object_vars($obj);
来源：http://vr.nszjky.cn

JS:   Object.entries(obj)
来源：http://oy.wgjwhj.cn

TS:   Object.entries(obj)
来源：http://bx.yuexingan06.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yz.bjjhwx.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://gw.bookmarksfly.cn

Ruby: obj.instance_variables
来源：http://xi.szxytkj.cn

C#:   // 用反射或 System.Text.Json
来源：http://pe.bjjhwx.cn

================================================================================
来源：http://wn.hnjuh.cn

H. 异常与错误处理
来源：http://ma.chemitech.net.cn

================================================================================
来源：http://se.panjiajie.cn

[H01] try / catch 基础
来源：http://ch.shtwfgs.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ph.huanxung.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://gf.nszjky.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rt.asd995.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://vw.muxihuayi.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://al.asd995.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ct.hnjuh.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ga.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hu.szsharing.cn

[H02] finally / ensure 收尾
来源：http://ln.szsharing.cn

Py:   try: f()⏎finally: cleanup()
来源：http://cj.shxzskj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sv.nicolike.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://nr.nszjky.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://gf.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://oe.wgjwhj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://wl.shtwfgs.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://io.haigaiapp.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://sv.nszjky.cn

[H03] 主动抛出异常
来源：http://al.jctech888.com.cn

Py:   raise ValueError("错误信息")
来源：http://ym.hahajie.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://px.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://tg.gzmigu.cn

TS:   throw new Error("错误信息");
来源：http://rk.nicolike.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://jm.chemitech.net.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://bf.hahajie.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rb.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://xr.jianghongdianzi.cn

[H04] 自定义异常类型
来源：http://uj.shxzskj.cn

Py:   class MyError(Exception): pass
来源：http://dx.yuntaijiaju.cn

PHP:  class MyError extends RuntimeException {}
来源：http://gf.chemitech.net.cn

JS:   class MyError extends Error {}
来源：http://lx.szsharing.cn

TS:   class MyError extends Error {}
来源：http://wz.shtwfgs.cn

Java: class MyException extends RuntimeException {}
来源：http://gf.huanxung.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ax.szsharing.cn


<!-- 参考信息 -->