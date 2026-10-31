代发 wailian999

[E22] 字节长度与字符长度
来源：http://gc.asd995.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://ly.shxzskj.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://cb.gzmigu.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mf.huanxung.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://xs.asd995.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://zg.hnjuh.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://zi.chemitech.net.cn

Ruby: s.bytesize;  s.length
来源：http://xc.szsharing.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://lm.jianghongdianzi.cn

================================================================================
来源：http://ia.yuexingan06.cn

F. 文件与目录
来源：http://rc.newstarts.cn

================================================================================
来源：http://bq.gzmigu.cn

[F01] 读取整个文件
来源：http://kt.asd995.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://nb.haigaiapp.cn

PHP:  file_get_contents("a.txt");
来源：http://lg.yuntaijiaju.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://fv.nicolike.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://bj.jianghongdianzi.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://pk.szsharing.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://bf.yuntaijiaju.cn

Ruby: File.read("a.txt")
来源：http://xq.nszjky.cn

C#:   File.ReadAllText("a.txt");
来源：http://us.chemitech.net.cn

[F02] 逐行读取文件
来源：http://aw.huanxung.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://tp.shtwfgs.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://tz.yuntaijiaju.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pn.panjiajie.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://ok.asd995.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vr.panjiajie.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://ns.hnjuh.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://sv.szxytkj.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://ms.jianghongdianzi.cn

[F03] 写入文件（覆盖）
来源：http://zu.jctech888.com.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://uc.gzmigu.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://to.huixiangedu.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://tu.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://qb.jianghongdianzi.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://us.yuntaijiaju.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://xl.hahajie.cn

Ruby: File.write("a.txt", "hi")
来源：http://xz.9csxet.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://xy.haigaiapp.cn

[F04] 追加写入文件
来源：http://np.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://bu.yuntaijiaju.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://rt.wgjwhj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://dz.hnjuh.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://za.yuntaijiaju.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://cr.nicolike.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://cw.hnjuh.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://dm.521024.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://ly.asd995.cn

[F05] 判断文件或目录是否存在
来源：http://ze.newstarts.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://uk.bookmarksfly.cn

PHP:  file_exists("a.txt");
来源：http://ck.wgjwhj.cn

JS:   fs.existsSync("a.txt")
来源：http://pw.bookmarksfly.cn

TS:   fs.existsSync("a.txt")
来源：http://ic.shxzukj.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ic.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://xy.szsharing.cn

Ruby: File.exist?("a.txt")
来源：http://qi.521024.cn

C#:   File.Exists("a.txt")
来源：http://fc.521024.cn

[F06] 删除文件
来源：http://zn.shxzukj.cn

Py:   os.remove("a.txt")
来源：http://cl.shxzskj.cn

PHP:  unlink("a.txt");
来源：http://ki.hnjuh.cn

JS:   fs.unlinkSync("a.txt")
来源：http://tw.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://zl.gzmigu.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://ry.521024.cn

Go:   os.Remove("a.txt")
来源：http://zl.nicolike.cn

Ruby: File.delete("a.txt")
来源：http://yn.shxzukj.cn

C#:   File.Delete("a.txt");
来源：http://un.nicolike.cn

[F07] 创建目录（含多级）
来源：http://ov.hnjuh.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hv.lnxyls.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://xx.haigaiapp.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kt.asd995.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://kx.yuntaijiaju.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://ck.panjiajie.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vf.yuexingan06.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://ek.szsharing.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://ro.newstarts.cn

[F08] 遍历目录
来源：http://gf.huixiangedu.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://gu.lnxyls.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://lx.muxihuayi.cn

JS:   fs.readdirSync("dir")
来源：http://cj.hnjuh.cn

TS:   fs.readdirSync("dir")
来源：http://mf.huixinmuqiang.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://gz.nszjky.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://au.huanxung.cn

Ruby: Dir.children("dir")
来源：http://us.szxytkj.cn

C#:   Directory.GetFiles("dir")
来源：http://sj.nicolike.cn

[F09] 获取文件大小
来源：http://wl.shxzskj.cn

Py:   os.path.getsize("a.txt")
来源：http://ws.huixiangedu.cn

PHP:  filesize("a.txt");
来源：http://hw.yuexingan06.cn

