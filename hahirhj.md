代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://xi.nicolike.cn

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://nt.hnjuh.cn

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://fa.nicolike.cn

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wn.newstarts.cn

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://jr.muxihuayi.cn

Go:   // 按 rune 判断长度后截断
来源：http://bd.9csxet.cn

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mk.yuexingan06.cn

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://pj.wgjwhj.cn

[E22] 字节长度与字符长度
来源：http://fs.nicolike.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://xy.jctech888.com.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://bm.shxzukj.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://ra.wgjwhj.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://uy.newstarts.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://ln.nicolike.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://dw.lnxyls.cn

Ruby: s.bytesize;  s.length
来源：http://co.bookmarksfly.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://jb.panjiajie.cn

================================================================================
来源：http://zq.9csxet.cn

F. 文件与目录
来源：http://mj.shxzukj.cn

================================================================================
来源：http://pq.shxzukj.cn

[F01] 读取整个文件
来源：http://ib.haigaiapp.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://oc.521024.cn

PHP:  file_get_contents("a.txt");
来源：http://fi.huixiangedu.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://cx.lnxyls.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://iz.yuexingan06.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://sd.yuntaijiaju.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://gc.yuexingan06.cn

Ruby: File.read("a.txt")
来源：http://ku.newstarts.cn

C#:   File.ReadAllText("a.txt");
来源：http://ku.haigaiapp.cn

[F02] 逐行读取文件
来源：http://vz.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://yg.hnjuh.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://va.bjjhwx.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.bookmarksfly.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://yz.jctech888.com.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://vk.huixiangedu.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://tu.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://ol.nicolike.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://lc.shtwfgs.cn

[F03] 写入文件（覆盖）
来源：http://lj.wgjwhj.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://jx.nicolike.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://nr.huanxung.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://iy.521024.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://ku.huixiangedu.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mt.gzmigu.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://gc.asd995.cn

Ruby: File.write("a.txt", "hi")
来源：http://az.nicolike.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://pj.newstarts.cn

[F04] 追加写入文件
来源：http://jo.huixinmuqiang.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wb.yuexingan06.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://sq.szxytkj.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://ed.nicolike.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://bo.9csxet.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://pk.haigaiapp.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://tb.shxzukj.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wv.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://sf.hahajie.cn

[F05] 判断文件或目录是否存在
来源：http://og.haigaiapp.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ia.huanxung.cn

PHP:  file_exists("a.txt");
来源：http://ju.nszjky.cn

JS:   fs.existsSync("a.txt")
来源：http://pp.9csxet.cn

TS:   fs.existsSync("a.txt")
来源：http://fm.huixiangedu.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://ir.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://is.muxihuayi.cn

Ruby: File.exist?("a.txt")
来源：http://ig.wgjwhj.cn

C#:   File.Exists("a.txt")
来源：http://ml.newstarts.cn

[F06] 删除文件
来源：http://ug.huixinmuqiang.cn

Py:   os.remove("a.txt")
来源：http://xo.panjiajie.cn

PHP:  unlink("a.txt");
来源：http://oi.yuexingan06.cn

JS:   fs.unlinkSync("a.txt")
来源：http://zt.newstarts.cn

TS:   fs.unlinkSync("a.txt")
来源：http://ff.yuntaijiaju.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mi.haigaiapp.cn

Go:   os.Remove("a.txt")
来源：http://di.shxzskj.cn

Ruby: File.delete("a.txt")
来源：http://ir.lnxyls.cn

C#:   File.Delete("a.txt");
来源：http://vf.bjjhwx.cn

[F07] 创建目录（含多级）
来源：http://sn.shxzskj.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://us.huixiangedu.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://vb.yuntaijiaju.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ut.szsharing.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://vh.asd995.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://tj.521024.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://jc.asd995.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mq.521024.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://oe.shtwfgs.cn

[F08] 遍历目录
来源：http://qm.hahajie.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://vr.bjjhwx.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wb.newstarts.cn

JS:   fs.readdirSync("dir")
来源：http://il.shxzskj.cn

TS:   fs.readdirSync("dir")
来源：http://yh.bjjhwx.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://jh.wgjwhj.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://ye.haigaiapp.cn

Ruby: Dir.children("dir")
来源：http://wn.hnjuh.cn

