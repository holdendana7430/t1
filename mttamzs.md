代发 wailian999

[E22] 字节长度与字符长度
来源：http://ba.jctech888.com.cn

Py:   len(s.encode("utf-8"));  len(s)
来源：http://nc.bjjhwx.cn

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://od.jianghongdianzi.cn

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://od.huixinmuqiang.cn

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://ks.nicolike.cn

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://fu.huixinmuqiang.cn

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://xo.szxytkj.cn

Ruby: s.bytesize;  s.length
来源：http://lz.9csxet.cn

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://xe.shtwfgs.cn

================================================================================
来源：http://eb.521024.cn

F. 文件与目录
来源：http://ml.wgjwhj.cn

================================================================================
来源：http://rb.9csxet.cn

[F01] 读取整个文件
来源：http://ql.yuexingan06.cn

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://py.huixiangedu.cn

PHP:  file_get_contents("a.txt");
来源：http://ef.nicolike.cn

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://ed.wgjwhj.cn

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://ba.lnxyls.cn

Java: Files.readString(Path.of("a.txt"))
来源：http://dy.panjiajie.cn

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://go.bjjhwx.cn

Ruby: File.read("a.txt")
来源：http://ja.hnjuh.cn

C#:   File.ReadAllText("a.txt");
来源：http://kf.haigaiapp.cn

[F02] 逐行读取文件
来源：http://qx.bjjhwx.cn

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wc.chemitech.net.cn

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://pt.jctech888.com.cn

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://rz.szxytkj.cn

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://pw.hahajie.cn

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://el.bjjhwx.cn

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mf.newstarts.cn

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://fb.panjiajie.cn

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wt.bjjhwx.cn

[F03] 写入文件（覆盖）
来源：http://qz.huanxung.cn

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://oe.bjjhwx.cn

PHP:  file_put_contents("a.txt", "hi");
来源：http://db.huixinmuqiang.cn

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://jh.chemitech.net.cn

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wz.jctech888.com.cn

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://tb.yuexingan06.cn

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://qe.huanxung.cn

Ruby: File.write("a.txt", "hi")
来源：http://vs.haigaiapp.cn

C#:   File.WriteAllText("a.txt", "hi");
来源：http://gw.jianghongdianzi.cn

[F04] 追加写入文件
来源：http://tx.szxytkj.cn

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://an.szsharing.cn

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://xu.hnjuh.cn

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://uw.newstarts.cn

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://gi.gzmigu.cn

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://vl.jctech888.com.cn

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://pq.chemitech.net.cn

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mp.szsharing.cn

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://dc.szxytkj.cn

[F05] 判断文件或目录是否存在
来源：http://co.nszjky.cn

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://ox.jianghongdianzi.cn

PHP:  file_exists("a.txt");
来源：http://fl.jianghongdianzi.cn

JS:   fs.existsSync("a.txt")
来源：http://zi.chemitech.net.cn

TS:   fs.existsSync("a.txt")
来源：http://ij.newstarts.cn

Java: Files.exists(Path.of("a.txt"))
来源：http://vo.muxihuayi.cn

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://je.hnjuh.cn

Ruby: File.exist?("a.txt")
来源：http://iq.nszjky.cn

C#:   File.Exists("a.txt")
来源：http://bu.chemitech.net.cn

[F06] 删除文件
来源：http://ee.521024.cn

Py:   os.remove("a.txt")
来源：http://lk.gzmigu.cn

PHP:  unlink("a.txt");
来源：http://lk.9csxet.cn

JS:   fs.unlinkSync("a.txt")
来源：http://ww.muxihuayi.cn

TS:   fs.unlinkSync("a.txt")
来源：http://vz.haigaiapp.cn

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://yt.asd995.cn

Go:   os.Remove("a.txt")
来源：http://dy.chemitech.net.cn

Ruby: File.delete("a.txt")
来源：http://dw.shxzskj.cn