JS:   fs.statSync("a.txt").size
来源：http://oc.lnxyls.cn

TS:   fs.statSync("a.txt").size
来源：http://zn.panjiajie.cn

Java: Files.size(Path.of("a.txt"))
来源：http://hq.newstarts.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://vj.huanxung.cn

Ruby: File.size("a.txt")
来源：http://jn.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://ok.yuexingan06.cn

[F10] 取文件扩展名 / 文件名
来源：http://um.521024.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wl.colortex.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qf.shxzukj.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://bn.shxzukj.cn

TS:   path.extname("a.txt")
来源：http://fa.huixiangedu.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://ue.huixiangedu.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://oh.shtwfgs.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wz.lnxyls.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://xu.wgjwhj.cn

[F11] 复制与移动文件
来源：http://ry.szsharing.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://nb.hnjuh.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://zj.asd995.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ui.panjiajie.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ys.shtwfgs.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://ps.huixinmuqiang.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://cj.nszjky.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://ss.chemitech.net.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://ix.asd995.cn

[F12] CSV 读写
来源：http://ke.szxytkj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sy.shtwfgs.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mo.hnjuh.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wu.shxzskj.cn

TS:   // 同上
来源：http://lj.huixinmuqiang.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://zh.huixiangedu.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://kg.newstarts.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://yr.jctech888.com.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://lv.yuexingan06.cn

================================================================================
来源：http://hb.shxzskj.cn

G. 面向对象
来源：http://fy.shxzskj.cn

================================================================================
来源：http://dp.asd995.cn

[G01] 定义类
来源：http://xs.yuntaijiaju.cn

Py:   class User: pass
来源：http://sz.shxzskj.cn

PHP:  class User {}
来源：http://wr.szxytkj.cn

JS:   class User {}
来源：http://st.hnjuh.cn

TS:   class User { name: string = ""; }
来源：http://au.chemitech.net.cn

Java: class User {}
来源：http://bx.szsharing.cn

Go:   type User struct { Name string }
来源：http://oa.nicolike.cn

Ruby: class User; end
来源：http://dr.jctech888.com.cn

C#:   class User {}
来源：http://fn.hahajie.cn

[G02] 构造函数
来源：http://ov.bjjhwx.cn

Py:   def __init__(self, name): self.name = name
来源：http://db.bjjhwx.cn

PHP:  public function __construct(public string $name) {}
来源：http://cp.jianghongdianzi.cn

JS:   constructor(name) { this.name = name; }
来源：http://ew.huixiangedu.cn

TS:   constructor(public name: string) {}
来源：http://ig.lnxyls.cn

Java: User(String name) { this.name = name; }
来源：http://ev.bookmarksfly.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://co.colortex.cn

Ruby: def initialize(name); @name = name; end
来源：http://mt.haigaiapp.cn

C#:   public User(string name) { Name = name; }
来源：http://ak.huanxung.cn

[G03] 实例属性
来源：http://qd.newstarts.cn

Py:   self.name = "x"
来源：http://tc.huixiangedu.cn

PHP:  public string $name = "x";
来源：http://mk.huanxung.cn

JS:   this.name = "x";
来源：http://tq.panjiajie.cn

TS:   name: string = "x";
来源：http://rk.shxzskj.cn

Java: private String name;
来源：http://pf.huanxung.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://kr.szxytkj.cn

Ruby: @name = "x"
来源：http://cd.9csxet.cn

C#:   public string Name { get; set; } = "x";
来源：http://ci.muxihuayi.cn

[G04] 定义方法
来源：http://fw.asd995.cn

Py:   def greet(self): return self.name
来源：http://zg.nszjky.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://fb.panjiajie.cn

JS:   greet() { return this.name; }
来源：http://hr.shtwfgs.cn

TS:   greet(): string { return this.name; }
来源：http://wv.hnjuh.cn

Java: String greet() { return name; }
来源：http://sp.szxytkj.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://wm.huixinmuqiang.cn

Ruby: def greet; @name; end
来源：http://mm.szxytkj.cn

C#:   public string Greet() => Name;
来源：http://na.colortex.cn

[G05] 继承
来源：http://qu.szxytkj.cn

Py:   class Admin(User): pass
来源：http://ty.huanxung.cn

