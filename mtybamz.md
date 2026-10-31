代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://yo.521024.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://me.yuntaijiaju.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://qt.jctech888.com.cn

Ruby: s.bytesize;  s.length
来源：http://ji.asd995.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://cm.gzmigu.cn

================================================================================
来源：http://ux.shxzukj.cn

F. 文件与目录
来源：http://st.jianghongdianzi.cn

================================================================================
来源：http://rc.bookmarksfly.cn

[F01] 读取整个文件
来源：http://nk.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gp.shtwfgs.cn

PHP:  file_get_contents("a.txt");
来源：http://hk.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mz.szsharing.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hk.yuntaijiaju.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://zj.shxzukj.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://jp.colortex.cn

Ruby: File.read("a.txt")
来源：http://rq.wgjwhj.cn

C#:   File.ReadAllText("a.txt");
来源：http://uc.shxzskj.cn

[F02] 逐行读取文件
来源：http://qj.nicolike.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://ki.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wk.panjiajie.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://aj.nicolike.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://eu.yuntaijiaju.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://zb.hnjuh.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ry.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://yz.muxihuayi.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ic.yuexingan06.cn

[F03] 写入文件（覆盖）
来源：http://ew.bjjhwx.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://vn.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ya.bookmarksfly.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://fm.huixiangedu.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ia.nszjky.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://bc.9csxet.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://fa.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://xp.bjjhwx.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://te.huixiangedu.cn

[F04] 追加写入文件
来源：http://zm.yuexingan06.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wp.huanxung.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://ln.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://zw.huixinmuqiang.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://nk.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://ra.nszjky.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://ji.colortex.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://fn.chemitech.net.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://ap.muxihuayi.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wp.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://iy.panjiajie.cn

JS:   fs.existsSync("a.txt")
来源：http://vx.nszjky.cn

TS:   fs.existsSync("a.txt")
来源：http://es.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://wh.shxzskj.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://ey.huanxung.cn

Ruby: File.exist?("a.txt")
来源：http://ml.shxzukj.cn

C#:   File.Exists("a.txt")
来源：http://tu.asd995.cn

[F06] 删除文件
来源：http://ei.szsharing.cn

Py:   os.remove("a.txt")
来源：http://jb.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://il.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://wi.huixinmuqiang.cn

TS:   fs.unlinkSync("a.txt")
来源：http://tw.colortex.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ht.lnxyls.cn

Go:   os.Remove("a.txt")
来源：http://yu.hnjuh.cn

Ruby: File.delete("a.txt")
来源：http://lw.521024.cn

C#:   File.Delete("a.txt");
来源：http://nw.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://df.chemitech.net.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://gy.9csxet.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://ja.jctech888.com.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://zg.nicolike.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://on.nszjky.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://fa.yuntaijiaju.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://ok.gzmigu.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://lf.chemitech.net.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ux.hnjuh.cn

[F08] 遍历目录
来源：http://ln.shxzskj.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://mh.jianghongdianzi.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://kw.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://nc.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://ac.newstarts.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://fn.lnxyls.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ez.gzmigu.cn

Ruby: Dir.children("dir")
来源：http://ux.newstarts.cn

C#:   Directory.GetFiles("dir")
来源：http://yn.nszjky.cn

[F09] 获取文件大小
来源：http://xc.9csxet.cn

Py:   os.path.getsize("a.txt")
来源：http://ha.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://eu.shxzukj.cn

JS:   fs.statSync("a.txt").size
来源：http://qa.gzmigu.cn

TS:   fs.statSync("a.txt").size
来源：http://pm.huixinmuqiang.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ct.asd995.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://rh.yuexingan06.cn

Ruby: File.size("a.txt")
来源：http://ql.bjjhwx.cn

C#:   new FileInfo("a.txt").Length
来源：http://ib.hahajie.cn

[F10] 取文件扩展名 / 文件名
来源：http://ig.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://lr.yuntaijiaju.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://bd.yuntaijiaju.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mt.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://ly.huanxung.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://aq.shxzskj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://zx.huixinmuqiang.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gw.huixinmuqiang.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wu.bookmarksfly.cn