C#:   Directory.GetFiles("dir")
来源：http://ut.newstarts.cn

[F09] 获取文件大小
来源：http://mt.521024.cn

Py:   os.path.getsize("a.txt")
来源：http://li.newstarts.cn

PHP:  filesize("a.txt");
来源：http://nj.haigaiapp.cn

JS:   fs.statSync("a.txt").size
来源：http://mq.wgjwhj.cn

TS:   fs.statSync("a.txt").size
来源：http://xd.newstarts.cn

Java: Files.size(Path.of("a.txt"))
来源：http://ox.hnjuh.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://jn.huixinmuqiang.cn

Ruby: File.size("a.txt")
来源：http://iw.gzmigu.cn

C#:   new FileInfo("a.txt").Length
来源：http://pf.jianghongdianzi.cn

[F10] 取文件扩展名 / 文件名
来源：http://je.asd995.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://tr.shxzskj.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://qs.huixinmuqiang.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wq.nicolike.cn

TS:   path.extname("a.txt")
来源：http://iv.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://bx.wgjwhj.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://sf.huixiangedu.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://yw.jianghongdianzi.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://sc.chemitech.net.cn

[F11] 复制与移动文件
来源：http://su.nszjky.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://ln.asd995.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ob.hnjuh.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ki.colortex.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://qm.nszjky.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wt.asd995.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://at.bjjhwx.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://pv.nszjky.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://sq.shxzskj.cn

[F12] CSV 读写
来源：http://jr.shxzukj.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://sr.muxihuayi.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mj.shxzskj.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://pp.gzmigu.cn

TS:   // 同上
来源：http://lo.chemitech.net.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://fz.shxzukj.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lu.panjiajie.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://fq.bookmarksfly.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://kg.yuexingan06.cn

================================================================================
来源：http://jl.hahajie.cn

G. 面向对象
来源：http://rn.yuntaijiaju.cn

================================================================================
来源：http://mr.huixiangedu.cn

[G01] 定义类
来源：http://jt.9csxet.cn

Py:   class User: pass
来源：http://at.shxzukj.cn

PHP:  class User {}
来源：http://yv.shxzskj.cn

JS:   class User {}
来源：http://qa.nicolike.cn

TS:   class User { name: string = ""; }
来源：http://ou.yuntaijiaju.cn

Java: class User {}
来源：http://bb.shxzukj.cn

Go:   type User struct { Name string }
来源：http://pk.hnjuh.cn

Ruby: class User; end
来源：http://xv.shtwfgs.cn

C#:   class User {}
来源：http://oq.nszjky.cn

[G02] 构造函数
来源：http://xi.hahajie.cn

Py:   def __init__(self, name): self.name = name
来源：http://qx.nszjky.cn

PHP:  public function __construct(public string $name) {}
来源：http://ge.hnjuh.cn

JS:   constructor(name) { this.name = name; }
来源：http://cw.bookmarksfly.cn

TS:   constructor(public name: string) {}
来源：http://zo.bjjhwx.cn

Java: User(String name) { this.name = name; }
来源：http://pe.shtwfgs.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://xy.gzmigu.cn

Ruby: def initialize(name); @name = name; end
来源：http://qp.asd995.cn

C#:   public User(string name) { Name = name; }
来源：http://tm.lnxyls.cn

[G03] 实例属性
来源：http://xf.szxytkj.cn

Py:   self.name = "x"
来源：http://zp.colortex.cn

PHP:  public string $name = "x";
来源：http://we.huixiangedu.cn

JS:   this.name = "x";
来源：http://lp.muxihuayi.cn

TS:   name: string = "x";
来源：http://iu.lnxyls.cn

Java: private String name;
来源：http://og.lnxyls.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://nx.muxihuayi.cn

Ruby: @name = "x"
来源：http://oc.panjiajie.cn

C#:   public string Name { get; set; } = "x";
来源：http://to.shtwfgs.cn

[G04] 定义方法
来源：http://zp.muxihuayi.cn

Py:   def greet(self): return self.name
来源：http://zz.bjjhwx.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://qa.huixinmuqiang.cn

JS:   greet() { return this.name; }
来源：http://fv.9csxet.cn

TS:   greet(): string { return this.name; }
来源：http://vf.nicolike.cn