PHP:  class Admin extends User {}
来源：http://df.hahajie.cn

JS:   class Admin extends User {}
来源：http://ti.szsharing.cn

TS:   class Admin extends User {}
来源：http://nd.szsharing.cn

Java: class Admin extends User {}
来源：http://ss.muxihuayi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://nc.yuntaijiaju.cn

Ruby: class Admin < User; end
来源：http://ff.szsharing.cn

C#:   class Admin : User {}
来源：http://wo.shtwfgs.cn

[G06] 重写方法
来源：http://fg.szxytkj.cn

Py:   def greet(self): return "admin"
来源：http://bb.yuexingan06.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://cc.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ps.yuexingan06.cn

TS:   greet(): string { return "admin"; }
来源：http://ut.szsharing.cn

Java: @Override String greet() { return "admin"; }
来源：http://tq.shxzukj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mg.szsharing.cn

Ruby: def greet; "admin"; end
来源：http://ja.nszjky.cn

C#:   public override string Greet() => "admin";
来源：http://zk.huixiangedu.cn

[G07] 调用父类方法
来源：http://tc.shxzukj.cn

Py:   super().greet()
来源：http://jo.gzmigu.cn

PHP:  parent::greet();
来源：http://ih.9csxet.cn

JS:   super.greet();
来源：http://uv.gzmigu.cn

TS:   super.greet();
来源：http://zk.yuexingan06.cn

Java: super.greet();
来源：http://oi.nicolike.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mm.hahajie.cn

Ruby: super
来源：http://ir.lnxyls.cn

C#:   base.Greet();
来源：http://ic.yuntaijiaju.cn

[G08] 静态方法与属性
来源：http://ar.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://jm.huixiangedu.cn

PHP:  public static function f() {}
来源：http://ys.521024.cn

JS:   static f() {}
来源：http://ox.nicolike.cn

TS:   static f(): void {}
来源：http://dl.newstarts.cn

Java: static void f() {}
来源：http://hk.shxzskj.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://zt.521024.cn

Ruby: def self.f; end
来源：http://ps.wgjwhj.cn

C#:   public static void F() {}
来源：http://fu.bookmarksfly.cn

[G09] 接口 / 抽象类
来源：http://mg.hnjuh.cn

Py:   from abc import ABC, abstractmethod
来源：http://ve.panjiajie.cn

PHP:  interface Shape { public function area(): float; }
来源：http://xx.hahajie.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://hs.huixiangedu.cn

TS:   interface Shape { area(): number; }
来源：http://cu.huanxung.cn

Java: interface Shape { double area(); }
来源：http://aq.gzmigu.cn

Go:   type Shape interface { Area() float64 }
来源：http://jf.panjiajie.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://fq.muxihuayi.cn

C#:   interface IShape { double Area(); }
来源：http://jr.asd995.cn

[G10] 访问控制
来源：http://oa.gzmigu.cn

Py:   约定 _protected / __private（不强制）
来源：http://gp.nicolike.cn

PHP:  public / protected / private
来源：http://zs.huanxung.cn

JS:   #private 字段；其余公开
来源：http://pr.shtwfgs.cn

TS:   public / protected / private
来源：http://qd.szxytkj.cn

Java: public / protected / private / 默认包级
来源：http://in.nszjky.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hi.szsharing.cn

Ruby: public / protected / private
来源：http://zx.szsharing.cn

C#:   public / protected / private / internal
来源：http://zk.lnxyls.cn

[G11] getter / setter
来源：http://cw.jianghongdianzi.cn

Py:   @property 与 @x.setter
来源：http://oo.nszjky.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://an.gzmigu.cn

JS:   get name() { return this._name; }
来源：http://pb.nszjky.cn

TS:   get name(): string { return this._name; }
来源：http://ay.chemitech.net.cn

Java: public String getName() { return name; }
来源：http://tp.muxihuayi.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://wd.yuntaijiaju.cn

Ruby: attr_accessor :name
来源：http://zq.newstarts.cn

C#:   public string Name { get; set; }
来源：http://ez.huixinmuqiang.cn

[G12] 对象转字符串
来源：http://bv.chemitech.net.cn

