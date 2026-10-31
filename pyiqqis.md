代发 wailian999

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shtwfgs.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://dw.wgjwhj.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://bk.newstarts.cn

Ruby: s.bytesize;  s.length
来源：http://dw.muxihuayi.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://sm.asd995.cn

================================================================================
来源：http://lz.haigaiapp.cn

F. 文件与目录
来源：http://xw.szsharing.cn

================================================================================
来源：http://wf.szxytkj.cn

[F01] 读取整个文件
来源：http://uo.jianghongdianzi.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://gz.panjiajie.cn

PHP:  file_get_contents("a.txt");
来源：http://cd.jianghongdianzi.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wp.shtwfgs.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://lk.muxihuayi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://ij.521024.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://lq.szsharing.cn

Ruby: File.read("a.txt")
来源：http://cb.gzmigu.cn

C#:   File.ReadAllText("a.txt");
来源：http://re.521024.cn

[F02] 逐行读取文件
来源：http://nw.jctech888.com.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://kf.lnxyls.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://dz.521024.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://jk.shtwfgs.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ht.hnjuh.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mj.asd995.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ta.nicolike.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ih.szsharing.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://er.jctech888.com.cn

[F03] 写入文件（覆盖）
来源：http://gn.yuntaijiaju.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://ed.panjiajie.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://ib.yuntaijiaju.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://en.shtwfgs.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://le.szxytkj.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://ag.bookmarksfly.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://pf.szsharing.cn

Ruby: File.write("a.txt", "hi")
来源：http://ru.colortex.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://tb.shxzskj.cn

[F04] 追加写入文件
来源：http://jn.asd995.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://ka.nicolike.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://vo.huixiangedu.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dr.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://xx.nicolike.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://zr.szsharing.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://se.bjjhwx.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://sa.jianghongdianzi.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://zb.haigaiapp.cn

[F05] 判断文件或目录是否存在
来源：http://qx.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://dx.521024.cn

PHP:  file_exists("a.txt");
来源：http://tw.nicolike.cn

JS:   fs.existsSync("a.txt")
来源：http://uk.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://zq.hnjuh.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://lu.huixiangedu.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://et.chemitech.net.cn

Ruby: File.exist?("a.txt")
来源：http://lp.nicolike.cn

C#:   File.Exists("a.txt")
来源：http://qp.gzmigu.cn

[F06] 删除文件
来源：http://ns.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://dx.shxzukj.cn

PHP:  unlink("a.txt");
来源：http://qp.huanxung.cn

JS:   fs.unlinkSync("a.txt")
来源：http://xn.nszjky.cn

TS:   fs.unlinkSync("a.txt")
来源：http://nm.521024.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://fo.newstarts.cn

Go:   os.Remove("a.txt")
来源：http://pt.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://qb.szsharing.cn

C#:   File.Delete("a.txt");
来源：http://gi.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://zk.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://bi.jianghongdianzi.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://jg.lnxyls.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://xr.hahajie.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://gx.gzmigu.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ym.asd995.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://az.haigaiapp.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://eh.huanxung.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://uk.lnxyls.cn

[F08] 遍历目录
来源：http://ml.szsharing.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://xg.newstarts.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://uo.hnjuh.cn

JS:   fs.readdirSync("dir")
来源：http://if.521024.cn

TS:   fs.readdirSync("dir")
来源：http://bc.yuexingan06.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://zx.shxzukj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://cv.huanxung.cn

Ruby: Dir.children("dir")
来源：http://zg.haigaiapp.cn

C#:   Directory.GetFiles("dir")
来源：http://wv.hahajie.cn

[F09] 获取文件大小
来源：http://pm.haigaiapp.cn

Py:   os.path.getsize("a.txt")
来源：http://kc.jctech888.com.cn

PHP:  filesize("a.txt");
来源：http://vd.szxytkj.cn

JS:   fs.statSync("a.txt").size
来源：http://af.9csxet.cn

TS:   fs.statSync("a.txt").size
来源：http://oo.nszjky.cn

Java: Files.size(Path.of("a.txt"))
来源：http://sz.gzmigu.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://gw.bjjhwx.cn