Java: String greet() { return name; }
来源：http://ld.yuexingan06.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://yr.shxzskj.cn

Ruby: def greet; @name; end
来源：http://vd.colortex.cn

C#:   public string Greet() => Name;
来源：http://bx.muxihuayi.cn

[G05] 继承
来源：http://us.shxzskj.cn

Py:   class Admin(User): pass
来源：http://ue.szsharing.cn

PHP:  class Admin extends User {}
来源：http://po.nicolike.cn

JS:   class Admin extends User {}
来源：http://ud.hahajie.cn

TS:   class Admin extends User {}
来源：http://fj.panjiajie.cn

Java: class Admin extends User {}
来源：http://lj.chemitech.net.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://no.huanxung.cn

Ruby: class Admin < User; end
来源：http://en.yuntaijiaju.cn

C#:   class Admin : User {}
来源：http://gt.wgjwhj.cn

[G06] 重写方法
来源：http://cs.bjjhwx.cn

Py:   def greet(self): return "admin"
来源：http://uf.jianghongdianzi.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://ot.shxzukj.cn

JS:   greet() { return "admin"; }
来源：http://ra.huixiangedu.cn

TS:   greet(): string { return "admin"; }
来源：http://hg.chemitech.net.cn

Java: @Override String greet() { return "admin"; }
来源：http://hr.huanxung.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://du.szxytkj.cn

Ruby: def greet; "admin"; end
来源：http://lc.newstarts.cn

C#:   public override string Greet() => "admin";
来源：http://ln.szsharing.cn

[G07] 调用父类方法
来源：http://mx.colortex.cn

Py:   super().greet()
来源：http://km.521024.cn

PHP:  parent::greet();
来源：http://nc.huanxung.cn

JS:   super.greet();
来源：http://ac.panjiajie.cn

TS:   super.greet();
来源：http://if.huanxung.cn

Java: super.greet();
来源：http://na.shtwfgs.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mi.bjjhwx.cn

Ruby: super
来源：http://et.szsharing.cn

C#:   base.Greet();
来源：http://cx.yuexingan06.cn

[G08] 静态方法与属性
来源：http://ow.newstarts.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://ho.shxzukj.cn

PHP:  public static function f() {}
来源：http://bm.huanxung.cn

JS:   static f() {}
来源：http://ay.muxihuayi.cn

TS:   static f(): void {}
来源：http://cm.lnxyls.cn

Java: static void f() {}
来源：http://xx.huixinmuqiang.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://mv.nicolike.cn

Ruby: def self.f; end
来源：http://ox.jctech888.com.cn

C#:   public static void F() {}
来源：http://dk.muxihuayi.cn

[G09] 接口 / 抽象类
来源：http://kd.lnxyls.cn

Py:   from abc import ABC, abstractmethod
来源：http://ml.shtwfgs.cn

PHP:  interface Shape { public function area(): float; }
来源：http://ic.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://bo.szxytkj.cn

TS:   interface Shape { area(): number; }
来源：http://ly.yuexingan06.cn

Java: interface Shape { double area(); }
来源：http://tg.wgjwhj.cn

Go:   type Shape interface { Area() float64 }
来源：http://pn.jctech888.com.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://xl.yuexingan06.cn

C#:   interface IShape { double Area(); }
来源：http://fo.newstarts.cn

[G10] 访问控制
来源：http://mu.bjjhwx.cn

Py:   约定 _protected / __private（不强制）
来源：http://dr.shxzskj.cn

PHP:  public / protected / private
来源：http://aj.nszjky.cn

JS:   #private 字段；其余公开
来源：http://xg.shxzukj.cn

TS:   public / protected / private
来源：http://ha.hahajie.cn

Java: public / protected / private / 默认包级
来源：http://tj.hnjuh.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://hh.nszjky.cn

Ruby: public / protected / private
来源：http://eo.chemitech.net.cn

C#:   public / protected / private / internal
来源：http://hu.muxihuayi.cn

[G11] getter / setter
来源：http://ab.jctech888.com.cn

Py:   @property 与 @x.setter
来源：http://rt.huanxung.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ub.bjjhwx.cn

JS:   get name() { return this._name; }
来源：http://es.huixinmuqiang.cn