Py:   def __str__(self): return self.name
来源：http://tx.chemitech.net.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://bg.chemitech.net.cn

JS:   toString() { return this.name; }
来源：http://wf.szsharing.cn

TS:   toString(): string { return this.name; }
来源：http://jj.haigaiapp.cn

Java: @Override public String toString() { return name; }
来源：http://po.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://uq.gzmigu.cn

Ruby: def to_s; @name; end
来源：http://uy.huanxung.cn

C#:   public override string ToString() => Name;
来源：http://gc.nszjky.cn

[G13] 判断对象类型
来源：http://cg.muxihuayi.cn

Py:   isinstance(u, User)
来源：http://zs.colortex.cn

PHP:  $u instanceof User
来源：http://yh.colortex.cn

JS:   u instanceof User
来源：http://qg.szxytkj.cn

TS:   u instanceof User
来源：http://ro.shtwfgs.cn

Java: u instanceof User
来源：http://cj.jianghongdianzi.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://nd.huixinmuqiang.cn

Ruby: u.is_a?(User)
来源：http://it.jianghongdianzi.cn

C#:   u is User
来源：http://tm.huixinmuqiang.cn

[G14] 数据类 / record
来源：http://bf.huanxung.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tl.gzmigu.cn

PHP:  // 用 readonly 属性模拟
来源：http://sk.wgjwhj.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ep.huixinmuqiang.cn

TS:   type User = { name: string; age: number };
来源：http://hb.hnjuh.cn

Java: record User(String name, int age) {}
来源：http://ww.muxihuayi.cn

Go:   type User struct { Name string; Age int }
来源：http://wl.nszjky.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://rz.chemitech.net.cn

C#:   record User(string Name, int Age);
来源：http://bm.bjjhwx.cn

[G15] 枚举
来源：http://oj.szsharing.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://go.jianghongdianzi.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://ro.colortex.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wi.asd995.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://bz.colortex.cn

Java: enum Color { RED, GREEN }
来源：http://ib.wgjwhj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://lo.bjjhwx.cn

Ruby: Color = %i[red green].freeze
来源：http://hx.hahajie.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://vv.hahajie.cn

[G16] 对象转数组 / 字典
来源：http://ud.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://an.yuntaijiaju.cn

PHP:  get_object_vars($obj);
来源：http://dq.521024.cn

JS:   Object.entries(obj)
来源：http://br.bookmarksfly.cn

TS:   Object.entries(obj)
来源：http://se.huanxung.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://os.yuntaijiaju.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://cw.muxihuayi.cn

Ruby: obj.instance_variables
来源：http://na.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://il.nicolike.cn

================================================================================
来源：http://gz.szsharing.cn

H. 异常与错误处理
来源：http://dt.muxihuayi.cn

================================================================================
来源：http://nh.huixiangedu.cn

[H01] try / catch 基础
来源：http://zj.huixiangedu.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://ex.shxzskj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://yv.jianghongdianzi.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ao.jctech888.com.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://zb.huixinmuqiang.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://pe.yuntaijiaju.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://ou.wgjwhj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://iy.lnxyls.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://qf.nicolike.cn

[H02] finally / ensure 收尾
来源：http://qs.huixiangedu.cn

Py:   try: f()⏎finally: cleanup()
来源：http://rp.szxytkj.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://sk.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mv.lnxyls.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://ee.colortex.cn

Java: try { f(); } finally { cleanup(); }
来源：http://um.yuexingan06.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://zz.muxihuayi.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://km.lnxyls.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://yc.shxzukj.cn

[H03] 主动抛出异常
来源：http://id.lnxyls.cn

Py:   raise ValueError("错误信息")
来源：http://jx.szsharing.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://am.panjiajie.cn

JS:   throw new Error("错误信息");
来源：http://fg.haigaiapp.cn

TS:   throw new Error("错误信息");
来源：http://uv.newstarts.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://ok.szxytkj.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://ls.huixinmuqiang.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://is.shxzukj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://je.521024.cn

[H04] 自定义异常类型
来源：http://rq.huixinmuqiang.cn

Py:   class MyError(Exception): pass
来源：http://jx.nszjky.cn

PHP:  class MyError extends RuntimeException {}
来源：http://wy.muxihuayi.cn


<!-- 参考信息 -->