[F11] 复制与移动文件
来源：http://ow.bjjhwx.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://br.yuntaijiaju.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://cy.shxzskj.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://nu.shtwfgs.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ld.szsharing.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://am.shtwfgs.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://tl.yuexingan06.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://rw.yuexingan06.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ec.bjjhwx.cn

[F12] CSV 读写
来源：http://sv.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wf.panjiajie.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://ps.asd995.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://bn.nszjky.cn

TS:   // 同上
来源：http://xo.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://rn.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://pl.shxzukj.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yy.nszjky.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lv.shxzukj.cn

================================================================================
来源：http://tt.szsharing.cn

G. 面向对象
来源：http://hc.hnjuh.cn

================================================================================
来源：http://cy.shtwfgs.cn

[G01] 定义类
来源：http://tz.huixiangedu.cn

Py:   class User: pass
来源：http://ty.shxzskj.cn

PHP:  class User {}
来源：http://id.haigaiapp.cn

JS:   class User {}
来源：http://ut.bjjhwx.cn

TS:   class User { name: string = ""; }
来源：http://xa.muxihuayi.cn

Java: class User {}
来源：http://lt.chemitech.net.cn

Go:   type User struct { Name string }
来源：http://os.gzmigu.cn

Ruby: class User; end
来源：http://ux.shtwfgs.cn

C#:   class User {}
来源：http://nq.lnxyls.cn

[G02] 构造函数
来源：http://mw.9csxet.cn

Py:   def __init__(self, name): self.name = name
来源：http://tb.521024.cn

PHP:  public function __construct(public string $name) {}
来源：http://wb.huixinmuqiang.cn

JS:   constructor(name) { this.name = name; }
来源：http://rk.huixinmuqiang.cn

TS:   constructor(public name: string) {}
来源：http://gq.hnjuh.cn

Java: User(String name) { this.name = name; }
来源：http://ez.chemitech.net.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://io.521024.cn

Ruby: def initialize(name); @name = name; end
来源：http://ig.yuntaijiaju.cn

C#:   public User(string name) { Name = name; }
来源：http://fl.szxytkj.cn

[G03] 实例属性
来源：http://sf.newstarts.cn

Py:   self.name = "x"
来源：http://ib.szxytkj.cn

PHP:  public string $name = "x";
来源：http://jr.huixinmuqiang.cn

JS:   this.name = "x";
来源：http://hl.wgjwhj.cn

TS:   name: string = "x";
来源：http://ya.9csxet.cn

Java: private String name;
来源：http://zc.chemitech.net.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://jk.bookmarksfly.cn

Ruby: @name = "x"
来源：http://vy.nicolike.cn

C#:   public string Name { get; set; } = "x";
来源：http://aa.hahajie.cn

[G04] 定义方法
来源：http://nz.lnxyls.cn

Py:   def greet(self): return self.name
来源：http://pt.yuntaijiaju.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://bg.bookmarksfly.cn

JS:   greet() { return this.name; }
来源：http://sg.newstarts.cn

TS:   greet(): string { return this.name; }
来源：http://pm.haigaiapp.cn

Java: String greet() { return name; }
来源：http://dq.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://kk.nszjky.cn

Ruby: def greet; @name; end
来源：http://iw.lnxyls.cn

C#:   public string Greet() => Name;
来源：http://nv.huixinmuqiang.cn

[G05] 继承
来源：http://xb.haigaiapp.cn

Py:   class Admin(User): pass
来源：http://td.newstarts.cn

PHP:  class Admin extends User {}
来源：http://tl.gzmigu.cn

JS:   class Admin extends User {}
来源：http://vj.jctech888.com.cn

TS:   class Admin extends User {}
来源：http://lu.9csxet.cn

Java: class Admin extends User {}
来源：http://jf.wgjwhj.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://cm.wgjwhj.cn

Ruby: class Admin < User; end
来源：http://uk.huixinmuqiang.cn