TS:   get name(): string { return this._name; }
来源：http://br.huanxung.cn

Java: public String getName() { return name; }
来源：http://mi.9csxet.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://tm.wgjwhj.cn

Ruby: attr_accessor :name
来源：http://vg.9csxet.cn

C#:   public string Name { get; set; }
来源：http://xl.shtwfgs.cn

[G12] 对象转字符串
来源：http://sg.panjiajie.cn

Py:   def __str__(self): return self.name
来源：http://ea.hnjuh.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://df.shxzukj.cn

JS:   toString() { return this.name; }
来源：http://if.chemitech.net.cn

TS:   toString(): string { return this.name; }
来源：http://lm.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://mk.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://ah.panjiajie.cn

Ruby: def to_s; @name; end
来源：http://vd.muxihuayi.cn

C#:   public override string ToString() => Name;
来源：http://kg.wgjwhj.cn

[G13] 判断对象类型
来源：http://zj.yuntaijiaju.cn

Py:   isinstance(u, User)
来源：http://lx.huixiangedu.cn

PHP:  $u instanceof User
来源：http://ut.jctech888.com.cn

JS:   u instanceof User
来源：http://kf.hahajie.cn

TS:   u instanceof User
来源：http://zd.hnjuh.cn

Java: u instanceof User
来源：http://cw.9csxet.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://cv.wgjwhj.cn

Ruby: u.is_a?(User)
来源：http://zg.521024.cn

C#:   u is User
来源：http://cc.bjjhwx.cn

[G14] 数据类 / record
来源：http://fi.bjjhwx.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mr.yuexingan06.cn

PHP:  // 用 readonly 属性模拟
来源：http://xc.hahajie.cn

JS:   // 无内置：普通类或对象字面量
来源：http://be.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://ay.lnxyls.cn

Java: record User(String name, int age) {}
来源：http://hc.shxzukj.cn

Go:   type User struct { Name string; Age int }
来源：http://px.panjiajie.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://gq.bookmarksfly.cn

C#:   record User(string Name, int Age);
来源：http://jw.shxzskj.cn

[G15] 枚举
来源：http://yn.nszjky.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hi.huixinmuqiang.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://hq.9csxet.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://sz.gzmigu.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://ot.shxzskj.cn

Java: enum Color { RED, GREEN }
来源：http://ic.asd995.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://si.jianghongdianzi.cn

Ruby: Color = %i[red green].freeze
来源：http://uc.szxytkj.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ls.lnxyls.cn

[G16] 对象转数组 / 字典
来源：http://te.huixinmuqiang.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://fj.huanxung.cn

PHP:  get_object_vars($obj);
来源：http://pt.lnxyls.cn

JS:   Object.entries(obj)
来源：http://ue.nicolike.cn

TS:   Object.entries(obj)
来源：http://hw.gzmigu.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://tj.shtwfgs.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://by.huanxung.cn

Ruby: obj.instance_variables
来源：http://ya.shxzukj.cn

C#:   // 用反射或 System.Text.Json
来源：http://cw.huixinmuqiang.cn

================================================================================
来源：http://rr.huixinmuqiang.cn

H. 异常与错误处理
来源：http://lb.bjjhwx.cn

================================================================================
来源：http://dx.newstarts.cn

[H01] try / catch 基础
来源：http://vx.yuntaijiaju.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://uv.521024.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://kj.9csxet.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://ky.colortex.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://yn.newstarts.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://xx.lnxyls.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://yr.nszjky.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ha.huanxung.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ac.chemitech.net.cn

[H02] finally / ensure 收尾
来源：http://kq.bookmarksfly.cn

Py:   try: f()⏎finally: cleanup()
来源：http://dk.newstarts.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://pe.gzmigu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://sj.9csxet.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://fg.yuexingan06.cn

Java: try { f(); } finally { cleanup(); }
来源：http://un.shxzskj.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://pm.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://sq.hahajie.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://of.haigaiapp.cn

[H03] 主动抛出异常
来源：http://gg.hnjuh.cn

Py:   raise ValueError("错误信息")
来源：http://rx.haigaiapp.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://rr.wgjwhj.cn

JS:   throw new Error("错误信息");
来源：http://he.newstarts.cn


<!-- 参考信息 -->