C#:   File.Delete("a.txt");
来源：http://cs.szsharing.cn

[F07] 创建目录（含多级）
来源：http://an.huanxung.cn

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://sm.521024.cn

PHP:  mkdir("dir/sub", 0777, true);
来源：http://gs.9csxet.cn

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://ur.lnxyls.cn

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://nh.bookmarksfly.cn

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://rt.9csxet.cn

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://vv.nicolike.cn

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://zk.hnjuh.cn

C#:   Directory.CreateDirectory("dir/sub");
来源：http://zd.lnxyls.cn

[F08] 遍历目录
来源：http://hx.asd995.cn

Py:   for name in os.listdir("dir"): print(name)
来源：http://wr.hahajie.cn

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://ib.jctech888.com.cn

JS:   fs.readdirSync("dir")
来源：http://px.yuexingan06.cn

TS:   fs.readdirSync("dir")
来源：http://gz.chemitech.net.cn

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://ia.huixinmuqiang.cn

Go:   entries, _ := os.ReadDir("dir")
来源：http://yi.muxihuayi.cn

Ruby: Dir.children("dir")
来源：http://io.muxihuayi.cn

C#:   Directory.GetFiles("dir")
来源：http://zx.shxzukj.cn

[F09] 获取文件大小
来源：http://jy.newstarts.cn

Py:   os.path.getsize("a.txt")
来源：http://py.chemitech.net.cn

PHP:  filesize("a.txt");
来源：http://yx.jianghongdianzi.cn

JS:   fs.statSync("a.txt").size
来源：http://jn.huixinmuqiang.cn

TS:   fs.statSync("a.txt").size
来源：http://gi.nicolike.cn

Java: Files.size(Path.of("a.txt"))
来源：http://on.szxytkj.cn

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://zg.asd995.cn

Ruby: File.size("a.txt")
来源：http://rb.9csxet.cn

C#:   new FileInfo("a.txt").Length
来源：http://hu.9csxet.cn

[F10] 取文件扩展名 / 文件名
来源：http://as.9csxet.cn

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://nu.gzmigu.cn

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://xo.muxihuayi.cn

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://qm.wgjwhj.cn

TS:   path.extname("a.txt")
来源：http://vj.bookmarksfly.cn

Java: // 手动 substring(lastIndexOf('.'))
来源：http://nq.jianghongdianzi.cn

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://rq.bjjhwx.cn

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://zl.wgjwhj.cn

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://le.lnxyls.cn

[F11] 复制与移动文件
来源：http://ub.nicolike.cn

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mg.chemitech.net.cn

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://ww.nicolike.cn

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://ds.bjjhwx.cn

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://id.muxihuayi.cn

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://nk.jianghongdianzi.cn

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://nb.9csxet.cn

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://bw.hahajie.cn

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://si.jctech888.com.cn

[F12] CSV 读写
来源：http://tv.yuntaijiaju.cn

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://gm.wgjwhj.cn

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://kd.jianghongdianzi.cn

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://uo.nszjky.cn

TS:   // 同上
来源：http://xz.wgjwhj.cn

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://qg.yuexingan06.cn

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://lv.nszjky.cn

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://bm.huanxung.cn

C#:   // 无内置：用 CsvHelper 库
来源：http://hx.hahajie.cn

================================================================================
来源：http://yu.nicolike.cn

G. 面向对象
来源：http://kl.jctech888.com.cn

================================================================================
来源：http://ul.chemitech.net.cn

[G01] 定义类
来源：http://jm.hnjuh.cn

Py:   class User: pass
来源：http://de.jianghongdianzi.cn

PHP:  class User {}
来源：http://in.9csxet.cn

JS:   class User {}
来源：http://su.chemitech.net.cn

TS:   class User { name: string = ""; }
来源：http://yw.yuntaijiaju.cn

Java: class User {}
来源：http://dt.szxytkj.cn

Go:   type User struct { Name string }
来源：http://nk.wgjwhj.cn