C#:   class Admin : User {}
来源：http://hn.yuntaijiaju.cn

[G06] 重写方法
来源：http://ra.wgjwhj.cn

Py:   def greet(self): return "admin"
来源：http://zs.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.huixinmuqiang.cn

JS:   greet() { return "admin"; }
来源：http://ew.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://bs.gzmigu.cn

Java: @Override String greet() { return "admin"; }
来源：http://wy.yuexingan06.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://yl.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ah.jctech888.com.cn

C#:   public override string Greet() => "admin";
来源：http://zy.hahajie.cn

[G07] 调用父类方法
来源：http://ks.panjiajie.cn

Py:   super().greet()
来源：http://yt.muxihuayi.cn

PHP:  parent::greet();
来源：http://of.521024.cn

JS:   super.greet();
来源：http://dd.szsharing.cn

TS:   super.greet();
来源：http://lj.huixinmuqiang.cn

Java: super.greet();
来源：http://dt.yuexingan06.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://na.panjiajie.cn

Ruby: super
来源：http://bd.hnjuh.cn

C#:   base.Greet();
来源：http://kt.chemitech.net.cn

[G08] 静态方法与属性
来源：http://ih.chemitech.net.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://qp.szxytkj.cn

PHP:  public static function f() {}
来源：http://pj.chemitech.net.cn

JS:   static f() {}
来源：http://zm.lnxyls.cn

TS:   static f(): void {}
来源：http://qz.yuexingan06.cn

Java: static void f() {}
来源：http://ic.bjjhwx.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://sc.hnjuh.cn

Ruby: def self.f; end
来源：http://yx.szxytkj.cn

C#:   public static void F() {}
来源：http://qi.lnxyls.cn

[G09] 接口 / 抽象类
来源：http://ji.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://wp.huanxung.cn

PHP:  interface Shape { public function area(): float; }
来源：http://to.panjiajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://zz.gzmigu.cn

TS:   interface Shape { area(): number; }
来源：http://vv.hahajie.cn

Java: interface Shape { double area(); }
来源：http://vb.szsharing.cn

Go:   type Shape interface { Area() float64 }
来源：http://wr.bookmarksfly.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://gi.jianghongdianzi.cn

C#:   interface IShape { double Area(); }
来源：http://fk.yuexingan06.cn

[G10] 访问控制
来源：http://ox.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://ve.huanxung.cn

PHP:  public / protected / private
来源：http://qn.colortex.cn

JS:   #private 字段；其余公开
来源：http://as.shtwfgs.cn

TS:   public / protected / private
来源：http://pd.521024.cn

Java: public / protected / private / 默认包级
来源：http://yh.yuntaijiaju.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://lh.shtwfgs.cn

Ruby: public / protected / private
来源：http://fl.lnxyls.cn

C#:   public / protected / private / internal
来源：http://io.9csxet.cn

[G11] getter / setter
来源：http://wy.chemitech.net.cn

Py:   @property 与 @x.setter
来源：http://qm.szxytkj.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://yp.lnxyls.cn

JS:   get name() { return this._name; }
来源：http://zf.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://vw.521024.cn

Java: public String getName() { return name; }
来源：http://qm.nszjky.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://gb.huanxung.cn

Ruby: attr_accessor :name
来源：http://pa.gzmigu.cn

C#:   public string Name { get; set; }
来源：http://zy.lnxyls.cn

[G12] 对象转字符串
来源：http://ht.muxihuayi.cn

Py:   def __str__(self): return self.name
来源：http://ke.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://eu.szsharing.cn

JS:   toString() { return this.name; }
来源：http://kk.asd995.cn

TS:   toString(): string { return this.name; }
来源：http://um.nicolike.cn

Java: @Override public String toString() { return name; }
来源：http://pp.hnjuh.cn

Go:   func (u User) String() string { return u.Name }
来源：http://rk.huixinmuqiang.cn

Ruby: def to_s; @name; end
来源：http://tk.shtwfgs.cn