Ruby: File.size("a.txt")
来源：http://xp.haigaiapp.cn

C#:   new FileInfo("a.txt").Length
来源：http://fb.newstarts.cn

[F10] 取文件扩展名 / 文件名
来源：http://kh.szsharing.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mm.bjjhwx.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://uw.9csxet.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://kw.yuexingan06.cn

TS:   path.extname("a.txt")
来源：http://kg.asd995.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://kz.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://nj.shxzukj.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://gz.huanxung.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://pn.muxihuayi.cn

[F11] 复制与移动文件
来源：http://zb.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://al.huixinmuqiang.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ut.bookmarksfly.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://vb.haigaiapp.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wg.bookmarksfly.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hg.huixiangedu.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://ns.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ik.521024.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://qa.muxihuayi.cn

[F12] CSV 读写
来源：http://ug.panjiajie.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://jx.huixinmuqiang.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://xu.wgjwhj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://ho.muxihuayi.cn

TS:   // 同上
来源：http://mz.jctech888.com.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zz.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://xp.shtwfgs.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://ze.521024.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://fc.huanxung.cn

================================================================================
来源：http://ta.newstarts.cn

G. 面向对象
来源：http://ik.huixiangedu.cn

================================================================================
来源：http://ry.chemitech.net.cn

[G01] 定义类
来源：http://jp.bjjhwx.cn

Py:   class User: pass
来源：http://my.hnjuh.cn

PHP:  class User {}
来源：http://rw.nicolike.cn

JS:   class User {}
来源：http://ox.huanxung.cn

TS:   class User { name: string = ""; }
来源：http://xc.muxihuayi.cn

Java: class User {}
来源：http://bg.wgjwhj.cn

Go:   type User struct { Name string }
来源：http://rh.nicolike.cn

Ruby: class User; end
来源：http://gu.szsharing.cn

C#:   class User {}
来源：http://td.asd995.cn

[G02] 构造函数
来源：http://ku.huixiangedu.cn

Py:   def __init__(self, name): self.name = name
来源：http://xj.bookmarksfly.cn

PHP:  public function __construct(public string $name) {}
来源：http://op.nicolike.cn

JS:   constructor(name) { this.name = name; }
来源：http://vx.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://wg.asd995.cn

Java: User(String name) { this.name = name; }
来源：http://hr.newstarts.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://sm.shxzskj.cn

Ruby: def initialize(name); @name = name; end
来源：http://gu.newstarts.cn

C#:   public User(string name) { Name = name; }
来源：http://mi.huixiangedu.cn

[G03] 实例属性
来源：http://ff.shxzskj.cn

Py:   self.name = "x"
来源：http://pw.hnjuh.cn

PHP:  public string $name = "x";
来源：http://oj.gzmigu.cn

JS:   this.name = "x";
来源：http://py.huixiangedu.cn

TS:   name: string = "x";
来源：http://fi.lnxyls.cn

Java: private String name;
来源：http://yz.nicolike.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://na.nszjky.cn

Ruby: @name = "x"
来源：http://gz.newstarts.cn

C#:   public string Name { get; set; } = "x";
来源：http://xu.jianghongdianzi.cn

[G04] 定义方法
来源：http://qk.nszjky.cn

Py:   def greet(self): return self.name
来源：http://za.asd995.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ub.jctech888.com.cn

JS:   greet() { return this.name; }
来源：http://qs.jctech888.com.cn

TS:   greet(): string { return this.name; }
来源：http://xm.shxzskj.cn

Java: String greet() { return name; }
来源：http://zl.huanxung.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://ez.lnxyls.cn

Ruby: def greet; @name; end
来源：http://oa.panjiajie.cn

C#:   public string Greet() => Name;
来源：http://rz.chemitech.net.cn

[G05] 继承
来源：http://io.shxzskj.cn

Py:   class Admin(User): pass
来源：http://qi.huixiangedu.cn

PHP:  class Admin extends User {}
来源：http://rf.521024.cn

JS:   class Admin extends User {}
来源：http://xc.jianghongdianzi.cn

TS:   class Admin extends User {}
来源：http://xo.bjjhwx.cn