Ruby: class User; end
来源：http://vn.bookmarksfly.cn

C#:   class User {}
来源：http://ym.panjiajie.cn

[G02] 构造函数
来源：http://gq.hnjuh.cn

Py:   def __init__(self, name): self.name = name
来源：http://ya.colortex.cn

PHP:  public function __construct(public string $name) {}
来源：http://fu.szxytkj.cn

JS:   constructor(name) { this.name = name; }
来源：http://fa.yuntaijiaju.cn

TS:   constructor(public name: string) {}
来源：http://dw.shxzukj.cn

Java: User(String name) { this.name = name; }
来源：http://ss.nicolike.cn

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://dz.hahajie.cn

Ruby: def initialize(name); @name = name; end
来源：http://ik.yuexingan06.cn

C#:   public User(string name) { Name = name; }
来源：http://ex.jianghongdianzi.cn

[G03] 实例属性
来源：http://nw.panjiajie.cn

Py:   self.name = "x"
来源：http://ux.521024.cn

PHP:  public string $name = "x";
来源：http://vt.9csxet.cn

JS:   this.name = "x";
来源：http://zl.wgjwhj.cn

TS:   name: string = "x";
来源：http://ex.haigaiapp.cn

Java: private String name;
来源：http://tj.yuexingan06.cn

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://fl.bookmarksfly.cn

Ruby: @name = "x"
来源：http://fm.muxihuayi.cn

C#:   public string Name { get; set; } = "x";
来源：http://ya.muxihuayi.cn

[G04] 定义方法
来源：http://vj.yuntaijiaju.cn

Py:   def greet(self): return self.name
来源：http://ah.gzmigu.cn

PHP:  public function greet(): string { return $this->name; }
来源：http://ke.huanxung.cn

JS:   greet() { return this.name; }
来源：http://zt.colortex.cn

TS:   greet(): string { return this.name; }
来源：http://bp.shxzskj.cn

Java: String greet() { return name; }
来源：http://td.hnjuh.cn

Go:   func (u User) Greet() string { return u.Name }
来源：http://bk.panjiajie.cn

Ruby: def greet; @name; end
来源：http://sn.9csxet.cn

C#:   public string Greet() => Name;
来源：http://sv.9csxet.cn

[G05] 继承
来源：http://gs.bjjhwx.cn

Py:   class Admin(User): pass
来源：http://mz.haigaiapp.cn

PHP:  class Admin extends User {}
来源：http://ih.haigaiapp.cn

JS:   class Admin extends User {}
来源：http://cb.muxihuayi.cn

TS:   class Admin extends User {}
来源：http://ht.szxytkj.cn

Java: class Admin extends User {}
来源：http://tu.jianghongdianzi.cn

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://xd.szsharing.cn

Ruby: class Admin < User; end
来源：http://oe.521024.cn

C#:   class Admin : User {}
来源：http://md.jctech888.com.cn

[G06] 重写方法
来源：http://mz.colortex.cn

Py:   def greet(self): return "admin"
来源：http://wk.huixiangedu.cn

PHP:  public function greet(): string { return "admin"; }
来源：http://dr.newstarts.cn

JS:   greet() { return "admin"; }
来源：http://ga.szsharing.cn

TS:   greet(): string { return "admin"; }
来源：http://df.shtwfgs.cn

Java: @Override String greet() { return "admin"; }
来源：http://qw.szxytkj.cn

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://af.shtwfgs.cn

Ruby: def greet; "admin"; end
来源：http://wn.shxzukj.cn

C#:   public override string Greet() => "admin";
来源：http://oq.haigaiapp.cn

[G07] 调用父类方法
来源：http://ee.shtwfgs.cn

Py:   super().greet()
来源：http://nz.lnxyls.cn

PHP:  parent::greet();
来源：http://dd.huixiangedu.cn

JS:   super.greet();
来源：http://rz.9csxet.cn

TS:   super.greet();
来源：http://fg.hnjuh.cn