C#:   public override string ToString() => Name;
来源：http://wu.yuexingan06.cn

[G13] 判断对象类型
来源：http://fh.newstarts.cn

Py:   isinstance(u, User)
来源：http://nq.shtwfgs.cn

PHP:  $u instanceof User
来源：http://yw.muxihuayi.cn

JS:   u instanceof User
来源：http://xp.huixiangedu.cn

TS:   u instanceof User
来源：http://wt.shxzukj.cn

Java: u instanceof User
来源：http://qj.panjiajie.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cb.muxihuayi.cn

Ruby: u.is_a?(User)
来源：http://fg.bjjhwx.cn

C#:   u is User
来源：http://mx.9csxet.cn

[G14] 数据类 / record
来源：http://jn.shxzukj.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://qn.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://to.huixinmuqiang.cn

JS:   // 无内置：普通类或对象字面量
来源：http://uv.shtwfgs.cn

TS:   type User = { name: string; age: number };
来源：http://bl.panjiajie.cn

Java: record User(String name, int age) {}
来源：http://an.asd995.cn

Go:   type User struct { Name string; Age int }
来源：http://ye.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://an.nszjky.cn

C#:   record User(string Name, int Age);
来源：http://db.wgjwhj.cn

[G15] 枚举
来源：http://no.colortex.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://yb.colortex.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://im.hnjuh.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://zs.nicolike.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bj.yuexingan06.cn

Java: enum Color { RED, GREEN }
来源：http://ea.huixiangedu.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://rr.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://dk.9csxet.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://qh.muxihuayi.cn

[G16] 对象转数组 / 字典
来源：http://at.huanxung.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ev.haigaiapp.cn

PHP:  get_object_vars($obj);
来源：http://wl.9csxet.cn

JS:   Object.entries(obj)
来源：http://su.jianghongdianzi.cn

TS:   Object.entries(obj)
来源：http://ll.lnxyls.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://xf.huixinmuqiang.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://el.521024.cn

Ruby: obj.instance_variables
来源：http://cq.wgjwhj.cn

C#:   // 用反射或 System.Text.Json
来源：http://ao.szsharing.cn

================================================================================
来源：http://zu.bjjhwx.cn

H. 异常与错误处理
来源：http://yl.shtwfgs.cn

================================================================================
来源：http://nv.wgjwhj.cn

[H01] try / catch 基础
来源：http://yy.huixinmuqiang.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kk.asd995.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://lr.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://eg.shxzukj.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gu.huixiangedu.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://lq.9csxet.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://an.huixiangedu.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://sy.nszjky.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://jf.asd995.cn

[H02] finally / ensure 收尾
来源：http://tr.asd995.cn

Py:   try: f()⏎finally: cleanup()
来源：http://ty.hnjuh.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lt.huixiangedu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://gt.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://sc.nicolike.cn

Java: try { f(); } finally { cleanup(); }
来源：http://ja.colortex.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yq.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://ao.jctech888.com.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://kn.nszjky.cn

[H03] 主动抛出异常
来源：http://xo.huixinmuqiang.cn

Py:   raise ValueError("错误信息")
来源：http://vg.bjjhwx.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://jb.colortex.cn

JS:   throw new Error("错误信息");
来源：http://zq.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://da.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://oq.muxihuayi.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://uo.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://bq.panjiajie.cn

C#:   throw new ArgumentException("错误信息");
来源：http://rd.haigaiapp.cn

[H04] 自定义异常类型
来源：http://xx.haigaiapp.cn

Py:   class MyError(Exception): pass
来源：http://yu.lnxyls.cn

PHP:  class MyError extends RuntimeException {}
来源：http://zj.hnjuh.cn

JS:   class MyError extends Error {}
来源：http://cr.haigaiapp.cn

TS:   class MyError extends Error {}
来源：http://nq.bookmarksfly.cn

Java: class MyException extends RuntimeException {}
来源：http://vn.shxzskj.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://ch.shxzskj.cn


<!-- 参考信息 -->