Java: class Admin extends User {}
来源：http://ln.huanxung.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://kb.9csxet.cn

Ruby: class Admin < User; end
来源：http://hs.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://ld.colortex.cn

[G06] 重写方法
来源：http://rw.521024.cn

Py:   def greet(self): return "admin"
来源：http://ro.hahajie.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://vn.panjiajie.cn

JS:   greet() { return "admin"; }
来源：http://ro.bookmarksfly.cn

TS:   greet(): string { return "admin"; }
来源：http://nq.shxzukj.cn

Java: @Override String greet() { return "admin"; }
来源：http://eg.asd995.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://na.gzmigu.cn

Ruby: def greet; "admin"; end
来源：http://ap.asd995.cn

C#:   public override string Greet() => "admin";
来源：http://vx.newstarts.cn

[G07] 调用父类方法
来源：http://vw.nicolike.cn

Py:   super().greet()
来源：http://sg.hnjuh.cn

PHP:  parent::greet();
来源：http://wi.bookmarksfly.cn

JS:   super.greet();
来源：http://hk.chemitech.net.cn

TS:   super.greet();
来源：http://lt.szsharing.cn

Java: super.greet();
来源：http://pc.szxytkj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://gk.shtwfgs.cn

Ruby: super
来源：http://tw.colortex.cn

C#:   base.Greet();
来源：http://ph.hahajie.cn

[G08] 静态方法与属性
来源：http://is.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://fs.chemitech.net.cn

PHP:  public static function f() {}
来源：http://nk.lnxyls.cn

JS:   static f() {}
来源：http://sn.jctech888.com.cn

TS:   static f(): void {}
来源：http://yq.muxihuayi.cn

Java: static void f() {}
来源：http://vv.gzmigu.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://io.shtwfgs.cn

Ruby: def self.f; end
来源：http://zg.chemitech.net.cn

C#:   public static void F() {}
来源：http://em.gzmigu.cn

[G09] 接口 / 抽象类
来源：http://yw.gzmigu.cn

Py:   from abc import ABC, abstractmethod
来源：http://pg.gzmigu.cn

PHP:  interface Shape { public function area(): float; }
来源：http://wz.chemitech.net.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://lg.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://ju.jctech888.com.cn

Java: interface Shape { double area(); }
来源：http://zb.szxytkj.cn

Go:   type Shape interface { Area() float64 }
来源：http://vx.nszjky.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://go.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://oj.chemitech.net.cn

[G10] 访问控制
来源：http://dc.szsharing.cn

Py:   约定 _protected / __private（不强制）
来源：http://ek.szxytkj.cn

PHP:  public / protected / private
来源：http://lx.jctech888.com.cn

JS:   #private 字段；其余公开
来源：http://ua.szxytkj.cn

TS:   public / protected / private
来源：http://yp.hnjuh.cn

Java: public / protected / private / 默认包级
来源：http://km.huanxung.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://yk.shtwfgs.cn

Ruby: public / protected / private
来源：http://fv.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://zu.panjiajie.cn

[G11] getter / setter
来源：http://ka.asd995.cn

Py:   @property 与 @x.setter
来源：http://tf.asd995.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://xr.panjiajie.cn

JS:   get name() { return this._name; }
来源：http://ve.szxytkj.cn

TS:   get name(): string { return this._name; }
来源：http://iq.huixiangedu.cn

Java: public String getName() { return name; }
来源：http://gf.shtwfgs.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tc.muxihuayi.cn

Ruby: attr_accessor :name
来源：http://aw.9csxet.cn

C#:   public string Name { get; set; }
来源：http://fd.521024.cn

[G12] 对象转字符串
来源：http://rw.szsharing.cn

Py:   def __str__(self): return self.name
来源：http://cl.szxytkj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://zc.hnjuh.cn

JS:   toString() { return this.name; }
来源：http://ug.nicolike.cn

TS:   toString(): string { return this.name; }
来源：http://dw.huixiangedu.cn

Java: @Override public String toString() { return name; }
来源：http://wa.nicolike.cn

Go:   func (u User) String() string { return u.Name }
来源：http://kk.muxihuayi.cn