Java: super.greet();
来源：http://nw.wgjwhj.cn

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://nz.shtwfgs.cn

Ruby: super
来源：http://ai.lnxyls.cn

C#:   base.Greet();
来源：http://ip.hnjuh.cn

[G08] 静态方法与属性
来源：http://yc.yuntaijiaju.cn

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://nk.panjiajie.cn

PHP:  public static function f() {}
来源：http://jc.bjjhwx.cn

JS:   static f() {}
来源：http://hm.9csxet.cn

TS:   static f(): void {}
来源：http://zk.bjjhwx.cn

Java: static void f() {}
来源：http://rg.haigaiapp.cn

Go:   // 无 static：用包级函数，按包名调用
来源：http://bk.lnxyls.cn

Ruby: def self.f; end
来源：http://sn.hnjuh.cn

C#:   public static void F() {}
来源：http://zh.asd995.cn

[G09] 接口 / 抽象类
来源：http://pa.huanxung.cn

Py:   from abc import ABC, abstractmethod
来源：http://cr.521024.cn

PHP:  interface Shape { public function area(): float; }
来源：http://jr.wgjwhj.cn

JS:   // 无接口：靠约定或 JSDoc
来源：http://dn.lnxyls.cn

TS:   interface Shape { area(): number; }
来源：http://pr.chemitech.net.cn

Java: interface Shape { double area(); }
来源：http://mm.521024.cn

Go:   type Shape interface { Area() float64 }
来源：http://kx.bjjhwx.cn

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://ri.huixinmuqiang.cn

C#:   interface IShape { double Area(); }
来源：http://qk.szsharing.cn

[G10] 访问控制
来源：http://xc.asd995.cn

Py:   约定 _protected / __private（不强制）
来源：http://el.shxzskj.cn

PHP:  public / protected / private
来源：http://bz.yuntaijiaju.cn

JS:   #private 字段；其余公开
来源：http://kd.szsharing.cn

TS:   public / protected / private
来源：http://bw.newstarts.cn

Java: public / protected / private / 默认包级
来源：http://du.wgjwhj.cn

Go:   首字母大写可导出，小写仅包内可见
来源：http://cz.colortex.cn

Ruby: public / protected / private
来源：http://ox.shxzukj.cn

C#:   public / protected / private / internal
来源：http://sn.shtwfgs.cn

[G11] getter / setter
来源：http://jc.hnjuh.cn

Py:   @property 与 @x.setter
来源：http://fu.haigaiapp.cn

PHP:  public function getName(): string { return $this->name; }
来源：http://ie.shxzukj.cn

JS:   get name() { return this._name; }
来源：http://qf.huanxung.cn

TS:   get name(): string { return this._name; }
来源：http://us.gzmigu.cn

Java: public String getName() { return name; }
来源：http://fq.huixinmuqiang.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://rl.huixinmuqiang.cn

Ruby: attr_accessor :name
来源：http://wd.nszjky.cn

C#:   public string Name { get; set; }
来源：http://if.wgjwhj.cn

[G12] 对象转字符串
来源：http://bm.newstarts.cn

Py:   def __str__(self): return self.name
来源：http://qz.wgjwhj.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://jv.colortex.cn

JS:   toString() { return this.name; }
来源：http://ar.hnjuh.cn

TS:   toString(): string { return this.name; }
来源：http://bs.gzmigu.cn

Java: @Override public String toString() { return name; }
来源：http://nw.huixiangedu.cn

Go:   func (u User) String() string { return u.Name }
来源：http://eu.szxytkj.cn

Ruby: def to_s; @name; end
来源：http://iw.gzmigu.cn

C#:   public override string ToString() => Name;
来源：http://hj.shtwfgs.cn

[G13] 判断对象类型
来源：http://uk.yuexingan06.cn

Py:   isinstance(u, User)
来源：http://ru.9csxet.cn