Ruby: def to_s; @name; end
来源：http://by.bjjhwx.cn

C#:   public override string ToString() => Name;
来源：http://rt.nicolike.cn

[G13] 判断对象类型
来源：http://ye.hnjuh.cn

Py:   isinstance(u, User)
来源：http://sn.szxytkj.cn

PHP:  $u instanceof User
来源：http://vm.gzmigu.cn

JS:   u instanceof User
来源：http://xi.nszjky.cn

TS:   u instanceof User
来源：http://ah.szsharing.cn

Java: u instanceof User
来源：http://dl.huanxung.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nf.jctech888.com.cn

Ruby: u.is_a?(User)
来源：http://bg.asd995.cn

C#:   u is User
来源：http://to.jctech888.com.cn

[G14] 数据类 / record
来源：http://ag.newstarts.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://gx.newstarts.cn

PHP:  // 用 readonly 属性模拟
来源：http://fs.panjiajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://qn.asd995.cn

TS:   type User = { name: string; age: number };
来源：http://fx.muxihuayi.cn

Java: record User(String name, int age) {}
来源：http://jx.lnxyls.cn

Go:   type User struct { Name string; Age int }
来源：http://kl.muxihuayi.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jm.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://jn.nicolike.cn

[G15] 枚举
来源：http://dl.yuntaijiaju.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://gc.asd995.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://cl.panjiajie.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://xp.panjiajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://pk.jianghongdianzi.cn

Java: enum Color { RED, GREEN }
来源：http://xx.521024.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lu.szxytkj.cn

Ruby: Color = %i[red green].freeze
来源：http://fh.bookmarksfly.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://af.shxzskj.cn

[G16] 对象转数组 / 字典
来源：http://pr.lnxyls.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://lg.shtwfgs.cn

PHP:  get_object_vars($obj);
来源：http://rr.szxytkj.cn

JS:   Object.entries(obj)
来源：http://ew.shtwfgs.cn

TS:   Object.entries(obj)
来源：http://hg.colortex.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wx.gzmigu.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://zu.shxzskj.cn

Ruby: obj.instance_variables
来源：http://pp.huixiangedu.cn

C#:   // 用反射或 System.Text.Json
来源：http://dg.colortex.cn

================================================================================
来源：http://kq.shxzskj.cn

H. 异常与错误处理
来源：http://qo.hahajie.cn

================================================================================
来源：http://vz.bjjhwx.cn

[H01] try / catch 基础
来源：http://et.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hv.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://we.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://xd.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://gh.bjjhwx.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xg.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://kp.521024.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://lf.9csxet.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://hl.panjiajie.cn

[H02] finally / ensure 收尾
来源：http://ba.chemitech.net.cn

Py:   try: f()⏎finally: cleanup()
来源：http://em.lnxyls.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://oi.shxzukj.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://yh.bookmarksfly.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://zx.gzmigu.cn

Java: try { f(); } finally { cleanup(); }
来源：http://vp.haigaiapp.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://ph.huixinmuqiang.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://vy.szsharing.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://mm.yuexingan06.cn

[H03] 主动抛出异常
来源：http://vi.gzmigu.cn

Py:   raise ValueError("错误信息")
来源：http://sj.shxzskj.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://pe.lnxyls.cn

JS:   throw new Error("错误信息");
来源：http://ht.shtwfgs.cn

TS:   throw new Error("错误信息");
来源：http://hd.asd995.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://qv.nicolike.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ep.szxytkj.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://rf.lnxyls.cn

C#:   throw new ArgumentException("错误信息");
来源：http://ig.muxihuayi.cn

[H04] 自定义异常类型
来源：http://kb.yuntaijiaju.cn

Py:   class MyError(Exception): pass
来源：http://xx.wgjwhj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://yy.huanxung.cn

JS:   class MyError extends Error {}
来源：http://pz.jctech888.com.cn

TS:   class MyError extends Error {}
来源：http://ut.gzmigu.cn

Java: class MyException extends RuntimeException {}
来源：http://wb.huixinmuqiang.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://li.nszjky.cn


<!-- 参考信息 -->