PHP:  $u instanceof User
来源：http://or.shxzukj.cn

JS:   u instanceof User
来源：http://cr.colortex.cn

TS:   u instanceof User
来源：http://ex.nicolike.cn

Java: u instanceof User
来源：http://sy.jctech888.com.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://sm.9csxet.cn

Ruby: u.is_a?(User)
来源：http://no.shxzukj.cn

C#:   u is User
来源：http://hg.nicolike.cn

[G14] 数据类 / record
来源：http://yb.9csxet.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://tu.szxytkj.cn

PHP:  // 用 readonly 属性模拟
来源：http://ht.newstarts.cn

JS:   // 无内置：普通类或对象字面量
来源：http://ku.hnjuh.cn

TS:   type User = { name: string; age: number };
来源：http://dj.huixinmuqiang.cn

Java: record User(String name, int age) {}
来源：http://jo.bookmarksfly.cn

Go:   type User struct { Name string; Age int }
来源：http://xe.wgjwhj.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://jd.yuexingan06.cn

C#:   record User(string Name, int Age);
来源：http://yu.szsharing.cn

[G15] 枚举
来源：http://xa.521024.cn

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://un.szsharing.cn

PHP:  enum Color: string { case Red = "red"; }
来源：http://lb.huixiangedu.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://dv.hahajie.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://lm.9csxet.cn

Java: enum Color { RED, GREEN }
来源：http://sc.szxytkj.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://ap.haigaiapp.cn

Ruby: Color = %i[red green].freeze
来源：http://ew.haigaiapp.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://av.521024.cn

[G16] 对象转数组 / 字典
来源：http://wa.nszjky.cn

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://ef.huixiangedu.cn

PHP:  get_object_vars($obj);
来源：http://ul.asd995.cn

JS:   Object.entries(obj)
来源：http://br.szxytkj.cn

TS:   Object.entries(obj)
来源：http://pe.yuntaijiaju.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://yf.lnxyls.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://do.wgjwhj.cn

Ruby: obj.instance_variables
来源：http://du.yuntaijiaju.cn

C#:   // 用反射或 System.Text.Json
来源：http://fa.521024.cn

================================================================================
来源：http://yq.yuntaijiaju.cn

H. 异常与错误处理
来源：http://kp.szxytkj.cn

================================================================================
来源：http://tz.shxzskj.cn

[H01] try / catch 基础
来源：http://zz.yuexingan06.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://do.szxytkj.cn

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://rj.colortex.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://rn.huixinmuqiang.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://ek.shxzskj.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://qw.muxihuayi.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wv.shxzskj.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wk.newstarts.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://gr.521024.cn

[H02] finally / ensure 收尾
来源：http://vp.bjjhwx.cn

Py:   try: f()⏎finally: cleanup()
来源：http://kk.jctech888.com.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://lh.muxihuayi.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://mz.szsharing.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://vr.muxihuayi.cn

Java: try { f(); } finally { cleanup(); }
来源：http://se.521024.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://rf.jctech888.com.cn

Ruby: begin; f; ensure; cleanup; end
来源：http://pv.gzmigu.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://lm.bjjhwx.cn

[H03] 主动抛出异常
来源：http://qz.shtwfgs.cn

Py:   raise ValueError("错误信息")
来源：http://hm.nicolike.cn

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://hr.shxzukj.cn

JS:   throw new Error("错误信息");
来源：http://kp.yuexingan06.cn

TS:   throw new Error("错误信息");
来源：http://yf.gzmigu.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://cw.9csxet.cn

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://sa.521024.cn

Ruby: raise ArgumentError, "错误信息"
来源：http://fu.shxzskj.cn

C#:   throw new ArgumentException("错误信息");
来源：http://zn.nicolike.cn

[H04] 自定义异常类型
来源：http://qv.wgjwhj.cn

Py:   class MyError(Exception): pass
来源：http://qx.shxzskj.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ed.wgjwhj.cn


<!-- 参考信息 -->